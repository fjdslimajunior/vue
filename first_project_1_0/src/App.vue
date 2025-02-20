<template>
  <TheHeader 
    v-show="showHeader"
  />



  <img alt="Vue logo" src="./assets/logo.png">
  <TheMain 
  v-show="showMain"
  />
  <HelloWorld msg="Welcome to Your Vue.js App"/>
  <TheFooter 
  v-show="showFooter"
  />
</template>

<script>
import HelloWorld from './components/HelloWorld.vue'
import TheFooter from './components/TheFooter.vue';
import TheHeader from './components/TheHeader.vue';
import TheMain from './components/TheMain.vue';

export default {
  name: 'App',
  components: {
    HelloWorld, 
    TheHeader,
    TheMain,
    TheFooter
  },
  data() {
    return{
      showHeader: false,
      showMain: false,
      showFooter: false
    }
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
