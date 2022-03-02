<script setup>
// custom event
defineEmits(['likeMe'])
const prop = defineProps({
  buttonName: {
    type: String,
    require: true
    // default: 'OK'
  },
  props2: {}
})
// console.log(prop.buttonName)
</script>

<template>
  <button class="button-color" @click="$emit('likeMe', false, 404, 'FAIL')">{{ buttonName }}</button>
</template>

<style scoped>
.button-color {
  background-color: cornflowerblue;
  color: azure;
}
</style>