<script>
import CardActionsProjects from "./CardActionsProjects.vue";
export default {
  name: "SectionActionProjects",
  data() {
    const cardArray = [
      {
        image: "project-1.jpg",
        text: "Academy professional program in social media",
      },
      {
        image: "project-2.jpg",
        text: "President's speech at the annual mithing",
      },
      {
        image: "project-3.jpg",
        text: "International business trip in Shangai",
      },
      {
        image: "project-4.jpg",
        text: "Technology workshop whit education team",
      },
      {
        image: "project-5.jpg",
        text: "Donation of clothes and food to the partner NGO",
      },
      {
        image: "project-6.jpg",
        text: "Confraternization of the procurement team",
      },
    ];
    return {
      cardArray,
    };
  },
  components: {
    CardActionsProjects,
  },
};
</script>

<template>
  <div class="projects">
    <div class="ms_container text-center">
      <div class="divider d-flex">
        <div>
          <img src="../../assets/images/bullets.png" alt="" />
        </div>
        <div>
          <img src="../../assets/images/bullets.png" alt="" />
        </div>
      </div>
      <div class="everyone mb-4">WE DO MORE FOR EVERYONE</div>
      <div class="d-flex justify-content-center">
        <div class="title">Actions &</div>
        <div class="proj">Projects</div>
      </div>
      <ul class="list mt-3">
        <li>
          <a href="">ALL</a>
        </li>
        <li>
          <a href="">INSTITUTIONAL</a>
        </li>
        <li>
          <a href="">SOCIAL</a>
        </li>
        <li>
          <a href="">EVENTS</a>
        </li>
        <li>
          <a href="">INNOVATION</a>
        </li>
        <li>
          <a href="">ENVIRONMENT</a>
        </li>
        <li>
          <a href="">TECHNOLOGY</a>
        </li>
      </ul>
      <div class="ms_row mt-4">
        <CardActionsProjects
          :text="card.text"
          :image="card.image"
          v-for="(card, index) in cardArray"
          :key="index"
        />
      </div>
    </div>
  </div>
</template>

<style scoped lang="scss">
.projects {
  padding: 100px 0;
  position: relative;

  .everyone {
    color: #058283;
    font-size: 12px;
  }

  .title {
    font-size: 2rem;
    font-weight: 800;
  }

  .proj {
    font-size: 2rem;
    font-weight: 800;
    color: #058283;
    background-color: #d5e7e8;
    padding: 5px 5px;
  }

  .list {
    display: flex;
    gap: 30px;
    justify-content: center;
    font-size: 14px;
    margin-bottom: 0;
  }

  .ms_row {
    display: flex;
    flex-wrap: wrap;
  }

  .divider {
    position: absolute;
    top: 0px;
    left: 50%;
    transform: translate(-50%, -50%);

    img {
      width: 50px;
      object-fit: cover;
    }
  }
}
</style>
