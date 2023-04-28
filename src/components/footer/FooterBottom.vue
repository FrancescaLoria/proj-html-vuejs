<script>
export default {
  name: "FooterBottom",

  data() {
    return {};
  },
};
</script>

<template>
  <div class="footer-bottom">
    <div class="ms_container">
      <div class="d-flex justify-content-between">
        <div class="text-left">
          Enjoy the low price. We are tracking any intention of piracy
        </div>
        <div class="text-right d-flex">
          <div>&copy;2020 NEXGEN is Proudly Powered by</div>
          <span class="ms-1">Codings</span>
        </div>
      </div>
    </div>
  </div>
</template>

<style scoped lang="scss">
.footer-bottom {
  padding: 30px 0;
  background-color: #0d0d11;
  font-size: 12px;
  color: white;

  span {
    color: #058283;
  }
}
</style>
