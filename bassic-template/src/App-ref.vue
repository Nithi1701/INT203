<script setup>
    import { ref } from 'vue';
    const hasError = ref(false)
    console.log(hasError.value)
// แก้ไขค่า
    hasError.value != hasError.value
    console.log(hasError.value)

// obj
    const student = ref({sId: 1234, sName: 'Nithi'})
    console.log(student.value)
    console.log(student.value.sName)

// array
    const id = ref([11, 12, 23, 44, 50, 56])
    console.log(id.value)
    console.log(id.value[2])
    const ids = id.value.filter((id) => id > 20)
    console.log(ids)
</script>
 
<template>
    <p>hasError: {{ hasError }}</p>
    <p>student: {{ student }}</p>
    <p>student id: {{ student.sId }}</p>
    <p>id: {{ id }}</p>
    <p>filter id: {{ ids }}</p>
</template>
 
<style>

</style>