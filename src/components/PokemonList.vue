<template>
    <div class="grid grid-cols-1 sm:grid-cols-2 md:grid-cols-3 lg:grid-cols-4 xl:grid-cols-5 gap-7">
        <div class="flex items-center bg-blue-300 p-7 rounded shadow-lg cursor-pointer hover:opacity-50" v-for="(pokemon, index) in pokemons" :key="index" @click="handleSelect(pokemon)">
            <span class="flex-grow text-lg font-medium capitalize">{{ pokemon.name }}</span>
            <img :src="pokemon.sprites.front_default" :alt="pokemon.name" class="w-24 h-24">
        </div>
    </div>
</template>

<script setup>
import { defineProps, defineEmits } from 'vue';

const props = defineProps({
    pokemons: Array
});

const emit = defineEmits(['select']);

const handleSelect = (pokemon) => {
    emit('select', pokemon);
};
</script>