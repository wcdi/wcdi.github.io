<template>
  <div class="SectionContainer">
    <h2 class="SectionTitle">コンタクト</h2>
    <div class="Contents">
      <a
        class="ContactButton"
        href="https://docs.google.com/forms/d/15WcQIkXtw05Mp33BrtDshMIHhfjJwTIquOIZpzQ69ug/edit"
        target="_blank"
        rel="noopener"
      >Googleフォームへ</a>
    </div>
  </div>
</template>

<script>
  // 現状ここは無視でいいよ
  export default {};
</script>

<style scoped>
  /* ここにCSS書いてね */
  .SectionContainer {
    background-color: #F5F5F5;
  }

  .Contents {
    display: flex;
    flex-direction: column;
    align-items: center;
  }

  .ContactButton {
    background-color: #555aaa;
    color: #fff;
    font-weight: bold;
    font-size: 22px;
    padding: 2rem 8rem;
    border-radius: 30px;
    text-decoration: none;
  }

  @media screen and (max-width: 576px) {
    .ContactButton {
      padding: 1rem 2rem;
    }
  }
</style>
