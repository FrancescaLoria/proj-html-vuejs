<script>
import MyButton from "../commons/MyButton.vue";
export default {
  name: "SectionInput",
  data() {
    return {};
  },
  components: {
    MyButton,
  },
};
</script>

<template>
  <div class="input">
    <div class="ms_container d-flex">
      <div class="left">
        <div class="message">SEND A MESSAGE</div>
        <div class="d-flex my-3">
          <div class="get">Get in</div>
          <div class="touch">Touch</div>
        </div>
        <p>We will respond to your message as soon as possible.</p>
        <div class="d-flex cont">
          <div class="form-floating mb-3 me-3">
            <input
              type="name"
              class="form-control ms_input"
              id="floatingInputDisabled"
              placeholder="name@example.com"
              disabled
            />
            <label for="floatingInputDisabled">Name</label>
          </div>
          <div class="form-floating mb-3">
            <input
              type="email"
              class="form-control ms_input"
              id="floatingInputDisabled"
              placeholder="name@example.com"
              disabled
            />
            <label for="floatingInputDisabled">Email</label>
          </div>
        </div>
        <div class="d-flex cont">
          <div class="form-floating mb-3 me-3">
            <input
              type="email"
              class="form-control ms_input"
              id="floatingInputDisabled"
              placeholder="name@example.com"
              disabled
            />
            <label for="floatingInputDisabled">Phone</label>
          </div>
          <div class="form-floating mb-3">
            <input
              type="email"
              class="form-control ms_input"
              id="floatingInputDisabled"
              placeholder="name@example.com"
              disabled
            />
            <label for="floatingInputDisabled">More info</label>
          </div>
        </div>
        <div class="form-floating ms_textarea mb-3">
          <textarea
            class="form-control"
            placeholder="Leave a comment here"
            id="floatingTextarea2Disabled"
            style="height: 150px"
            disabled
          ></textarea>
          <label for="floatingTextarea2Disabled">Message</label>
        </div>
        <div>
          <MyButton :text="'SEND'" :variant="'blue'" />
        </div>
      </div>
      <div class="right">
        <div class="title-right">Example Inc.</div>
        <p class="mt-3">
          Lorem ipsum dolor sit amet consectetur adipisicing elit.
        </p>
        <p class="mb-5">
          Quae voluptate numquam doloribus excepturi nulla quasi explicabo
          molestias.
        </p>
        <div class="d-flex align-items-center my-3">
          <i class="fa-solid fa-phone mx-1"></i>
          <div class="ms-2 text">+1 (305) 1234-5678</div>
        </div>
        <div class="d-flex align-items-center my-3">
          <i class="fa-solid fa-envelope mx-1"></i>
          <div class="ms-2 text">hello@example.com</div>
        </div>
        <div class="d-flex align-items-center my-3">
          <i class="fa-solid fa-location-dot last"></i>
          <div class="ms-2 text">Main Avenue, 987</div>
        </div>
        <div class="mt-4">
          <MyButton :text="'VIEW MAP'" :variant="'trasparent'" class="ms_btn" />
        </div>
      </div>
    </div>
  </div>
</template>

<style scoped lang="scss">
.input {
  padding: 100px 0;

  .left {
    width: 80%;
  }

  .cont {
    width: 100%;
  }

  .message {
    color: #058283;
    font-size: 12px;
    font-weight: 600;
  }

  .get {
    font-size: 2.5rem;
    font-weight: 800;
  }

  .touch {
    font-size: 2.5rem;
    font-weight: 800;
    color: #058283;
    background-color: #d5e7e8;
    padding: 2px 5px;
  }

  p {
    font-size: 13px;
    color: grey;
  }

  .right {
    padding-left: 20px;
    .title-right {
      font-size: 20px;
      font-weight: 700;
    }

    .fa-solid,
    .text {
      color: #058283;
    }

    .last {
      margin-left: 5px;
    }

    .fa-solid {
      background-color: #daeced;
      padding: 10px;
      border-radius: 100%;
    }

    .ms_btn {
      color: #058283;
      font-weight: 600;
    }
  }

  .ms_input {
    height: 50px;
  }

  .form-floating:not(.ms_textarea) {
    width: 50%;
  }
}
</style>
