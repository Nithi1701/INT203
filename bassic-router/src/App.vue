<script setup>
import { ref } from 'vue';
// dimamic img
    // const UnknowImg = ref('images/BlackHayate.jpg')
</script>
 
<template>
    <div>
        <!-- <img :src="UnknowImg"> -->
        <div>
            <router-link :to="{name: 'Home'}">Home</router-link>
            <router-link :to="{name: 'MyPortfolio'}">My Portfolio</router-link>
        </div>
        <div>
            <router-view></router-view>
        </div>
        
    </div>
</template>
 
<style>
    a{
        color: sienna;
    }
    .router-link-active{
        color: tomato;
    }
</style>