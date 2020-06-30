<template>
  <div>
    <Header pageTitle="コミックマーケット98にサークル参加します"></Header>
    <div class="Container">
      <h2 class="title">概要</h2>
      <div class="InformationContainer">
        <ul>
          <li>
            <h3>場所</h3
          ></li>
          <p>東京ビッグサイト  南4</p>
          <li>
            <h3>説明</h3>
          </li>
          <p>
            <span class="mobile-text">東京ビックサイトやコミックマーケットについては</span><span class="mobile-text">コミックマーケット公式サイトをご覧ください。</span>
          </p>
          <li>
            <h3>hogehoge</h3>
          </li>
          <p>fugafuga</p>
        </ul>
        <img src="/bigsite.jpg">
      </div>
      <h2 class="title">最新のお知らせ一覧</h2>
      <div class="InformationContainer">
        <ul>
          <li>
            <span class="mobile-text">コミックマーケット98に</span><span class="mobile-text">サークル参加します</span>
          </li>
          <li>
            <span class="mobile-text">コミックマーケット98に</span><span class="mobile-text">サークル参加します</span>
          </li>
          <li>
            <span class="mobile-text">コミックマーケット98に</span><span class="mobile-text">サークル参加します</span>
          </li>
        </ul>
      </div>
      <p class="backtotop">Top→</p>
    </div>
  </div>
</template>

<script>
  import Header from '@/components/Header';
  export default {
    name: "information",
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
.title {
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
div.InformationContainer {
  display: flex;
  justify-content: center;
  flex-wrap: wrap;
  padding-top: 5vh;
}
img {
  max-width: 50%;
  max-height: 50%;
  margin: 2vh 0;
}
@media screen and (max-width: 1000px) {
  .mobile-text {
    display: inline-block;
    text-align: left;
  }
}
@media screen and (max-width: 426px) {
  img {
    max-width: 70%;
    max-height: 70%;
  }
}
</style>
