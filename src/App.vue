<template>
  <img alt="Vue logo" src="./assets/logo.png">
  <HelloWorld msg="Welcome to Your Vue.js App"/>
  <a-button @click="onClick">点击次数：{{ count }}</a-button>
</template>
<script setup>
  import { ref } from 'vue';
  import HelloWorld from './components/HelloWorld.vue'

  const count = ref(0);
  const onClick = () => {
    count.value ++;
  };
</script>

<style>
  #app {
    font-family: Avenir, Helvetica, Arial, sans-serif;
    -webkit-font-smoothing: antialiased;
    -moz-osx-font-smoothing: grayscale;
    text-align: center;
    color: #2c3e50;
    margin-top: 60px;
  }
</style>
