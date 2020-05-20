<template>
  <!-- ここにHTML書いてね -->
  <div id="announce">
    <h2 class="announceTitle">最新のお知らせ</h2>
    <div class="Container">
      <div class="content">
        <!-- <dl id="announce-list">
          <template v-for="announcement in announcements.slice().reverse()">
            <dt :key="`first-${announcement.id}`">{{ announcement.id }}</dt>
            <dd :key="`second-${announcement.id}`">{{ announcement.title }}</dd>
            <dd :key="`third-${announcement.id}`" id="announce-list-item-date">
              {{ announcement.date }}
            </dd>
          </template>
        </dl> -->
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

/* #announce {
  width: 100%;
  height: 100%;
  background-color: brown;
}

@media screen and (max-width: 959px){
#announce-container {
  font-size: 3vw;
  display: grid;
  grid-template-rows: 0.5fr 2fr 2fr;
  row-gap: 10px;
  margin-left: 50px;
  margin-right: 50px;
  grid-template-areas: 
  "title"
  "announcements"
  "twitter";
}
}

@media screen and (min-width: 960px) {
  #announce-container {
    grid-template-columns: 2fr 1fr;
    grid-template-areas: 
    "title title"
    "announcements twitter";
    column-gap: 20em;
    margin-left: 2em; 
    margin-right: 2em;
    display: grid;
  }
}

.twitter {
  background-color: #66ffee;
  grid-area: twitter;
}
#announce-list-block {
  background-color: #77eeff;
  grid-area: announcements;
  display: flex;
}

#announce-header {
  position: relative;
  display: flex;
  justify-content: center;
  align-items: center;
  color: #55aaff;
  grid-area: title;
}

#announce-list-header {
  text-align: center;
  background-color: blue;
}

dt {
	float: left;
	clear: left;
	margin-right: 0.5vw;
  margin-left: 0.5vw;
	width: 5vw;
  padding-top: 0.5ex;
  padding-bottom: 0.5ex;
}
dd {
  float: left;
  margin-left: 1vw;
  padding-top: 1vh;
  padding-bottom: 1vh;
}

#announce-list-item-date {
  float: right;
  margin-left: 1em;
  margin-right: 0.5em;
}

.aspectwrapper {
  position: relative;
}

.aspectwrapper:after {
  padding-top: 60%;
  display: block;
  content: "";
}

.aspectwrapper > .content{
position: absolute;
top: 0px;
left: 0px;
bottom: 0px;
right: 0px;
overflow: auto;
} */
</style>
