<template>
  <div>
    <Header pageTitle="活動ログ"></Header>
    <div class="Container">
      <h2 class="title">最近の活動</h2>
      <div class="activityContainer">
        <h3 class="title">2019年12月</h3>
        <ul class="activities">
          <li><h3>コミックマーケット98</h3></li>
          <p>コミックマーケットC98にサークル参加し、技術関連の同人誌を発行しました。</p>
        </ul>
        <h3 class="title">2019年8月</h3>
        <ul class="activities">
          <li><h3>ICTトラブルシューティングコンテスト1次予選</h3></li>
          <p>ICTトラブルシューティングコンテストという、ネットワークやサーバで発生した問題を解決する技術コンテストの1次予選に参加しました。hogeチーム中foo位</p>
        </ul>
      </div>
      <p class="backtotop">Top→</p>
    </div>
  </div>
</template>

<script>
  import Header from '../components/Header';
    export default {
        name: "activity",
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
.activityContainer {
  display: flex;
  flex-direction: column;
  margin-top: 5vh;
  justify-content: center;
}
.activities {
  padding: 3vh 10vw;
}
</style>
