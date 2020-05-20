<template>
  <!-- ここにHTML書いてね -->
  <div id="announce">
    <h2 class="announceTitle">最新のお知らせ</h2>
    <div class="Container">
      <div class="content">
        <div
          v-for="announcement in announcements.slice().reverse()"
          :key="announcement.id"
        >
          <div class="annouce-list">
            <p>{{ announcement.id }}</p>
            <p>{{ announcement.title }}</p>
            <p>{{ announcement.date }}</p>
          </div>
        </div>
      </div>
      <div class="TwitterContainer content">
        <Timeline
          id="twitterdev"
          sourceType="profile"
          :options="{ tweetLimit: '10' }"
        />
      </div>
      <!-- <a class="twitter-timeline" data-width="100%" data-height="400" href="https://twitter.com/gamoutatsumi?ref_src=twsrc%5Etfw">Tweets by gamoutatsumi</a> <script async src="https://platform.twitter.com/widgets.js" charset="utf-8"></script> -->
    </div>
  </div>
</template>

<script>
// 現状ここは無視でいいよ
import announcements from "@/assets/announcements.json";
import { Timeline } from "vue-tweet-embed";
export default {
  components: {
    Timeline
  },
  data: function() {
    return {
      announcements: announcements
    };
  }
};
</script>

<style scoped>
/* ここにCSS書いてね */

#announce {
  padding: 1rem;
}

.Container {
  display: flex;
  justify-content: space-around;
}

.annouce-list {
  display: flex;
  height: 3rem;
  align-items: center;
  border: 1px solid;
}
.annouce-list > p:nth-child(1) {
  flex: 1;
  text-align: center;
  height: 100%;
  display: flex;
  align-items: center;
  justify-content: center;
  border-right: 1px solid;
}
.annouce-list > p:nth-child(2) {
  flex: 7;
  padding: 0 0.5rem;
}
.annouce-list > p:nth-child(3) {
  flex: 3;
  text-align: center;
  height: 100%;
  display: flex;
  align-items: center;
  justify-content: center;
  border-left: 1px solid;
}

.content {
  flex: 3;
  margin: 0;
}

.TwitterContainer {
  flex: 1;
  height: 80vh;
  overflow-y: auto;
}

.announceTitle {
  text-align: center;
  color: #55aaff;
  margin: 1rem 0;
}

@media screen and (max-width: 960px) {
  .Container {
    flex-direction: column;
  }
  .content {
    margin: 1rem 0;
  }
}

</style>
