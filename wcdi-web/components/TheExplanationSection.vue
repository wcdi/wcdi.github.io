<template>
  <!-- ここにHTML書いてね -->
  <div class="SectionContainer">
    <div class="Contents">
      <div id="ITRC_Title">
        <p>情報技術研究部</p>
      </div>
      <div class="ArticleContainer">
        <div>
          <p class="text">情報技術研究部は日本工学院八王子専門学校にて<br>活動中のサークルです</p>
          <p class="text">それぞれ<strong>高い目標</strong>を持つ部員が集まり活動しています</p>
          <p class="text">定期的にもくもく会, LT大会, コンテストの参加を行い<br>日々研鑽を重ねています</p>
         
          <div class="AboutUsButton">
            <a id="ButtonText" href="./about">about us ></a>
          </div>
        </div>
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
  .Contents {
    text-align: center;
  }

  #ITRC_Title {
    font-size: 64px;
  }

  .ArticleContainer {
    margin-top: 4rem;
    font-size: 22px;
  }

  .AboutUsButton {
    margin-top: 1rem;
    text-align: right;
    width: 80%;
  }

  #ButtonText {
    color: black;
    text-decoration: none;
    font-size: 18px;
  }
  .text br {
    display: none;
  }

  @media screen and (max-width: 784px) {
    .text  br {
      display: inline-block;
    }
  }
</style>
