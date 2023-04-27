<script>
export default {
  name: "CardListFooter",
  props: {
    list: Array,
  },
  data() {
    return {};
  },
};
</script>

<template>
  <div class="ms_card">
    <ul>
      <li v-for="(link, index) in list" :key="index">
        <span v-if="index === 0" class="title-card">{{ link }}</span>
        <span v-else class="element d-flex align-items-center mt-3">
          <i class="fa-solid fa-chevron-right"></i>
          <div class="ms-3">{{ link }}</div>
        </span>
      </li>
      <!-- <li class="title-card">About</li>
      <li class="element d-flex align-items-center mt-3">
        <i class="fa-solid fa-chevron-right"></i>
        <div class="ms-3">Lorem</div>
      </li>
      <li class="element d-flex align-items-center mt-3">
        <i class="fa-solid fa-chevron-right"></i>
        <div class="ms-3">Lorem</div>
      </li>
      <li class="element d-flex align-items-center mt-3">
        <i class="fa-solid fa-chevron-right"></i>
        <div class="ms-3">Lorem</div>
      </li>
      <li class="element d-flex align-items-center mt-3">
        <i class="fa-solid fa-chevron-right"></i>
        <div class="ms-3">Lorem</div>
      </li>
      <li class="element d-flex align-items-center mt-3">
        <i class="fa-solid fa-chevron-right"></i>
        <div class="ms-3">Lorem</div>
      </li> -->
    </ul>
  </div>
</template>

<style scoped lang="scss">
.ms_card {
  background-color: #1f1f26;
  padding: 20px;
  width: 25%;
  margin: 0 20px;
  text-align: center;
  border-radius: 10px;

  ul {
    margin: 0;
    padding-left: 0;

    .title-card {
      font-weight: 800;
      font-size: 18px;
    }

    .element {
      font-size: 12px;
      justify-content: center;
    }
  }
}
</style>
