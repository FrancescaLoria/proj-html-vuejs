<script>
import MyButton from "../commons/MyButton.vue";
export default {
  name: "SectionNetwork",
  data() {
    return {};
  },
  components: {
    MyButton,
  },
};
</script>

<template>
  <div class="network d-flex">
    <div class="about">
      <div class="cont-net">
        <div class="title-about mb-3">ABOUT THE NETWORK</div>
        <div class="d-flex">
          <div class="the me-2">The</div>
          <div class="company">Company</div>
        </div>
        <p class="mt-3">
          For 12 years we have been providing audit and warranty, finalcial
          advice, risk advice, texes and related services to select clients.
        </p>
        <div class="d-flex my-5">
          <div class="box">
            <div class="d-flex mb-3">
              <i class="fa-solid fa-medal awesome"></i>
              <div class="title-box ms-2">Tradition</div>
            </div>
            <p>Lorem ipsum, dolor sit amet consectetur adipisicing elit.</p>
          </div>
          <div class="box">
            <div class="d-flex mb-3">
              <i class="fa-solid fa-lock awesome"></i>
              <div class="title-box ms-2">Security</div>
            </div>
            <p>Lorem ipsum, dolor sit amet consectetur adipisicing elit.</p>
          </div>
        </div>
        <div class="d-flex">
          <div class="box">
            <div class="d-flex mb-3">
              <i class="fa-solid fa-pen-to-square awesome"></i>
              <div class="title-box ms-2">Certificate</div>
            </div>
            <p>Lorem ipsum, dolor sit amet consectetur adipisicing elit.</p>
          </div>
          <div class="box">
            <div class="d-flex mb-3">
              <i class="fa-solid fa-graduation-cap awesome"></i>
              <div class="title-box ms-2">Expertise</div>
            </div>
            <p>Lorem ipsum, dolor sit amet consectetur adipisicing elit.</p>
          </div>
        </div>
        <div class="mt-5">
          <MyButton :text="'GET IN TOUCH'" :variant="'blue'" class="me-3" />
          <MyButton
            :text="'READ MORE'"
            :variant="'trasparent'"
            class="text-white"
          />
        </div>
      </div>
    </div>
    <div class="img-network"></div>
  </div>
</template>

<style scoped lang="scss">
.network {
  background-color: #111117;
  color: white;

  .about {
    width: 50%;
  }

  .cont-net {
    margin-left: 215px;
    padding: 100px 0;
  }

  .title-about {
    color: #058283;
    font-size: 12px;
  }

  .the {
    font-size: 2rem;
    font-weight: 800;
    background-color: #0e272d;
    padding: 1px 5px;
  }

  .company {
    font-size: 2rem;
    font-weight: 800;
  }

  p {
    font-size: 13px;
    width: 80%;
    color: lightgray;
  }

  .awesome {
    color: #058283;
    font-size: 20px;
  }

  .title-box {
    font-size: 1rem;
    font-weight: 600;
  }
}

.img-network {
  width: 50%;
  background-image: url(../../assets/images/about-4.jpg);
  background-size: 100%;
}
</style>
