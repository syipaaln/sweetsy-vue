<template>
    <div v-if="showModal" class="fixed inset-0 flex items-center justify-center bg-black bg-opacity-50">
        <div class="bg-white p-6 rounded-lg shadow-lg w-1/2">
            <div class="flex justify-between items-center">
                <h2 class="text-xl font-bold capitalize">{{ pokemon.name }}'s Stats</h2>
                <button @click="closeModal" class="text-black font-bold">&times;</button>
            </div>
            <div v-for="(stat, index) in pokemon.stats" :key="index" class="mt-4">
                <span class="text-lg">{{ stat.stat.name }}:</span>
                <span class="text-lg font-bold">{{ stat.base_stat }}%</span>
            </div>
        </div>
    </div>
</template>

<script setup>
import { defineProps, defineEmits } from 'vue';

const props = defineProps({
    showModal: Boolean,
    pokemon: Object
});

const emit = defineEmits(['close']);

const closeModal = () => {
    emit('close');
}
</script>