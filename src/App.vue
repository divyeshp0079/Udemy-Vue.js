<template>
  <img alt="Vue logo" src="./assets/logo.png" />
  <first_app />
</template>

<script>
import first_app from "./components/First_Vue_app.vue";
export default {
  name: "App",
  components: {
    first_app,
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
