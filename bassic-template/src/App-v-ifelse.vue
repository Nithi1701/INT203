<script setup>
  const depositAmt = 20000
  const interest = 0.1
  const d2 = 50000
</script>
 
<template>
  <p>Deposit amount: {{ depositAmt }}</p>
  <p v-if="depositAmt>=10000">Interest: {{ depositAmt*interest }}</p>
  <p v-else>Interest: 0</p>
  <p>-----------------------------------</p>
  <p>Deposit amount2: {{ d2 }}</p>
  <p v-if="d2 < 10000">Interest: {{ d2 }}</p>
  <p v-else-if="d2<=49999">Interest: {{ d2*0.1 }}</p>
  <p v-else-if="d2<=99999">Interest: {{ d2*0.2 }}</p>
  <p v-else>Interest: {{ d2*0.25 }}</p>

</template>
 
<style>

</style>