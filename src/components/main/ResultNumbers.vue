<script>
export default {
  name: "ResultNumbers",
  data() {
    return {};
  },
};
</script>

<template>
  <div class="result-numbers">
    <div class="ms_container text-center">
      <div class="doing">WHAT ARE YOU DOING</div>
      <div class="d-flex justify-content-center my-4">
        <div class="result">Risult</div>
        <div class="numbers">in Numbers</div>
      </div>
      <ul>
        <li>
          <div class="numb">128</div>
          <div class="text">Certification</div>
        </li>
        <li>
          <div class="numb">230</div>
          <div class="text">Employees</div>
        </li>
        <li>
          <div class="numb">517</div>
          <div class="text">Costumers</div>
        </li>
        <li>
          <div class="numb">94</div>
          <div class="text">Contries Served</div>
        </li>
      </ul>
    </div>
  </div>
</template>

<style scoped lang="scss">
.result-numbers {
  padding: 100px 0;
  background-image: url(../../assets/images/bg-7.jpg);
  background-size: 100%;

  color: white;

  .doing {
    color: #058283;
    font-size: 12px;
    font-weight: 800;
  }

  .result {
    font-size: 2rem;
    font-weight: 800;
    background-color: #0e272d;
    padding: 1px 5px;
  }

  .numbers {
    font-size: 2rem;
    font-weight: 800;
  }

  ul {
    display: flex;
    justify-content: center;
    gap: 90px;
    margin-top: 30px;
    li {
      .numb {
        color: #058283;
        font-size: 40px;
        font-weight: 700;
      }

      .text {
        font-size: 20px;
        font-weight: 600;
      }
    }
  }
}
</style>
