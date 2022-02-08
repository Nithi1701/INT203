<script setup>
  import { ref } from 'vue';
  const suggestion = ref('')
  const favorColor = ref('')
  const agree = ref(false)
  const jobs = ref([])
  const food = ref('')
  const activities = ref([])
</script>
 
<template>
<!-- textarea -->
  <div>
    suggestion
    <textarea 
      v-model = "suggestion"
      cols="30"
      rows="10"
      placeholder="type ypur suggestion here"
    ></textarea>
    <p>{{ suggestion }}</p>
  </div>

<!-- redio -->
  <div>
    <input type="radio" value="RED" v-model = "favorColor">
    <label>Red</label>
    <input type="radio" value="GREEN" v-model = "favorColor">
    <label>Green</label>
    <p>{{ favorColor }}</p>
  </div>

<!-- check box(single) -->
  <div>
    <input type="checkbox" v-model = "agree">
    <label>I agree</label>
    <p>{{ agree }}</p>
  </div>

<!-- check box(muli) -->
  <div>
    <input type="checkbox" value="FRONTEND" v-model = "jobs">
    <label>frontend</label>
    <input type="checkbox" value="BACKEND" v-model = "jobs">
    <label>backend</label>
    <input type="checkbox" value="DEVOPS" v-model = "jobs">
    <label>devops</label>
    <p>{{ jobs }}</p>
  </div>

<!-- select(single) -->
  <div>
    menu:
    <select v-model = "food">
      <option value="PIZZA"></option>
      <option value="SOUP"></option>
      <option value="WATER"></option>
    </select>
    <p>{{ food }}</p>
  </div>
<!-- select(muli) -->
  <div>
    activities:
    <select v-model = "activities" multiple>
      <option value="play"></option>
      <option value="sleep"></option>
      <option value="eat"></option>
    </select>
    <p>{{ activities }}</p>
  </div>
</template>
 
<style>

</style>