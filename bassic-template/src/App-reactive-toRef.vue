<script setup>
    import { reactive, toRef, toRefs } from 'vue';
    const student = reactive({sId: 1234, sName: 'Nithi'})
    console.log(student)
    console.log(student.sId)
    const item = reactive(['pepsi', 'coke', 'est', 'A&W'])
    console.log(item)
    console.log(item[3])

// reactive to ref
    const product = reactive({
        proId: 1001,
        proName: 'A&W',
        proPrice: 20,
        proDesc: 'for drinking'
    })
    const price = toRef(product, 'proPrice')
    console.log(price.value)
    price.value += 10
    console.log(product)
    const { proId, proDesc } = toRefs(product)
    console.log(proId.value)
    console.log(proDesc.value)
</script>
 
<template>
    <p>student: {{ student }}</p>
    <p>student id: {{ student.sId }}</p>
    <p>all Item: {{ item }}</p>
    <p>product: {{ product }}</p>
    <p>proId & proDesc: {{ proId }} {{ proDesc }}</p>
</template>
 
<style>

</style>