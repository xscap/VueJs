<script setup>
import ChildComponent from './ChildComponent.vue';
</script>

<template>

<div>
    <ChildComponent Heading = "Hi This the main Heading"/>
<ChildComponent message="This is a message passed from the parent component." />
    <ChildComponent Heading = "This is another Heading" message="This is another message passed from the parent component." />
    <ChildComponent Heading = "This is the last Heading" message="This is the last message passed from the parent component." />
</div>

</template>

<style scoped>

</style>
