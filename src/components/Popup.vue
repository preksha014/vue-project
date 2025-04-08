<template>
    <div>
        <h1>Popup</h1>
        <button @click="emit('close')">Close Popup</button>
    </div>
</template>

<script setup>
const emit = defineEmits(['close'])
</script>
<style lang="scss" scoped></style>