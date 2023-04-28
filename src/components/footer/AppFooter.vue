<script>
import FooterTop from "./footerTop.vue";
import FooterBottom from "./FooterBottom.vue";
export default {
  name: "AppFooter",
  data() {
    return {};
  },
  components: {
    FooterTop,
    FooterBottom,
  },
};
</script>

<template>
  <FooterTop />
  <FooterBottom />
</template>

<style scoped lang="scss"></style>
