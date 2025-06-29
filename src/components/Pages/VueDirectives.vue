<script setup >
import { ref } from 'vue'
import { workoutProgram } from '../../utils'; //Here we are mainly using a json type of js file which is the primary source of data in the codebase, As we previously imported in react we are importing it in VueJS as the same process
const name = ref('')
// This is a Vue 3 component using the Composition API
const number =  80;
const items = [
    { id: 1, name: 'Item 1' },
    { id: 2, name: 'Item 2' },
    { id: 3, name: 'Item 3' }
]
const proflink = "https://www.facebook.com/profile.php?id=100049732306068";

function getText() {
    console.log("Hello from getText");
}

const Arrowfuc = () => {
    console.log("Hello from Arrowfunction");
    document.getElementsByClassName("hi")[0].innerHTML = "This is changed by Arrow Function";
}

console.log(workoutProgram)

</script>

<template>

<!-- THIS IS THE CONCEPT O INITIA V-IF AND V-ELSE -->
<div class="vdirs">
    <div class="classes">
        <h5 class="hi">This is Changing......</h5>
    </div>
    <p v-if="number == 90"> Woah You got awesome grades</p>
   
    <p v-else> You suck</p>

    <li v-for="i in items" :key="i.id">
        <h2> This part has the key implementation {{ i.name }} </h2>
    </li>

    <a v-bind:href ="proflink" target="_blank">Click</a>

    <button @mouseover="getText">Press</button>
    <button @click="Arrowfuc">Click</button>

    <input v-model="name" type="text" placeholder="Enter your name">
    <p class="testname">Your name is {{ name }}</p>
    <h4>Here is the cahnge I want to push it on github
        
    </h4>
</div>
    
</template> 

<style scoped>

</style>
