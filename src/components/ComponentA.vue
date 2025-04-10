<template>
    <ComponentB/>
    <div>

    </div>
</template>

<script setup>
import ComponentB from './ComponentB.vue';
import { provide } from 'vue'
const personName = 'sdbebdj'
provide('personName',personName)
</script>

<style lang="scss" scoped>

</style>