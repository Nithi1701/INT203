<script setup>
    import { computed, ref } from 'vue';
    const num1 = ref()
    const num2 = ref()
    const sum = ref()
    const calculate = () => {
        sum.value = num1.value + num2.value
    }
    // const calculate = computed(() => num1.value + num2.value)

    const numbers = [1, 2, 3, 4, 5, 6, 7, 8, 9]
</script>
 
<template>
    <div>
        <input type="num" v-model="num1"> <br> 
        <input type="num" v-model="num2"> <br>
        <button @click="calculate">Calculate</button> <br>
        <span v-show="sum != 0">{{ sum }}</span>
        <!-- <span>{{ calculate }}</span> -->
    </div>

    <div>
        <ul>
            <li v-for="(number, index) in numbers" :key="index">
                {{ index+'-'+number }}
            </li>
        </ul>
    </div>
</template>
 
<style>

</style>    