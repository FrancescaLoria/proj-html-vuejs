<script>
import SectionBusiness from "./SectionBusiness.vue";
import SectionNetwork from "./SectionNetwork.vue";
export default {
  name: "AppMain",
  data() {
    return {};
  },
  components: {
    SectionBusiness,
    SectionNetwork,
  },
};
</script>

<template>
  <main>
    <SectionBusiness />
    <SectionNetwork />
  </main>
</template>

<style scoped lang="scss"></style>
