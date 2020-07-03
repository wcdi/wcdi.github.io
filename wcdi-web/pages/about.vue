<template>
  <div>
    <Header pageTitle="About Us"></Header>
    <div class="Container">
      <h2 class="title">ITRCについて</h2>
      <div class="aboutContainer">
        <div class="text">
          <p>
            <span class="mobile-text">ITRCは、日本工学院八王子専門学校の学生が主体となって</span><span class="mobile-text">活動しているサークルです。</span>
          </p>
        </div>
        <div class="philosophy">
          <div class="sub-title">
            <h3 class="sub-title-text">理念</h3>
          </div>
          <div class="text">
            <p>
              <span class="mobile-text">We Can Do It（やればできる）の理念のもとに</span><span class="mobile-text">情報技術に興味のある学生が集まり、</span><span class="mobile-text">日々自己研鑽に努めています。</span>
            </p>
          </div>
        </div>
        <div class="env">
          <div class="sub-title">
            <h3 class="sub-title-text">環境</h3>
          </div>
          <div class="text">
            <p>
              <span class="mobile-text">レベルとしては入学前から勉強していた人も多く、</span>
            </p>
            <p>
              <span class="mobile-text">過去には入学してから</span><span class="mobile-text">初めて本格的にパソコンを触ったような人も</span><span class="mobile-text">在籍していました。</span>
            </p>
            <p>
              <span class="mobile-text">初心者であってもビギナー向けの大会などで</span><span class="mobile-text">活躍する事が可能となっています。</span>
            </p>
          </div>
        </div>
        <div class="member">
          <div class="sub-title">
            <h3 class="sub-title-text">メンバー</h3>
          </div>
          <div class="text">
            <p>
              <span class="mobile-text">メンバーにはITスペシャリスト科の学生が多いですが、</span>
              <span class="mobile-text">他学科のメンバーも在籍しています。</span>
            </p>
            <p>
              <span class="mobile-text">また、同じ学科・専攻であっても</span>
              <span class="mobile-text">普段勉強している内容は違うことも多いため、</span>
              <span class="mobile-text">様々な分野の情報を交換したり、</span>
              <span class="mobile-text">それぞれの得意分野を活かして大会に出る事もあります。</span>
            </p>
          </div>
        </div>
        <div>
          <div class="section-line"></div>
          <div class="text">
            <p>
              <span class="mobile-text">このように、全体的に間口の広いサークルとなっています。</span>
            </p>
            <p>
              <span class="mobile-text">また、Twitterで直近の活動情報などを発信しているので、</span>
              <span class="mobile-text">興味のある方は是非ご活用ください。</span>
            </p>
            <div class="section-line"></div>
          </div>
        </div>
      </div>
    <p class="backtotop">Top→</p>
    <!-- Topボタンはまだただのカカシ -->
    </div>
    <Footer></Footer>
  </div>
</template>

<script>
  import Header from '../components/Header';
  import Footer from '../components/Footer';
  export default {
    name: "about",
    components: {
      Header,
      Footer
    }
  }
</script>

<style scoped>
.Container {
  padding: 3vh 15vw;
  display: flex;
  flex-direction: column;
}
h2.title {
  border-bottom: solid 3px #006F87;
  display: inline-block;
  margin: 0 auto 0;
}
p {
  padding: 1.5vh 0;
}
.backtotop {
  font-weight: bold;
  margin-left: auto;
}
.aboutContainer {
  padding: 3vh 0;
}
.sub-title-text {
  display: none;
}
@media screen and (max-width: 768px) {
  .sub-title {
    text-align: center;
  }
  h3.sub-title-text {
  border-bottom: solid 3px #006F87;
  display: inline-block;
  margin: 3vh auto 1vh;
  }
  .mobile-text {
    display: inline-block;
    padding: 1.5vh 0;
  }
  .section-line {
    display: flex;
    align-items: center;
    height: 1px;
    background-color: #006F87;
    margin: 3vh;
  }
}
@media screen and (max-width: 426px) {
  .mobile-text {
    padding: 0;
  }
}
</style>
