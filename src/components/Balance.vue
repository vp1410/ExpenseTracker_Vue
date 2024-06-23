<template>
    <h4>Your Balance</h4>

     <!-- Original logic -->
    <h1 id="balance">${{total.toFixed(2)}}</h1>

    <!-- Optional logic -->
    <!-- <h1 id="balance">${{formattedTotal}}</h1> -->
</template>

<script setup>
import {defineProps, computed}  from 'vue';

const props =  defineProps({

    total:{
        type: Number,
        required:true
    }
})

// Optional: To have total amount only upto 2 decimal places 
// const formattedTotal = computed(() => {
//     // Convert total to a string with 2 decimal places
//     return props.total.toFixed(2);
// });
</script>