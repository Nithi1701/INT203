<script setup>
import { MagicString } from 'vue/compiler-sfc';

// style
  const waringColor = 'orange'
  const italicText = 'italic'
  const isError = true
  const successText = 'color:orchid'
  const warningText = 'color:orange'

  const decorText = 'text-decoration:underline'
  const isDecor = false

// class
  const isSuccceed = true
  const msg = ''
  const hasLangth = () => msg.length !==0
</script>
 
<template>
<!-- style attribute with obj syntax -->
  <!-- เคบับเคส ใส่ '' -->
  <p :style="{color:waringColor, 'font-style':italicText}">Style with obj syntax</p>
  <p :style="isError?'color:red':'color:green'">this is error message</p>
  <p :style="isError?successText:warningText">this is binding on varible</p>

<!-- style attribute with array syntax -->
  <p :style="[successText, decorText]">Style with array syntax</p>
  <p :style="[successText, isDecor?decorText:'']">with condition</p>

<!-- class attribute with obj syntax -->
  <p :class="{'success-text':hasLangth(), 'decor-text':isSuccceed}">This is class binding with obj</p>

<!-- class attribute with array syntax -->
  <p :class="['error-text', isSuccceed?'decor-text':'']">This is class binding with array</p>
</template>
 
<style>
  .success-text{
    color: olive;
  }
  .error-text{
    color: crimson;
  }
  .decor-text{
    text-decoration: line-through;
  }
</style>