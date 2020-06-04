<template>
  <div class="Container">
    <p class="ContactText">コンタクト</p>
    <a
      class="ContactButton"
      href="https://docs.google.com/forms/d/15WcQIkXtw05Mp33BrtDshMIHhfjJwTIquOIZpzQ69ug/edit"
      target="_blank"
      rel="noopener"
    >Googleフォームへ</a>
  </div>
</template>

<script>
// 現状ここは無視でいいよ
export default {};
</script>

<style scoped>
/* ここにCSS書いてね */
.Container {
  padding: 3rem 1rem;
  display: flex;
  flex-direction: column;
  align-items: center;
}

.ContactButton {
  background-color: #555aaa;
  color: #fff;
  font-weight: bold;
  font-size: 30px;
  padding: 2rem 8rem;
  border-radius: 30px;
}

.ContactText {
  color: #55aaff;
  font-weight: bold;
  font-size: 34px;
  margin-bottom: 6rem;
}

@media screen and (max-width: 576px) {
  .ContactButton {
    padding: 1rem 2rem;
  }
}
</style>
