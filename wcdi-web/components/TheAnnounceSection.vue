<template>
  <!-- ここにHTML書いてね -->
  <div class="SectionContainer">
    <h2 class="SectionTitle">最新のお知らせ</h2>
    <div class="Contents">
      <div class="AnnounceContainer">
        <p id="NewAnnouncementsText">新着お知らせ</p>
        <div
          v-for="announcement in announcements.slice(-5).reverse()"
          :key="announcement.id"
        >
          <div class="AnnounceItem">
            <a v-bind:href="announcement.url">
              <p class="AnnounceTitle">{{ announcement.title }}</p>
              <p class="AnnounceDate">{{ announcement.date }}</p>
            </a>
          </div>
        </div>
      </div>
      <div class="TwitterContainer">
        <a class="twitter-timeline" data-width="456" data-height="512" data-theme="light"
           href="https://twitter.com/Twitter?ref_src=twsrc%5Etfw">Tweets by Twitter</a>
        <script async src="https://platform.twitter.com/widgets.js" charset="utf-8"></script>
      </div>
    </div>
  </div>
</template>

<script>
  // 現状ここは無視でいいよ
  import announcements from '../assets/announcements.json';

  export default {
    data: function () {
      return {
        announcements: announcements
      };
    },
  }
</script>

<style scoped>
  /* ここにCSS書いてね */
  .SectionContainer {
    background-color: #F5F5F5;
  }

  .Contents {
    /*flexコンテナ*/
    padding-left: 8px;
    padding-right: 8px;
    margin-left: auto;
    margin-right: auto;
    display: flex;
    justify-content: center;
    width: 80%;
  }

  .AnnounceContainer {
    width: 700px;
    height: 512px;
    padding: 10px
  }

  #NewAnnouncementsText {
    height: 56px;
    padding: 10px;
    font-size: 22px;
    border-bottom: solid 1px #5a5a5a;
  }

  .AnnounceItem {
    width: 100%;
    height: 80px;
    padding: 8px;
  }
  .AnnounceItem:hover{
    background: #e9e9e9;
  }

  .AnnounceItem > a {
    text-decoration: none;
  }

  .AnnounceTitle {
    font-size: 18px;
    color: #201d1d;
    height: 44px;
    line-height: 22px;
  }

  .AnnounceDate {
    margin-top: 3px;
    margin-bottom: 3px;
    font-size: 14px;
    color: #5a5a5a;
    border-bottom: solid 1px #5a5a5a;
  }

  .TwitterContainer {
    width: 456px;
    height: 512px;
    padding: 8px;
  }

  /*#announce {*/
  /*  padding: 1rem;*/
  /*}*/

  /*.Container {*/
  /*  display: flex;*/
  /*  justify-content: space-around;*/
  /*}*/

  /*.announce-list {*/
  /*  display: flex;*/
  /*  height: 3rem;*/
  /*  align-items: center;*/
  /*  border: 1px solid;*/
  /*}*/

  /*.announce-list > p:nth-child(1) {*/
  /*  flex: 1;*/
  /*  text-align: center;*/
  /*  height: 100%;*/
  /*  display: flex;*/
  /*  align-items: center;*/
  /*  justify-content: center;*/
  /*  border-right: 1px solid;*/
  /*}*/

  /*.announce-list > p:nth-child(2) {*/
  /*  flex: 7;*/
  /*  padding: 0 0.5rem;*/
  /*}*/

  /*.announce-list > p:nth-child(3) {*/
  /*  flex: 3;*/
  /*  text-align: center;*/
  /*  height: 100%;*/
  /*  display: flex;*/
  /*  align-items: center;*/
  /*  justify-content: center;*/
  /*  border-left: 1px solid;*/
  /*}*/

  /*.content {*/
  /*  flex: 3;*/
  /*  margin: 0;*/
  /*}*/

  /*.TwitterContainer {*/
  /*  flex: 1;*/
  /*  height: 80vh;*/
  /*  overflow-y: auto;*/
  /*}*/

  /*.announceTitle {*/
  /*  text-align: center;*/
  /*  color: #55aaff;*/
  /*  margin: 1rem 0;*/
  /*}*/

  /*@media screen and (max-width: 960px) {*/
  /*  .Container {*/
  /*    flex-direction: column;*/
  /*  }*/

  /*  .content {*/
  /*    margin: 1rem 0;*/
  /*  }*/
  /*}*/

  @media screen and (max-width: 784px) {
    .Contents {
      display: block;
    }
    .AnnounceContainer {
      width: 100%;
    }
    .TwitterContainer {
      width: 100%;
    }
  }

</style>
