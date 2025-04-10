<template>
    <form @submit.prevent="createPost">
    <div>
        <label for="title">Title</label>
        <input type="text" v-model="formData.title" placeholder="Title" />
    </div>
    <div>
        <label for="body">Body</label>
        <input type="text" v-model="formData.body" placeholder="Body" />
    </div>
    <div>
        <label for="userId">User ID</label>
        <input type="text" v-model="formData.userId" placeholder="User ID" />
    </div>
    <button>
        Create Post
    </button>
    </form>
</template>

<script setup>
import {ref} from 'vue'
import axios from 'axios'
const formData=ref({
    title: '',
    body: '',
    userId: ''
})

function createPost(){
    axios.post('https://jsonplaceholder.typicode.com/posts', formData.value)
        .then(response => {
            console.log('Post created:', response.data);
            // Optionally, reset the form or handle success
            // formData.value = { title: '', body: '', userId: '' };
        })
        .catch(error => {
            console.error('Error creating post:', error);
            // Optionally, handle error
        });
}
</script>

<style scoped>

</style>