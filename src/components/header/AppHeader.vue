<script>
import HeaderTop from "./HeaderTop.vue";
import Jambotron from "./Jambotron.vue";
export default {
  name: "AppHeader",
  data() {
    return {};
  },
  components: {
    HeaderTop,
    Jambotron,
  },
};
</script>

<template>
  <HeaderTop />
  <Jambotron />
</template>

<style scoped lang="scss"></style>
