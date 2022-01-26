<script setup>
// text
  const msg = "Hello, Vue.js"
  const counter = 1
// html
const paraStyle = '<i><b>INT203 Web Client 2</b></i>'
</script>
 
<template>
<!-- text -->
  <h1>{{ msg.toLowerCase() }}</h1>
  <h1>{{ counter += 10 }}</h1>
  <!-- html -->
  <h3 v-html="paraStyle"></h3>
</template>
 
<style>

</style>