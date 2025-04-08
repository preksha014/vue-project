<script setup>
import { onMounted, useTemplateRef, ref } from 'vue';


const list = ref(['Item 1', 'Item 2', 'Item 3']);

const itemsRef = useTemplateRef('items');

onMounted(() => console.log(itemsRef.value));
</script>

<template>
    <ul>
        <li v-for="item in list" :key="item.id" ref="items">{{ item }}</li>
    </ul>
</template>

<style scoped></style>