<template>
  <div>
    <Header pageTitle="メンバー"></Header>
    <div class="Container">
      <h2 class="title">メンバー一覧</h2>
      <div class="content">
        <p>情報技術研究部には日本工学院八王子専門学校の１年生から４年生が在籍しています。</p>
        <p>情報技術を好きな学生が集まっており、日々自己研鑽に努めています。</p>

        <p>メンバーにはITスペシャリスト科の学生が多いですが、日本工学院八王子専門学校の学生であればどなたでも参加することができます。</p>

        <p>レベルとしては入学前から勉強していた人も、入学してからプログラミングを始めた人もいます。</p>
        <p>サークル活動が終わったあとラーメンを食べに行ったり、休日に出かけることもあり部員同士仲が良いです。</p>
        <p>興味がある方はぜひサークル棟３階304号室の情報技術研究部部室へ！ </p>
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
</style>
