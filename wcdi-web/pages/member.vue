<template>
  <div>
    <Header pageTitle="メンバー"></Header>
    <div class="Container">
      <h2 class="title">メンバー一覧</h2>
      <div class="content">
        <p>
          <span class="mobile-text">情報技術研究部には日本工学院八王子専門学校の</span><span class="mobile-text">1年生から4年生が在籍しています。</span>
        </p>
        <p>
          <span class="mobile-text">情報技術を好きな学生が集まっており、</span><span class="mobile-text">日々自己研鑽に努めています。</span>
        </p>
        <p>
          <span class="mobile-text">メンバーにはITスペシャリスト科の学生が多いですが、</span><span class="mobile-text">日本工学院八王子専門学校の学生であれば</span><span class="mobile-text">どなたでも参加することができます。</span>
        </p>
        <p>
          <span class="mobile-text">レベルとしては入学前から勉強していた人も、</span><span class="mobile-text">入学してからプログラミングを始めた人もいます。</span>
        </p>
        <p>
          <span class="mobile-text">サークル活動が終わったあとラーメンを食べに行ったり、</span><span class="mobile-text">休日に出かけることもあり部員同士仲が良いです。</span>
        </p>
        <p>
          <span class="mobile-text">興味がある方は</span><span class="mobile-text">ぜひサークル棟3階304号室の情報技術研究部部室へ！</span>
        </p>
      </div>
      <p class="backtotop">Top→</p>
    </div>
  </div>
</template>

<script>
  import Header from '../components/Header';
  export default {
    name: "member",
    components: {
      Header
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
.content {
  display: flex;
  flex-direction: column;
  margin-top: 5vh;
  justify-content: center;
}
@media screen and (max-width: 1000px) {
  .mobile-text {
    display: inline-block;
    text-align: left;
    padding: 1.5vh 0;
  }
}
@media screen and (max-width: 426px) {
  .mobile-text {
    padding: 0.5vh 0;
  }
}
</style>
