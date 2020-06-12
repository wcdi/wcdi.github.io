<template>
  <!-- ここにHTML書いてね -->
  <div class="SectionContainer">
    <h2 class="SectionTitle">アクセス</h2>
    <div class="AccessContents">
        <div class="MapContents MediaQuery">
          <div class="MapItem">
            <h3 class="ContentsIndex">MAP</h3>
            <div class="ImageContent">
              <img src="../static/schoolMap.png" alt="サークル棟の場所"/>
            </div>
          </div>
          <div class="TextItem">
            <h3 class="ContentsIndex">活動時間</h3>
            <div class="TextDetail">
              <p>平日：17:00~19:00</p>
              <p>学校がある日は基本的に活動しています</p>
            </div>
          </div>
        </div>
        <div class="RoomContents MediaQuery">
          <div class="TextItem">
            <h3 class="ContentsIndex">活動場所</h3>
            <div class="TextDetail">
              <p>サークル棟 3階 304号室</p>
            </div>
          </div>
          <div class="RoomItem">
            <h3 class="ContentsIndex">部室</h3>
            <div class="ImageContent">
              <img src="../static/roomMap.png" alt="サークル部屋の場所"/>
            </div>
          </div>
        </div>
      </div>
    </div>
</template>

<script>
  // 現状ここは無視でいいよ
  export default {};
</script>


<style scoped>
  /* ここにCSS書いてね */

  /* moke */
  .AccessContainer > h2 {
    margin-bottom: 2rem;
  }

  .AccessContents {
    display: flex;
    flex-direction: column;
  }

  .MapItem {
    width: 50%;
    display: flex;
    align-items: center;
    flex-direction: column;
  }

  .TextItem {
    width: 50%;
    display: flex;
    text-align: center;
    align-items: center;
    flex-direction: column;
  }

  .RoomItem {
    width: 50%;
    display: flex;
    align-items: center;
    flex-direction: column;
  }

  .ImageContent > img {
    width: 100%;
    height: auto;
  }

  .TextDetail {
    height: 100%;
    width: 100%;
    display: flex;
    flex-direction: column;
    justify-content: center;
    border-bottom: 2px solid #2b2b2b;
  }

  .RoomContents {
    margin-top: 4rem;
  }

  .MapItem > h3 {
    margin-bottom: 1rem;
  }

  .TextItem > h3 {
    margin-bottom: 1rem;
  }

  .RoomItem > h3 {
    margin-bottom: 1rem;
  }

  .MediaQuery {
    display: flex;
    justify-content: center;
  }

  .ContentsIndex {
    font-size: 22px;
  }

  @media screen and (max-width: 1000px) {
    .MediaQuery {
      flex-direction: column;
      align-items: center;
    }

    .TextDetail {
      padding: 0 0 1rem 0;
    }

    .TextItem {
      order: 2;
      margin-top: 1rem;
      width: 100%;
    }

    .MapItem {
      width: 100%;
    }

    .RoomItem {
      width: 100%;
    }
  }

  @media screen and (min-width: 1001px) {
    .AccessContents {
      width: 1000px;
      margin-left: auto;
      margin-right: auto;
    }
  }

  /* nanoka css */

  /*  .access {
      width: 100%;
      color: #f7f8fb;
      background-color: #1d3156;
      padding-top: 1em;
      padding-bottom: 1em;
      text-align: center;
    }

    @media screen and (min-width: 880px) {
      .contents {
        margin: 2em auto 1em;
        width: 60%;
        display: flex;
        justify-content: center;
      }
    }

    .item {
      width: 50%;
      border-bottom: #f7f8fb solid 2px;
      height: auto;
    }

    .text {
      margin-top: 4em;
    }

    @media screen and (max-width: 880px) {
      .contents {
        margin: 2em auto 1em;
        width: 80%;
      }
    }*/
</style>
