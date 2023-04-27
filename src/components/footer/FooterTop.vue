<script>
import MyButton from "../commons/MyButton.vue";
import CardListFooter from "../footer/CardListFooter.vue";
export default {
  name: "FooterTop",
  data() {
    const listArray = [
      [
        "About",
        "The Company",
        "Istitutional",
        "Social & Event",
        "Innovation",
        "Environment",
        "Technology",
      ],
      [
        "Services",
        "Audit & Assurance",
        "Finalcial Advisory",
        "Analist M&A",
        "Middle Marketing",
        "Legal Consulting",
        "regulatory Risk",
      ],
      [
        "Support",
        "Responsibility",
        "Terms Of Use",
        "About Cookies",
        "Privacy Policy",
        "Accessibility",
        "Information",
      ],
    ];
    return {
      listArray,
    };
  },
  components: {
    MyButton,
    CardListFooter,
  },
};
</script>

<template>
  <div class="footer-top text-white">
    <div class="ms_container d-flex">
      <div class="info">
        <div class="logo">
          <img src="../../assets/images/logo.PNG" alt="" />
        </div>
        <p class="my-3">A Functional HTML template for Corporate & Business</p>
        <div class="d-flex align-items-center my-3">
          <i class="fa-solid fa-phone mx-1"></i>
          <div class="ms-2">+1 (305) 1234-5678</div>
        </div>
        <div class="d-flex align-items-center my-3">
          <i class="fa-solid fa-envelope mx-1"></i>
          <div class="ms-2">hello@example.com</div>
        </div>
        <div class="d-flex align-items-center my-3">
          <i class="fa-solid fa-location-dot"></i>
          <div class="ms-2">Main Avenue, 987</div>
        </div>
        <div class="mt-4">
          <MyButton
            :text="'READ MORE'"
            :variant="'trasparent'"
            class="text-white"
          />
        </div>
      </div>
      <div class="ms_row">
        <CardListFooter
          v-for="(list, index) in listArray"
          :key="index"
          :list="list"
        />
      </div>
    </div>
  </div>
</template>

<style scoped lang="scss">
.footer-top {
  padding: 100px 0;
  background-color: #111117;

  .info {
    font-size: 13px;
    width: 20%;
  }

  .logo {
    img {
      width: 115px;
      object-fit: cover;
    }
  }

  .ms_row {
    display: flex;
    width: 100%;
  }
}
</style>
