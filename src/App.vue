<script setup>
import HelloWorld from './components/Pages/HelloWorld.vue'
import SamplePage from './components/Pages/SamplePage.vue'
import Layout from './components/Layout/layout.vue'
import VueDirectives from './components/Pages/VueDirectives.vue'
import TeleportDir from './components/Pages/TeleportDir.vue'
</script>

<template>

  
  <Layout>
  <TeleportDir/>
  <HelloWorld/>
  <SamplePage/>
  <VueDirectives/>
  
  </Layout>
  
</template>

<style scoped>
/* h1{
  color: blue;
} */

</style>
