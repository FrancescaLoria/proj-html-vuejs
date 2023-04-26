<script>
export default {
  name: "MyButton",
  props: {
    text: String,
    variant: String,
  },

  data() {
    return {};
  },
};
</script>

<template>
  <button type="button" :class="`btn ${variant}`">{{ text }}</button>
</template>

<style scoped lang="scss">
.blue {
  background-color: #058283;
  color: white;
  font-size: 13px;
}

.trasparent {
  border: 1px solid #058283;
  color: black;
  font-size: 13px;
}
</style>
