<template>
  <img alt="Vue logo" src="./assets/logo.png">
  <!-- <HelloWorld msg="Welcome to Your Vue.js App"/> -->
  <!-- <HomeLayout /> -->
  <HomeLayout data="vishnu is here" msg="hi from vishnu" />
</template>

<script>

import HomeLayout from './components/HomeLayout.vue'
export default {
  name: 'App',
  components: {
    
    HomeLayout
  }
}
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
