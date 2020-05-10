<template>
  <!-- ここにHTML書いてね -->
  <div class="access">
    <h2>アクセス</h2>
    <div class="contents">
      <div class="item">
        <h3>MAP</h3>
        <img src="../static/schoolmap.jpg">
      </div>
      <div class="item">
        <h3>活動時間</h3>
        <div class="text">
          <p>平日：17:00~19:00</p>
          <p>学校がある日は基本的に活動しています</p>
        </div>
      </div>
    </div>
    <div class="contents">
      <div class="item">
        <h3>活動場所</h3>
        <div class="text">
          <p>サークル棟 3階 304号室</p>
        </div>
      </div>
      <div class="item">
        <h3>部室</h3>
        <img src="../static/roommap.jpg">
      </div>
    </div>
  </div>
</template>

<script>
  // 現状ここは無視でいいよ
  export default {};
</script>


<style>
  /* ここにCSS書いてね */

  .access {
    width: 100%;
    color: #f7f8fb;
    background-color: #1D3156;
    padding-top: 1em;
    padding-bottom: 1em;
    text-align: center;
  }

  @media screen and ( min-width: 880px ) {
    .contents {
      margin: 2em auto 1em;
      width: 60%;
      display: flex;
      justify-content: center;
    }
  }

  .item {
    width: 50%;
    border-bottom: #f7f8fb solid 2px;
    height: auto;
  }

  .text {
    margin-top: 4em;
  }

  @media screen and ( max-width: 880px ) {
    .contents {
      margin: 2em auto 1em;
      width: 80%;
    }
  }

  img {
    max-height: 100%;
  }
</style>
