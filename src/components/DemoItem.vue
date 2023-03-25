<template>
    <button v-on:click="increase">点我数字增加</button>
    <h1 class="color">{{number}}</h1>
</template>

<!-- <script setup>
import { ref } from 'vue';

let number=ref(0);
const increase = ()=>{
    number.value++;
};
</script> -->

<script>
import { ref } from 'vue';

export default{
    setup(){
        let number= ref(0);
        const increase = ()=>{
            number.value++;
        }
        return{
            number,
            increase
        }
    }
  
}
</script>

<style scoped>
.color{
    color: red;
}
</style>