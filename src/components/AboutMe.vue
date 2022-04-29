<template>
  <div>This component is about {{ name }}</div>
  <div>This is where I need to add a picture of me!</div>
</template>

<script>
export default {
  name: "AboutMe",
  props: {
    name: String,
  },
};
</script>
