<template>
  <!-- ここにHTML書いてね -->
  <div class="container">
    <div class="header">
      <p>情報技術研究部？</p>
      <p>ITRC? WCDI?</p>
    </div>

    <div class="contents">
      <div>
        <p>情報技術研究部は日本工学院八王子専門学校の部活動です</p>
        <p>[WCDIの説明]</p>
        <p>[ITRCの説明]</p>
        <p>[現在活動していること]</p>
      </div>
      <div class="side">
        <img src="../static/exampleImage.jpeg" alt="ITRCの関係図" title="ITRC関係図" />
      </div>
    </div>
  </div>
</template>

<script>
// 現状ここは無視でいいよ
export default {};
</script>


<style scoped>
/* ここにCSS書いてね */
.container {
  background-color: rgb(236, 235, 235);
  padding: 2rem;
  text-align: center;
}
.side {
  align-content: flex-end;
  height: auto;
}
.contents {
  margin: 2rem 0;
  display: flex;
  justify-content: space-around;
}
.side > img {
  width: 100%;
  max-width: 100%;
  height: auto;
}
.header > p {
  font-size: 5rem;
}
.header > p:nth-child(1) {
  margin-bottom: 1rem;
}
</style>