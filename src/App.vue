<template>
  <main class="container">
    <!-- <PictureComp
      imageFile="Profile-pic.jpeg"
      msg="Sam Wilk"
      height="200"
      width="200" -->
    <!-- /> -->
    <!-- <AboutMe name="Sam Wilk" /> -->
    <Navbar />
    <div class="content">Content Here</div>
  </main>
</template>

<script>
// import AboutMe from "./components/AboutMe.vue";
import Navbar from "./components/Navbar.vue";

export default {
  name: "App",
  components: {
    // AboutMe,
    Navbar,
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

.container {
  position: fixed;
  z-index: 2;
  display: flex;
  flex-direction: column;
  width: 100vw;
  max-height: 100vh;
  min-height: 100vh;
  justify-content: flex-start;
  align-items: center;
  background: #e6fff6;
  overflow-y: scroll;
  overflow-x: hidden;
}

@media only screen and (max-width: 800px) {
  .container {
    position: fixed;
    z-index: 2;
    display: flex;
    flex-direction: column-reverse;
    width: 100vw;
    max-height: 100vh;
    justify-content: flex-start;
    align-items: center;
    backdrop-filter: blur(10px);
    background: transparent;
    overflow-y: scroll;
    overflow-x: hidden;
  }
}

.paragraph {
  display: flex;
  flex-wrap: wrap;
  word-break: break-all;
  max-width: 40vw;
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
