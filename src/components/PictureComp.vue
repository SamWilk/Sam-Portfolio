<template>
  <img alt="" :src="getImgSrc()" width="100" height="100" class="myPic" />
</template>

<script>
export default {
  name: "PictureComp",
  props: {
    msg: String,
    imageFile: String,
  },
  methods: {
    getImgSrc() {
      return console.log("Image", this.imageFile) || this.imageFile;
    },
  },
};
</script>

<style scoped>
.myPic {
  border-radius: 12px;
}
</style>
