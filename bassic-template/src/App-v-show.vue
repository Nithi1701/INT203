<script setup>
  const isSearch = true
  const yourName = "Nithi"
</script>
 
<template>
  <dev v-show="isSearch">
    <label for="search">search</label>
    <input type="text" id="search" class="border">
  </dev>
  <p v-show="yourName">Hello,{{ yourName }}</p>
</template>
 
<style>

</style>