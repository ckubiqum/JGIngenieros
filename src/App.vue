<template>
  <div id="app">
    <Header />
    <HelloJgingenieros />
  </div>
</template>

<script>
import Header from "./components/Header.vue";
import HelloJgingenieros from "./components/HelloJgingenieros.vue";

export default {
  name: "App",
  components: {
    Header,
    HelloJgingenieros
  }
};
</script>

<style>
* {
   margin: 0px;
}
#app {
  font-family: Montserrat, Arial, Helvetica, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #ffffff;
  top: 0px !important;
  width: 100vw !important;
}
</style>
