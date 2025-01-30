<script>
export default {
  name: 'V-Header',
}
</script>

<template>
  <header>
    <div class="h_item">
      <img src="../assets/weather.png" alt=""/>
    </div>
    <h2>한국공학대학교 재학생 크롬 익스텐션</h2>
    <div class="h_item">
      <img src="../assets/meal.png" alt=""/>
    </div>
  </header>
</template>

<style>
  h2 {
    color: #3c63ae;
  }

  header {
    max-width: 100%;
    display: flex;
    justify-content: space-between;
    background-color: rgba(255, 255, 255, 1.0);
    padding: 10px;
  }

  .h_item {
    width: 5.5rem;
    display: flex;
    justify-content: center;
    align-items: center;

    img {
      width: 50%;
      height: fit-content;
    }
  }
</style>
