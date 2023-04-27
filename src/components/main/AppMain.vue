<script>
import SectionBusiness from "./SectionBusiness.vue";
import SectionNetwork from "./SectionNetwork.vue";
import SectionActionsProjects from "./SectionActionsProjects.vue";
export default {
  name: "AppMain",
  data() {
    return {};
  },
  components: {
    SectionBusiness,
    SectionNetwork,
    SectionActionsProjects,
  },
};
</script>

<template>
  <main>
    <SectionBusiness />
    <SectionNetwork />
    <SectionActionsProjects />
  </main>
</template>

<style scoped lang="scss"></style>
