<template>
  <div class="containerImg">
    <img
      :alt="getMsg()"
      :src="require(`@/assets/${imageFile}`)"
      :width="getWidth()"
      :height="getHeight()"
      class="myPic"
    />
    <!-- <div class="backImg" /> -->
  </div>
</template>

<script>
export default {
  name: "PictureComp",
  props: {
    msg: String,
    imageFile: String,
    height: String,
    width: String,
  },
  methods: {
    getImgSrc() {
      return console.log("Image", this.imageFile) || this.imageFile;
    },
    getMsg() {
      return console.log("Msg: ", this.msg) || this.msg;
    },
    getHeight() {
      return console.log("Height: ", this.height) || this.height;
    },
    getWidth() {
      return console.log("Height: ", this.height) || this.width;
    },
  },
};
</script>

<style scoped>
.myPic {
  /* position: absolute; */
  border-radius: 12px;
  /* z-index: 2;
  transform: translate(-15px, 15px);
  transition: ease 0.4s; */
}
</style>
