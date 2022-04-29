<template>
  <img
    :alt="getMsg()"
    :src="require(`@/assets/${imageFile}`)"
    :width="getWidth()"
    :height="getHeight()"
    class="myPic"
  />
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
  border-radius: 12px;
}
</style>
