<template>
  <img alt="Vue logo" src="./assets/logo.png" />
  <HelloWorld msg="texto pasado por param">
    <template v-slot:header>
      <h1>Header de la página</h1>
    </template>

    <p>Contenido de la página</p>

    <template v-slot:footer>
      <p>Footer de la página</p>
    </template>
  </HelloWorld>
</template>

<script>
import HelloWorld from "./components/HelloWorld.vue";

export default {
  name: "App",
  components: {
    HelloWorld,
  },
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
