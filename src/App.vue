<template>
  <img alt="Vue logo" src="./assets/logo.png">
  <!-- <HelloWorld msg="Welcome to Your Vue.js App"/> -->
  <register data="anil is here"/>
</template>

<script>
// import HelloWorld from './components/HelloWorld.vue'
import register from './components/register.vue'

import Vue from 'vue'
import { MdButton, MdContent, MdTabs } from 'vue-material/dist/components'
import 'vue-material/dist/vue-material.min.css'
import 'vue-material/dist/theme/default.css'

Vue.use(MdButton)
Vue.use(MdContent)
Vue.use(MdTabs)

export default {
  name: 'App',
  components: {
    // HelloWorld,
    register
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
