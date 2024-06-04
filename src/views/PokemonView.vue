<template>
    <div class="min-h-screen bg-black p-20">
        <div class="grid grid-cols-1 sm:grid-cols-2 md:grid-cols-3 lg:grid-cols-4 xl:grid-cols-5 gap-6">
            <div class="flex items-center bg-blue-300 p-8 rounded shadow-lg" v-for="(p, index) in pokemon" :key="index">
                <span class="flex-grow text-lg font-medium">{{ p.name }}</span>
                <img :src="p.sprites.front_default" alt="p.name" class="w-20 h-20">
            </div>
        </div>
    </div>
</template>

<script setup>
import { ref, onMounted } from 'vue';
import axios from 'axios';

const pokemon = ref([])

onMounted(() => {
    axios
    .get('https://pokeapi.co/api/v2/pokemon?offset=0&limit=15')
    .then(response => {
        const pokemonPromises = response.data.results.map(p => axios.get(p.url));
        Promise.all(pokemonPromises).then(responses => {
            pokemon.value = responses.map(r => r.data);
        });
    })
})
</script>