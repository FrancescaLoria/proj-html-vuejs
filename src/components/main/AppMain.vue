<script>
import SectionBusiness from "./SectionBusiness.vue";
import SectionNetwork from "./SectionNetwork.vue";
import SectionActionsProjects from "./SectionActionsProjects.vue";
import ResultNumbers from "./ResultNumbers.vue";
import SectionSponsor from "./SectionSponsor.vue";
export default {
  name: "AppMain",
  data() {
    return {};
  },
  components: {
    SectionBusiness,
    SectionNetwork,
    SectionActionsProjects,
    ResultNumbers,
    SectionSponsor,
  },
};
</script>

<template>
  <main>
    <SectionBusiness />
    <SectionNetwork />
    <SectionActionsProjects />
    <ResultNumbers />
    <SectionSponsor />
  </main>
</template>

<style scoped lang="scss"></style>
