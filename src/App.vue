<template>
  <img alt="Vue logo" src="./assets/logo.png" />
  <HelloWorld msg="Welcome to Your Vue.js App" />
  <div>Hello There I am testing out git</div>
  <AboutMe name="Sam Wilk" />
</template>

<script>
import HelloWorld from "./components/HelloWorld.vue";
import AboutMe from "./components/AboutMe.vue";

export default {
  name: "App",
  components: {
    HelloWorld,
    AboutMe,
  },
};
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  font-family: "Roboto", sans-serif;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
