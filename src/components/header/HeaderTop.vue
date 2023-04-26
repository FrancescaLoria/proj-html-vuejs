<script>
export default {
  name: "HeaderTop",
  data() {
    return {};
  },
};
</script>

<template>
  <header class="header-top">
    <div class="ms_container py-2 d-flex justify-content-between">
      <div class="timetables d-flex align-items-center">
        <i class="fa-solid fa-clock mx-1"></i>
        <div>Open Hours: Mon-Sat-9:00-18:00</div>
      </div>
      <div class="contacts d-flex">
        <div class="d-flex align-items-center mx-2">
          <i class="fa-solid fa-phone mx-1"></i>
          <div>+1 (305) 1234-5678</div>
        </div>
        <div class="d-flex align-items-center mx-3">
          <i class="fa-solid fa-envelope mx-1"></i>
          <div>hello@example.com</div>
        </div>
        <div class="mx-3">
          <i class="fa-brands fa-facebook-f"></i>
          <i class="fa-brands fa-twitter mx-4"></i>
          <i class="fa-brands fa-linkedin-in"></i>
        </div>
      </div>
    </div>
  </header>
</template>

<style scoped lang="scss">
.header-top {
  background-color: #21333e;

  .timetables,
  .contacts {
    color: white;
    font-size: 9px;
  }
}
</style>
