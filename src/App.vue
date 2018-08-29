<template>
  <div id="app">
    <img alt="Vue logo" src="./assets/logo.png">
    <HelloWorld msg="Hello World! I'm a component!"/>
    <h1>When a style tag has the scoped attribute,</h1>
    <h1>its CSS will apply to elements of the current component only.</h1>
  </div>
</template>

<script lang="ts">
import { Component, Vue } from "vue-property-decorator";
import HelloWorld from "./components/HelloWorld.vue";

@Component({
  components: {
    HelloWorld
  }
})
export default class App extends Vue {}
</script>

<style>
#app {
  text-align: center;
  margin-top: 60px;
  font-family: "Courier New", Courier, monospace;
}
</style>
