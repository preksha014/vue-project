<script setup>
defineProps(['personName'])
</script>

<template>
  <div class="greetings">
    <h1 class="heading">Hello, {{ personName }}</h1>
  </div>
</template>

<style scoped>
.greetings {
  text-align: center;
}

.heading {
  color: green;
}
</style>
