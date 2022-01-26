<script setup>
  const headingStyle = 'color:Green'
  const paraStyle = 'text-decoration:underline'
  const imgPath = '../images/BlackHayate.jpg'
</script>
 
<template>
  <h1 :style="headingStyle">Client 2</h1>
  <h2 :style="paraStyle">Lec by Nithi</h2>
  <!-- รูปตกแต่ง web ไว้ใน assets -->
  <img src="./assets/logo.png">
  <!-- รูปที่ต้องประมวลผล ไว้ใน public -->
  <img :src="imgPath">
</template>
 
<style>

</style>