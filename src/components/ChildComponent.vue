<template>
    <div>
        <p>{{ message }}</p>
        <input type="color" v-model="color" @input="changeColor">
    </div>
</template>

<script setup>
    import { ref } from 'vue';
    import { defineProps, defineEmits } from 'vue';

    const props = defineProps({
        message: {
            type: String,
            required: true
        }
    });

    const emit = defineEmits(['colorChanged']);

    const color = ref('#ffffff');

    function changeColor() {
        emit('colorChanged', color.value);
    }
</script>