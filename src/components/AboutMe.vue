<template>
  <div class="containerAbout">
    <h3>
      My Name is <label>{{ name }}</label>
    </h3>
    <h5>I am a <label>Full Stack Developer</label></h5>
  </div>
</template>

<script>
export default {
  name: "AboutMe",
  props: {
    name: String,
  },
};
</script>

<style scoped>
label {
  color: #6769e1;
}
.containerAbout {
  display: flex;
  flex-direction: column;
  min-width: 100vw;
  justify-content: space-evenly;
}
</style>
