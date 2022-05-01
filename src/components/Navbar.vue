<template>
  <div class="container">
    <div class="content">NavBar Here</div>
  </div>
</template>

<script>
export default {
  name: "NavBar",
  data() {
    return {
      flag: false,
    };
  },
  mounted() {
    console.log("Nav mounted");
  },
  methods: {
    updateFlag() {
      this.flag = this.flag === false ? true : false;
      return console.log("flag", this.flag) || this.flag;
    },
  },
};
</script>

<style scoped>
.container {
  font-family: "Roboto", sans-serif;
  position: sticky;
  top: 0%;
  display: flex;
  flex-direction: row;
  width: 100vw;
  max-height: 5vh;
  min-height: 5vh;
  background: #2a3e38;
  color: #6769e1;
  overflow: hidden;
}

@media only screen and (max-width: 800px) {
  .container {
    font-family: "Roboto", sans-serif;
    display: flex;
    flex-direction: row;
    width: 100vw;
    max-height: 5vh;
    min-height: 5vh;
    background: black;
    color: #6769e1;
    overflow: hidden;
  }
}
</style>
