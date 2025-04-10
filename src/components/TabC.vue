<template>
    <div>
        <h1>Tab C content</h1>
        <input type="text" v-model="name" />
    </div>
</template>

<script setup>
import { ref } from 'vue'
const name = ref('');
</script>

<style scoped></style>