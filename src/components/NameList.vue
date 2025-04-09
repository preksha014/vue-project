<template>
    <div>
        <h1>Name List</h1>
        <ul>
            <li v-for="name in names" :key="name.id">
                <slot v-bind="name"></slot>
                <!-- <slot :name="name.name" :id="name.id"></slot> -->
            </li>
        </ul>
    </div>
</template>

<script setup>

const names=[
    { id: 1, name: 'John Doe' },
    { id: 2, name: 'Jane Smith' },
    { id: 3, name: 'Alice Johnson' },
    { id: 4, name: 'Bob Brown' },
    { id: 5, name: 'Charlie Davis' },
];

</script>

<style scoped>

</style>