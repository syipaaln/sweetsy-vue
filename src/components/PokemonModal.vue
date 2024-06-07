<template>
    <div v-if="showModal" class="fixed inset-0 flex items-center justify-center bg-black bg-opacity-50">
        <div class="bg-white p-6 rounded-lg shadow-lg w-1/2">
            <div class="flex justify-between items-center">
                <h2 class="text-xl font-bold capitalize">{{ pokemon.name }}'s Stats</h2>
                <button @click="closeModal" class="text-black font-bold">&times;</button>
            </div>
            <nav class="flex justify-center space-x-4 mb-4">
                <button
                    v-for="(stat, index) in pokemon.stats"
                    :key="index"
                    @click="activeStat = stat.stat.name"
                    :class="['px-2 capitalize', activeStat === stat.stat.name ? 'font-bold' : 'font-medium']">
                    {{ stat.stat.name }}
                </button>
            </nav>
            <div v-for="(stat, index) in pokemon.stats" :key="index" class="mt-4">
                <span class="text-lg font-bold mb-2 capitalize">{{ stat.stat.name }}:</span>
                <div class="w-full bg-gray-200 rounded h-6">
                    <div class="bg-blue-500 h-6 rounded" :style="{ width: stat.base_stat + '%' }">
                        <div class="ml-2">{{ stat.base_stat }}%</div>
                    </div>
                </div>
            </div>
        </div>
    </div>
</template>

<script setup>
import { ref, defineProps, defineEmits } from 'vue';

const props = defineProps({
    showModal: Boolean,
    pokemon: Object
});

const emit = defineEmits(['close']);

const activeStat = ref(props.pokemon.stats[0].stat.name);

const closeModal = () => {
    emit('close');
}
</script>