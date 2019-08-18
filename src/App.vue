<template>
  <div id="app">
    <img alt="Vue logo" src="./assets/logo.png">
    <HelloWorld msg="Welcome to Your Vue.js App"/>
    <Smt msg="awesome"/>
  </div>
</template>

<script>
import HelloWorld from './components/HelloWorld.vue'
import Smt from './components/Smt.vue'
import { store } from "./store/store";

export default {
  name: 'app',
  store,
  components: {
    HelloWorld,
    Smt
  }
}
</script>

<style>
@import "./assets/style.css";
</style>
