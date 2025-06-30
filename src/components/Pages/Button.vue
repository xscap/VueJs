<script setup>

function handleClick() {
    console.log("Button clicked!");
    const textElement = document.querySelector('.cbtn').textContent = "Texting Works are done here properly";
}

</script>

<template>
<div>
    <button @click="handleClick">
        Click to use the componrnt
    </button>
    <h2 class="cbtn">this text is working properly</h2>
</div>
</template>

<style scoped>

</style>