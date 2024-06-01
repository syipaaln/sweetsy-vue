<template>
    <div :style="{ backgroundColor: backgroundColor }"  class="p-8 min-h-screen">
        <h1 class="text-2xl font-bold mb-6">Parent Component</h1>
        <child-component 
            :message="parentMessage" 
            @colorChanged="handleColorChanged"
            class="mb-4"
        ></child-component>
        <p class="text-xl">Selected Color: {{ backgroundColor }}</p>
    </div>
</template>

<script setup>
    import { ref } from 'vue';
    import ChildComponent from './ChildComponent.vue';

    const backgroundColor = ref('#ffffff')

    const parentMessage = ref('Ayo ubah warna latar belakang!');

    function handleColorChanged(color) {
        backgroundColor.value = color;
    }
</script>
  