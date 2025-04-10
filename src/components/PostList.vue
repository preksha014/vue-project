<template>
    <div>
        <button @click="getPosts">Fetch Posts</button>
        <ul v-if="posts.length > 0">
            <li v-for="post in posts" :key="post.id">
                <h2>{{ post.title }}</h2>
                <p>{{ post.body }}</p>
            </li>
        </ul>
    </div>
</template>

<script setup>
import { ref } from 'vue'
import axios from 'axios';
// import { onMounted } from 'vue';

// onMounted(() => {
//     getPosts();
// });
const posts=ref([]);

function getPosts(){
    axios('https://jsonplaceholder.typicode.com/posts')
        .then(response => {
            posts.value = response.data;
        })
        .catch(error => console.error('Error fetching posts:', error));
}
</script>

<style scoped>

</style>