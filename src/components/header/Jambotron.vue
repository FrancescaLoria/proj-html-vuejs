<script>
import MyButton from "../commons/MyButton.vue";
export default {
  name: "jambotron",
  data() {
    return {};
  },
  components: {
    MyButton,
  },
};
</script>

<template>
  <div class="jambotron">
    <div class="nav-bar">
      <div
        class="ms_container d-flex justify-content-between align-items-center pt-3"
      >
        <div class="logo">
          <img src="../../assets/images/logo.PNG" alt="" />
        </div>
        <div class="ms_nav d-flex">
          <ul class="list">
            <li>
              <a href="">HOME</a>
            </li>
            <li>
              <a href="">SERVICE</a>
            </li>
            <li>
              <a href="">ABOUT</a>
            </li>
            <li>
              <a href="">PROJECTS</a>
            </li>
            <li>
              <a href="">RESULTS</a>
            </li>
          </ul>
          <div class="ms-3">
            <MyButton :text="'GET IN TOUCH'" :variant="'blue'" />
          </div>
        </div>
      </div>
    </div>
    <div class="ready-team">
      <div class="ms_cont-rt">
        <div class="jambo-title d-flex">
          <div class="title">Ready</div>
          <div class="team">Team</div>
        </div>
        <p class="text-center">
          No matter what your company needs, we will be ready to assist you in
          the best possible way
        </p>
        <div>
          <MyButton :text="'GET IN TOUCH'" :variant="'blue'" class="me-3" />
          <MyButton :text="'READ MORE'" :variant="'trasparent'" />
        </div>
      </div>
    </div>
  </div>
</template>

<style scoped lang="scss">
.jambotron {
  height: 600px;

  background-image: url(../../assets/images/immaginesfondo.png);
  background-repeat: no-repeat;
  background-size: 100%;

  .nav-bar {
    .logo {
      img {
        width: 110px;
        object-fit: cover;
      }
    }

    .ms_nav {
      .list {
        display: flex;
        gap: 30px;
        align-items: center;
        font-size: 14px;
        margin-bottom: 0;
      }
    }
  }

  .ready-team {
    height: 92%;
    .ms_cont-rt {
      width: 35%;
      height: 100%;
      margin: 0 auto;
      display: flex;
      flex-direction: column;
      justify-content: center;
      align-items: center;

      p {
        width: 60%;
        font-size: 13px;
      }
    }

    .jambo-title {
      .title {
        font-size: 3rem;
        font-weight: 800;
      }

      .team {
        font-size: 3rem;
        font-weight: 800;
        color: #058283;
        background-color: #d5e7e8;
        padding: 5px 5px;
      }
    }
  }
}
</style>
