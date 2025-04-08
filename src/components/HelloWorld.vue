<script setup> 
defineProps({
  personName: {
    type: String,
    required: true
  },
  age: {
    type: Number,
    default: 0
  }
});
</script>

<template>
  <div class="greetings">
    <h1 class="heading">Hello, {{ personName }} {{ age }}</h1>
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
