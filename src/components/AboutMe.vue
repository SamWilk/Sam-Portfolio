<template>
  <div>This component is about {{ name }}</div>
</template>

<script>
export default {
  name: "AboutMe",
  props: {
    name: String,
  },
};
</script>
