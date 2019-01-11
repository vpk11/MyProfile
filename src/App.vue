<template>
  <div id="app">
    <img width="25%" src="./assets/logo.png" /> <MainProfile />
  </div>
</template>

<script>
import MainProfile from "./components/MainProfile";

export default {
  name: "App",
  components: {
    MainProfile
  }
};
</script>

<style>
#app {
  font-family: "Avenir", Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
