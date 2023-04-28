<script>
import MyButton from "../commons/MyButton.vue";
import CardBusiness from "./CardBusiness.vue";
export default {
  name: "SectionBusiness",

  data() {
    return {};
  },
  components: {
    MyButton,
    CardBusiness,
  },
};
</script>

<template>
  <div class="business">
    <div class="ms_container">
      <div class="areas mb-3">OUR BUSINESS ARES</div>
      <div class="d-flex">
        <div class="title">Excellence in</div>
        <div class="team">Services</div>
      </div>
      <div class="mt-3 d-flex justify-content-between">
        <p>
          We are leaders in providing consultacy services with a set of
          cutting-edge technologies and a team of experienced and renowned
          professional. These are some option that you can hire
        </p>
        <div>
          <MyButton :text="'SEE ALL'" :variant="'blue'" class="ms-2" />
        </div>
      </div>
      <div class="row">
        <CardBusiness />
      </div>
      <div class="divider d-flex">
        <div>
          <img src="../../assets/images/bullets.png" alt="" />
        </div>
        <div>
          <img src="../../assets/images/bullets.png" alt="" />
        </div>
      </div>
    </div>
  </div>
</template>

<style scoped lang="scss">
.business {
  padding: 100px 0;
  background-color: #eef4ed;
  position: relative;
  .areas {
    color: #058283;
    font-size: 12px;
  }

  .title {
    font-size: 2rem;
    font-weight: 800;
  }

  .team {
    font-size: 2rem;
    font-weight: 800;
    color: #058283;
    background-color: #d5e7e8;
    padding: 5px 5px;
  }

  p {
    width: 60%;
    font-size: 13px;
    color: grey;
  }

  .divider {
    position: absolute;
    bottom: -50px;
    left: 50%;
    transform: translate(-50%, -50%);

    img {
      width: 50px;
      object-fit: cover;
    }
  }
}
</style>
