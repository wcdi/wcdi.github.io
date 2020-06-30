<template>
  <!-- ここにHTML書いてね -->
  <div class="SectionContainer">
    <div class="Contents">
      <div id="ITRC_Title">
        <p>情報技術研究部</p>
      </div>
      <div class="ArticleContainer">
        <div>
          <p>情報技術研究部は日本工学院八王子専門学校にて活動中のサークルです</p>
          <p>それぞれ高い目標を持つ部員が集まり活動しています</p>
          <p>定期的にもくもく会, LT大会, コンテストの参加を行い日々研鑽を重ねています</p>
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
@font-face {
    font-family: 'Rationale';
    src: url(../assets/fonts/Rationale-Regular.ttf);
  }
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

  .AboutUsButtonSize{
   
    font-size:1.6em;
    padding:0 2em;
    margin-top: 4rem;
    margin-left: 65%;
    margin-right: 25%; 
  }
  .AboutUsButton {
    background:#208cc2;
    color:#fff;
    border:none;
    position:relative;
    height:35px;
    width: 150px;
    cursor:pointer;
    transition:800ms ease all;
    outline:none;
    border-radius:10px 0px 10px 0px;
  }
   .AboutUsButton:hover{
    background:#fff;
    color:#72aef3;
   }
  .AboutUsButton:before,.AboutUsButton:after{
    content:'';
    position:absolute;
    top:0;
    right:0;
    height:2px;
    width:0;
    background: #208cc2;
    transition:400ms ease all;
  }
  .AboutUsButton:after{
    right:inherit;
    top:inherit;
    left:0;
    bottom:0;
  }
  .AboutUsButton:hover:before,.AboutUsButton:hover:after{
    width:100%;
    transition:800ms ease all;
  }
   #ButtonText {
    color: rgb(255, 255, 255);
    text-decoration: none;
    font-size: 25px;
  }
  @media screen and (max-width: 1000px) {
    
    .AboutUsButtonSize{
    
      font-size:1.6em;
      padding:0 2em;
      margin-top: 4rem;
      margin-left: 30%;
      margin-right: 30%; 
    }
  }
  @media screen and (max-width: 600px) {
    
    .AboutUsButtonSize{
    
      font-size:1.6em;
      padding:0 2em;
      margin-top: 4rem;
      margin-left: 20%;
      margin-right: 20%; 
    }
  }
  @media screen and (max-width: 600px) {
    
    .AboutUsButtonSize{
    
      font-size:1.6em;
      padding:0 2em;
      margin-top: 4rem;
      margin-left: 10%;
      margin-right: 10%; 
    }
  }
</style>
