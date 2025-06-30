<script setup>

defineProps(['message', 'Heading'])
</script>

<template>
<div class="cc">
    <h1>{{ Heading }}</h1>

    <p>{{ message }}</p>
</div>

</template>

<style scoped>
.cc {
    background-color: #f0f0f0;
    padding: 20px;
    border-radius: 8px;
    box-shadow: 0 2px 4px rgba(0, 0, 0, 0.1);
}

</style>