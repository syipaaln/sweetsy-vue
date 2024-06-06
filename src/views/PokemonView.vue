<template>
    <div class="min-h-screen bg-black p-16">
        <PokemonList :pokemons="pokemons" @select="selectPokemon" />
        <PokemonModal :showModal="showModal" :pokemon="selectedPokemon" @close="closeModal" />
    </div>
</template>

<script setup>
import { ref, onMounted } from 'vue';
import axios from 'axios';
import PokemonList from '../components/PokemonList.vue'
import PokemonModal from '../components/PokemonModal.vue'

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