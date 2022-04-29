<template>
  <img alt="Vue logo" src="./assets/logo.png" />
  <!-- <img
    alt="Sam Wilk"
    src="./assets/picture-Sam/Profile-pic.jpeg"
    height="100"
    width="100"
    class="photo"
  /> -->
  <PictureComp
    imageFile="./assets/picture-Sam/Profile-pic.jpeg"
    msg="Sam Wilk"
  />
  <HelloWorld msg="Welcome to Your Vue.js App" />
  <div>Hello There I am testing out git</div>
  <AboutMe name="Sam Wilk" />
</template>

<script>
import HelloWorld from "./components/HelloWorld.vue";
import AboutMe from "./components/AboutMe.vue";
import PictureComp from "./components/PictureComp.vue";

export default {
  name: "App",
  components: {
    HelloWorld,
    AboutMe,
    PictureComp,
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
