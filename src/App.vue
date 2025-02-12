<template>
  <img alt="Vue logo" src="./assets/logo.png">
  <UsandoProps />
 
</template>

<script>

import UsandoProps from './components/UsandoProps.vue';


export default {
  name: 'App',
  components: {
    UsandoProps,
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

ul, li{
  list-style-type: none;
  align-items: center;
  text-align: center;
}
</style>
