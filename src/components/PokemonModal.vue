<template>
    <div v-if="showModal" class="fixed inset-0 flex items-center justify-center bg-black bg-opacity-50 p-4">
        <div class="bg-white p-6 rounded-lg shadow-lg w-full max-w-md md:max-w-lg lg:max-w-xl">
            <div class="flex justify-between items-center border-b pb-3">
                <h2 class="text-xl font-bold capitalize">{{ pokemon.name }}'s Stats</h2>
                <button @click="closeModal" class="text-black font-bold text-2xl leading-none">&times;</button>
            </div>
            <nav class="flex justify-center my-4">
                <button
                    v-for="(stat, index) in pokemon.stats"
                    :key="index"
                    @click="activeStat = stat.stat.name"
                    :class="['px-2 capitalize', activeStat === stat.stat.name ? 'font-bold' : 'font-medium hover:opacity-70']">
                    {{ stat.stat.name }}
                </button>
            </nav>
            <div v-for="(stat, index) in pokemon.stats" :key="index" class="mt-4">
                <div v-if="activeStat === stat.stat.name">
                    <span class="text-lg font-bold mb-2 capitalize block">{{ stat.stat.name }}:</span>
                    <div class="w-full bg-gray-200 rounded h-10 overflow-hidden">
                        <div class="bg-blue-500 h-full rounded" :style="{ width: stat.base_stat + '%' }">
                            <div class="ml-2 text-lg pt-1 text-white">{{ stat.base_stat }}%</div>
                        </div>
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

const activeStat = ref('hp');

const closeModal = () => {
    emit('close');
}
</script>