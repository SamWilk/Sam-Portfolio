<template>
  <div class="container">
    <div class="content"></div>
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
  align-items: center;
  justify-content: center;
  width: 100vw;
  max-height: 5vh;
  min-height: 3rem;
  background: #b5e8d6;
  color: #6769e1;
  overflow: hidden;
}

@media only screen and (max-width: 800px) {
  .container {
    font-family: "Roboto", sans-serif;
    position: sticky;
    display: flex;
    flex-direction: row;
    align-items: center;
    justify-content: center;
    width: 100vw;
    max-height: 5vh;
    min-height: 3rem;
    background: #b5e8d6;
    color: #6769e1;
    overflow: hidden;
  }
}
</style>
