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
    background-color: rgb(65, 111, 211);
    color: #fff;
    font-weight: bold;
    font-size: 22px;
    padding: 2rem 8rem;
    border-radius: 30px;
    text-decoration: none;
     -webkit-transition: all 200ms cubic-bezier(0.390, 0.500, 0.150, 1.360);
    -moz-transition: all 200ms cubic-bezier(0.390, 0.500, 0.150, 1.360);
    -ms-transition: all 200ms cubic-bezier(0.390, 0.500, 0.150, 1.360);
    -o-transition: all 200ms cubic-bezier(0.390, 0.500, 0.150, 1.360);
    transition: all 200ms cubic-bezier(0.390, 0.500, 0.150, 1.360);
  }

  .ContactButton:hover {
    color: rgba(255, 255, 255);
    box-shadow: #555aaa 0 0px 0px 50px inset;
}

  @media screen and (max-width: 576px) {
    .ContactButton {
      padding: 1rem 2rem;
    }
  }

</style>
