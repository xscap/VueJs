<script setup>
import { ref } from 'vue';
const show = ref(false);
</script>

<template>
    <div>
        <button @click="show = true">Open Modal</button>
    <teleport to="body">
      <div v-if="show" class="modal">
        <p>This is a self explanatory modal </p>
        <button @click="show = false">Close</button>
      </div>
    </teleport>
    </div>
</template>

<style scoped>

.modal {
    position: fixed;
    top: 50%;
    left: 50%;
    transform: translate(-50%, -50%);
    background-color: green;
    padding: 20px;
    border: 1px solid yellow;
    z-index: 1000;
}
</style>