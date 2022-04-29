<template>
  <main class="AboutMe">
    <PictureComp
      imageFile="Profile-pic.jpeg"
      msg="Sam Wilk"
      height="200"
      width="200"
    />
    <AboutMe name="Sam Wilk" />
  </main>
</template>

<script>
import AboutMe from "./components/AboutMe.vue";
import PictureComp from "./components/PictureComp.vue";

export default {
  name: "App",
  components: {
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

.AboutMe {
  display: flex;
  flex-direction: row;
  margin: auto;
  width: 50vw;
  justify-content: space-evenly;
  align-items: center;
}
</style>
