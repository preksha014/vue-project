<template>
    <div>
        <input type="text" :value="modelValue" @input="$emit('update:modelValue', $event.target.value)" />
    </div>
</template>

<script setup>
defineProps(['modelValue'])

</script>

<style scoped>
.input {
    padding: 10px;
    border: 1px solid #ccc;
    border-radius: 4px;
    width: 100%;
    box-sizing: border-box;
    font-size: 16px;
    transition: border-color 0.3s ease;
    outline: none;
}
</style>