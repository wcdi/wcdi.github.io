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

          <div class="AboutUsButtonSize">
            <a id="ButtonText" href="./about">
              <div class="AboutUsButton">about us</div>
            </a>
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

  .AboutUsButtonSize {
    display: flex;
    font-size: 1.6em;
    margin-top: 4rem;
    margin-left: 70%;
  }
.AboutUsButton {
  background: #208cc2;
  color: #fff;
  border: none;
  position: relative;
  height: 35px;
  width: 150px;
  cursor: pointer;
  transition: 800ms ease all;
  outline: none;
}
.AboutUsButton:hover {
  background: #fff;
  color: #72aef3;
}
.AboutUsButton:before,
.AboutUsButton:after {
  content: "";
  position: absolute;
  top: 0;
  right: 0;
  height: 2px;
  width: 0;
  background: #208cc2;
  transition: 400ms ease all;
}
.AboutUsButton:after {
  right: inherit;
  top: inherit;
  left: 0;
  bottom: 0;
}
.AboutUsButton:hover:before,
.AboutUsButton:hover:after {
  width: 100%;
  transition: 800ms ease all;
}

  #ButtonText {
  color: rgb(255, 255, 255);
  text-decoration: none;
  font-size: 25px;
}
  .text br {
    display: none;
  }

  @media screen and (max-width: 784px) {
    .text  br {
      display: inline-block;
    }
    .AboutUsButtonSize {
      margin-left: auto;
      margin-right: auto;
      justify-content: center;
    }
  }
</style>
