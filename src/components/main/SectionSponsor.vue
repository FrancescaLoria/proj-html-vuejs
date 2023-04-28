<script>
export default {
  name: "SectionSponsor",
  data() {
    return {};
  },
};
</script>

<template>
  <div class="sponsor">
    <div class="ms_container">
      <ul>
        <li>
          <img src="../../assets/images/logo-4.png" alt="" />
        </li>
        <li>
          <img src="../../assets/images/logo-5.png" alt="" />
        </li>
        <li>
          <img src="../../assets/images/logo-1.png" alt="" />
        </li>
        <li>
          <img src="../../assets/images/logo-2.png" alt="" />
        </li>
        <li>
          <img src="../../assets/images/logo-3.png" alt="" />
        </li>
        <li>
          <img src="../../assets/images/logo-4.png" alt="" />
        </li>
      </ul>
    </div>
  </div>
</template>

<style scoped lang="scss">
.sponsor {
  padding: 100px 0;
  background-color: #111117;

  ul {
    display: flex;
    align-items: center;
    gap: 80px;
    margin: 0;
    padding-left: 0;

    img {
      width: 95px;
      filter: invert(1);
    }
  }
}
</style>
