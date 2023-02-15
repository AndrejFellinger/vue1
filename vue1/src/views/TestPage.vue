<script setup lang="ts">
import { h } from 'vue';



let value = 1

const handleClick = () =>{
  value +=  1;
  console.log(value)
}

const testFunction = () =>{
  alert("test1")
  
}
</script>

<template>
  <main>
    <h2>This is test page!</h2>
    <button @click="handleClick">Say hello</button>
    <button class="testhover" @mouseover="testFunction">Hover me</button>

    <p>{{ value }}</p>
    <v-if>
      {{ value == 1 }}
        <h1>Value sa rovna 1</h1>
    </v-if>

  </main>
</template>
