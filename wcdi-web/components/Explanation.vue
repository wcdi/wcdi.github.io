<template>
  <!-- ここにHTML書いてね -->
  <div class="Container">
    <div class = "header">
      <h1>情報技術研究部？</h1>
      <br>
      <h1>ITRC? WCDI?</h1>
    </div>

    <div class="contents">
      <div class="main">
        <p>
          情報技術研究部は日本工学院八王子専門学校の部活動です<br>
          [WCDIの説明]<br>
          [ITRCの説明]<br>
          [現在活動していること]
        </p>
      </div>
      <div class="side">
        <img src="./../assets/サンプル画像.jpeg" alt="ITRCの関係図" title="ITRC関係図" >
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
.Container {
  background-color : rgb(236, 235, 235);
  padding: 3rem;
  max-width: 1920px;
  max-height: 1080px;
  min-width: 850px;
  margin-right: auto;
  margin-left: auto;
  text-align: center;
}
.main {
  padding: 3rem 1rem 0 0;
}
.side{
  align-content: flex-end;
  height: auto;
}
.contents  {
  padding: 2rem 3rem;
  display: flex;
  justify-content: space-around;
}
.side > img {
  width:100%;
  max-width: 100%;
  height: auto;
}
.header > h1{
  font-size: 5rem;
}
</style>