<script setup>
    import { ref } from 'vue';
    console.clear()
    const base = ref(4)
    const height = ref(8)
    let result = ref(0)
    const computeArea = () => (result.value = (1/2)*base.value*height.value)
</script>
 
<template>
    <p>Base: {{ base }}</p>
    <button @click="base++">Add 1 to base</button>

    <p>Height: {{ height }}</p>
    <button @click="height++">Add 1 to height</button>

    <p>Area Result: {{ result }}</p>
    <button @click="computeArea">Comput Area</button>
</template>
 
<style>

</style>    