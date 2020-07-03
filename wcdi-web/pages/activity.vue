<template>
  <div>
    <Header pageTitle="活動ログ"></Header>
    <div class="Container">
      <h2 class="title">最近の活動</h2>
      <div class="activityContainer">
        <h3 class="title">2020年2月</h3>
        <ul class="activities">
          <li>
            <h3>
              ICTトラブルシューティングコンテスト<span class="mobile-subtitle">本戦</span>
            </h3>
          </li>
          <p>
            <span class="mobile-text">ICTトラブルシューティングコンテストの</span><span class="mobile-text">本戦にリモートで参加しました。</span>
          </p>
        </ul>
        <h3 class="title">2019年12月</h3>
        <ul class="activities">
          <li>
            <h3>
              コミックマーケット<span class="mobile-subtitle">98</span>
            </h3>
          </li>
          <p>
            <span class="mobile-text">コミックマーケットC98にサークル参加し、</span><span class="mobile-text">技術関連の同人誌を発行しました。</span>
          </p>
          <li>
            <h3>
              ICTトラブルシューティングコンテスト<span class="mobile-subtitle">2次予選</span>
            </h3>
          </li>
          <p>
            <span class="mobile-text">ICTトラブルシューティングコンテストの</span><span class="mobile-text">2次予選に参加し、</span><span class="mobile-text">新人特別枠で本戦に進出しました。</span>
          </p>
        </ul>
        <h3 class="title">2019年8月</h3>
        <ul class="activities">
          <li>
            <h3>
              ICTトラブルシューティングコンテスト<span class="mobile-subtitle">1次予選</span>
            </h3>
          </li>
          <p>
            <span class="mobile-text">ICTトラブルシューティングコンテストという、</span><span class="mobile-text">ネットワークやサーバで発生した問題を解決する技術コンテストの</span><span class="mobile-text">1次予選に参加しました。</span>
          </p>
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
@media screen and (max-width: 768px) {
  .mobile-text {
    display: inline-block;
  }
  .mobile-subtitle {
    display: inline-block;
  }
  h3 {
    margin: 3vh auto 1vh;
  }
}
</style>
