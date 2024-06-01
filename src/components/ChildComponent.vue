<template>
    <div class="p-4 border rounded shadow-md">
        <p class="text-lg font-medium mb-4">{{ message }}</p>
        <input type="color" v-model="color" @input="changeColor" class="rounded">
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