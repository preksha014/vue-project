<script setup>
import { reactive, ref } from 'vue'

const firstName = "Preksha";

const lastName = "<p style=\"color:blue\">Rana</p>";

const objAttribute = {
  id: 'container',
  class: 'wrapper',
  style: 'background-color:pink; color:white; margin-top:5px;padding:10px; border-radius:10px;width:200px;'
};

const count = ref(0);

function increment() {
  count.value++
};

const classObj = {
  active: true,
  'text-danger': false
};

const styleObj = {
  color: 'red',
  fontSize: '20px'
};

const obj = reactive({
  name: 'Preksha',
  age: 22,
  city: 'Delhi'
});

function showData() {
  obj.name = 'Prekshii';
};

const awesome = ref(true);

const parentMessage = ref('Parent')
const items = ref([{ message: 'Foo' }, { message: 'Bar' }])

function greet(msg) {
  alert(msg);
}

const message = ref('Hello Preksha!');
</script>

<template>
  <h1>Hello, <span>{{ firstName }}</span><span v-html="lastName"></span></h1>

  <button :disabled="true">Click Me</button>

  <div v-bind="objAttribute">Hello World!</div>

  <button v-on:click="increment">Increment by {{ count }}</button>

  <p :class="classObj" :style="styleObj">This is a paragraph</p>

  <button @click="showData">Show Data</button>
  <p>{{ obj.name }} {{ obj.age }} {{ obj.city }}</p>

  <button @click="awesome = !awesome">Toggle</button>

  <h1 v-if="awesome">Vue is awesome!</h1>
  <h1 v-else>Oh no 😢</h1>

  <li v-for="(item, index) in items">
    {{ parentMessage }} - {{ index }} - {{ item.message }}
  </li>
  <br>
  <li v-for="(value, key) in obj">{{ key }}:{{ value }}</li>
  <br>
  <button @click="greet('Hello from preksha')">Greet</button><br><br>
  <button @click="greet(`Hello from ${firstName}`)">Greet</button>

  <p>Message is: {{ message }}</p>
  <input v-model="message" placeholder="edit me" />

</template>

<style scoped></style>
