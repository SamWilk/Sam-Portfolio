<template>
  <div class="content2">
    <AboutMe name="Sam Wilk" />
    <PictureComp
      imageFile="Profile-pic.jpeg"
      height="200"
      width="200"
      msg="Sam Wilk"
      class="imgContent"
    />
    <div class="behindImg" />
  </div>
</template>

<script>
import PictureComp from "./PictureComp.vue";
import AboutMe from "./AboutMe.vue";
export default {
  name: "TopPage",
  components: {
    PictureComp,
    AboutMe,
  },
};
</script>

<style scoped>
.content2 {
  display: flex;
  flex-direction: row;
  max-height: 30vh;
  min-height: 15rem;
  min-width: 100vw;
  justify-content: flex-start;
  align-items: center;
  color: #2a3e38;
  position: relative;
}

.imgContent {
  position: absolute;
  right: 20vw;
  transform: translate(-15px, 15px);
  transition: 0.4s ease;
}

.behindImg {
  position: absolute;
  right: 20vw;
  height: 200px;
  width: 200px;
  border-radius: 12px;
  z-index: -1;
  background: #2a3e38;
}

.imgContent:hover {
  transform: translate(-25px, -10px);
}

.backSlices {
  position: fixed;
  z-index: -1;
  right: 0;
  top: 0%;
  background: #b5e8d6;
  min-width: 20rem;
  width: 60vw;
  max-width: 90vw;
  min-height: 15rem;
  height: 35vh;
  max-height: 35vh;
}

.whiteSlices {
  position: fixed;
  z-index: -1;
  left: 0;
  top: 0%;
  background: #e6fff6;
  min-width: 40rem;
  min-height: 30rem;
  height: 36vh;
  transform: rotate(-45deg);
}
</style>
