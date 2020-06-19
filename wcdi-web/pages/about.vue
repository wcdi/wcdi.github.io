<template>
  <div>
    <Header pageTitle="About Us"></Header>
    <div class="Container">
      <h2 class="title">ITRCについて</h2>
      <div class="aboutContainer">
        <p>ITRCは、日本工学院八王子専門学校の学生が主体となって活動しているサークルです。</p>
        <p>We Can Do It（やればできる）の理念のもとに情報技術に興味のある学生が集まり、日々自己研鑽に努めています。</p>
        <p>レベルとしては入学前から勉強していた人も多く、過去には入学してから初めて本格的にパソコンを触ったような人も在籍していました。初心者であってもビギナー向けの大会などで活躍する事が可能となっています。</p>
        <p>メンバーにはITスペシャリスト科の学生が多いですが、他学科のメンバーも在籍しています。また、同じ学科・専攻であっても普段勉強している内容は違うことも多いため、様々な分野の情報を交換したり、それぞれの得意分野を活かして大会に出る事もあります。</p>
        <p>このように、全体的に間口の広いサークルとなっています。また、Twitterで直近の活動情報などを発信しているので、興味のある方は是非ご活用ください。</p>
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
</style>
