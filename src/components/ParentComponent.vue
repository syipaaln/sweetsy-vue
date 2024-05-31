<template>
    <div :style="{ backgroundColor: backgroundColor }">
        <child-component 
            :message="parentMessage" 
            @colorChanged="handleColorChanged"
        ></child-component>
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
  