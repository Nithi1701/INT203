<script setup>
  const headingStyle = 'color:Green'
  const paraStyle = 'text-decoration:underline'
  const imgPath = '../public/favicon.ico'
</script>
 
<template>
  <h1 :style="headingStyle">Client 2</h1>
  <h2 :style="paraStyle">Lec by Nithi</h2>
  <!-- รูปตกแต่งไว้ใน assets -->
  <img src="./assets/logo.png">
  <img :src="imgPath">
</template>
 
<style>

</style>