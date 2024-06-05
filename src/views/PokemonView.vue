<template>
    <div class="min-h-screen bg-black p-16">
        <div class="grid grid-cols-1 sm:grid-cols-2 md:grid-cols-3 lg:grid-cols-4 xl:grid-cols-5 gap-7">
            <div class="flex items-center bg-blue-300 p-7 rounded shadow-lg cursor-pointer hover:opacity-50" v-for="(pokemon, index) in pokemons" :key="index" @click="selectPokemon(pokemon)">
                <span class="flex-grow text-lg font-medium capitalize">{{ pokemon.name }}</span>
                <img :src="pokemon.sprites.front_default" :alt="pokemon.name" class="w-24 h-24">
            </div>
        </div>
        <div v-if="showModal" class="fixed inset-0 flex items-center justify-center bg-black bg-opacity-50">
            <div class="bg-white p-6 rounded-lg shadow-lg w-1/2">
                <div class="flex justify-between items-center">
                    <h2 class="text-xl font-bold capitalize">{{ selectedPokemon.name }}'s Stats</h2>
                    <button @click="closeModal" class="text-black font-bold">&times;</button>
                </div>
                <div v-for="(stat, index) in selectedPokemon.stats" :key="index" class="mt-4">
                    <span class="text-lg">{{ stat.stat.name }}:</span>
                    <span class="text-lg font-bold">{{ stat.base_stat }}%</span>
                </div>
            </div>
        </div>
    </div>
</template>

<script setup>
import { ref, onMounted } from 'vue';
import axios from 'axios';

const pokemons = ref([])
const selectedPokemon = ref(null)
const showModal = ref(false);

const selectPokemon = (pokemon) => {
    showModal.value = true;
    selectedPokemon.value = pokemon;
}

const closeModal = () => {
    showModal.value = false;
};

onMounted(() => {
    axios
    .get('https://pokeapi.co/api/v2/pokemon?offset=0&limit=15')
    .then(response => {
        const pokemonPromises = response.data.results.map(pokemon => axios.get(pokemon.url));
        Promise.all(pokemonPromises).then(responses => {
            pokemons.value = responses.map(r => r.data);
        });
    })
})
</script>