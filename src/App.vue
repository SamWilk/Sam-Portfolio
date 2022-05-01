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
  <div class="blur">
    <div class="blur1" />
    <div class="blur2" />
    <div class="blur3" />
  </div>
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
  margin: -0.5rem;
  background: #e6fff6;
  height: 100vh;
  widows: 100vw;
}

.AboutMe {
  position: fixed;
  z-index: 2;
  display: flex;
  flex-direction: row;
  width: 100vw;
  height: 100vh;
  justify-content: space-evenly;
  align-items: flex-start;
  backdrop-filter: blur(10px);
  background: transparent;
}

.blur {
  position: fixed;
  left: 30%;
  top: 20%;
  height: 40rem;
  width: 40rem;
  border-radius: 20px;
  background: transparent;
  animation-name: blockSpin;
  animation-duration: 50s;
  animation-iteration-count: 5;
}

@keyframes blockSpin {
  to {
    transform: rotate(360deg);
  }
}
@keyframes counterSpin {
  to {
    transform: rotate(-360deg);
  }
}

.blur1 {
  width: 40rem;
  height: 40rem;
  background: #2a3e38;
  border-radius: 12px;
  position: relative;
  top: -2rem;
  left: -2rem;
  animation-name: blockSpin;
  animation-duration: 90s;
  animation-iteration-count: 5;
}

.blur2 {
  width: 20rem;
  height: 20rem;
  background: #6769e1;
  border-radius: 12px;
  position: fixed;
  bottom: -2rem;
  left: -2rem;
  animation-name: counterSpin;
  animation-duration: 70s;
  animation-iteration-count: 5;
}

.blur3 {
  width: 30rem;
  height: 30rem;
  background: #b5e8d6;
  border-radius: 12px;
  position: fixed;
  bottom: -10rem;
  right: -5rem;
  animation-name: blockSpin;
  animation-duration: 100s;
  animation-iteration-count: 5;
}
</style>
