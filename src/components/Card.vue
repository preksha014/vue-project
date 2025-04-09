<template>
    <div class="card">
        <div class="card-header">
            <slot name="header">Default Header</slot>
        </div>
        <div class="card-body">
            <slot>Default Body</slot>
        </div>
        <div class="card-footer">
            <slot name="footer">Default Footer</slot>
        </div> 
    </div>
</template>

<script setup>

</script>

<style scoped>
.card {
    border: 1px solid #ccc;
    border-radius: 8px;
    box-shadow: 0 2px 4px rgba(0, 0, 0, 0.1);
    padding: 16px;
    margin: 16px;
    background-color: #fff;
}
.card-header {
    font-size: 1.5em;
    margin-bottom: 16px;
}
.card-body {
    font-size: 1em;
    margin-bottom: 16px;
}
.card-footer {
    font-size: 0.9em;
    text-align: right;
    color: #666;
}
</style>