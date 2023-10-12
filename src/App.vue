<script lang="ts" setup>
import{ref, type Ref} from 'vue'
const name:string="vars reactives";
let counter:Ref<number>=ref(0);
const increment = ()=>{
  counter.value++;
  console.log(counter);
  
};

const decrement = ()=>{
  counter.value--;
  console.log(counter);
  
};

const reset = ()=>{
  counter.value=0

};
</script>
<template>
  <h1>Hola {{ name }}</h1>
  <h2>{{ counter }}</h2>
  <button @click="increment">Botó increment</button>
  <button @click="decrement">Botón decremento</button>
  <button @click="reset">Reset</button>
</template>


