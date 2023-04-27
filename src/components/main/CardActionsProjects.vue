<script>
export default {
  name: "CardActionProjects",
  props: {
    text: String,
    image: String,
  },
  data() {
    return {};
  },
  methods: {
    getCardImg() {
      return new URL(`../../assets/images/${this.image}`, import.meta.url).href;
    },
  },
};
</script>

<template>
  <div class="ms_card">
    <div class="overlay"></div>
    <img :src="getCardImg()" alt="" />
    <div class="title-card">
      <div class="ms_text">{{ text }}</div>
    </div>
  </div>
</template>

<style scoped lang="scss">
.ms_card {
  background-color: white;
  border: 1px solid black;
  border-radius: 10px;
  width: calc(100% / 3 - 20px);
  height: 300px;
  margin: 10px;
  position: relative;
  overflow: hidden;

  .overlay {
    position: absolute;
    top: 0;
    left: 0;
    width: 100%;
    height: 100%;
    background-color: rgba(0, 0, 0, 0.6);
  }

  img {
    width: 100%;
    height: 100%;
    object-fit: cover;
    border-radius: 10px;
  }

  .title-card {
    color: white;
    font-weight: 800;
    font-size: 19px;

    .ms_text {
      position: absolute;
      bottom: 30px;
    }
  }
}
</style>
