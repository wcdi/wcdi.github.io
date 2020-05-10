<template>
  <div class=contact-section>
      <p>コンタクト</p>
      <button onclick="location.href='https://docs.google.com/forms/d/15WcQIkXtw05Mp33BrtDshMIHhfjJwTIquOIZpzQ69ug/edit'">Googleフォームへ</button>
  </div>
</template>

<script>
// 現状ここは無視でいいよ
export default {};
</script>

<style>
/* ここにCSS書いてね */
.contact-section {
  position:relative;
  width: 100%;
  height: 412px;
  padding: 82px 0 82px 0;
  background: #ffffff;
  text-align: center;
}

.contact-section p{
  font-style: normal;
  font-weight: bold;
  font-size: 34px;

  color: #55AAFF;
}

.contact-section button{
  position:relative;
  width: 576px;
  height: 128px;
  bottom: -70px;

  font-style: normal;
  font-weight: bold;
  font-size: 30px;

  color: #ffffff;
  background: #555AAA;
  border-radius: 30px;
}

</style>