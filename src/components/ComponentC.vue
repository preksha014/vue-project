<template>
    <div>
        componentC
        {{ personName }}
    </div>
</template>

<script setup>
import { inject } from 'vue'

const personName = inject('personName')
</script>

<style lang="scss" scoped></style>