<template>
  <!-- ここにHTML書いてね -->
  <footer>
    <div class="SectionContainer">
      <div class="LogoContainer">
        <p class="FooterTitleItem">ITRC</p>
        <p class="SubTitleItem">情報技術研究部</p>
        <div class="IconsItem">
          <img src="../static/GitHub-Mark-Light-32px.png" alt="GitHub-icon">
          <img src="../static/Twitter_Social_Icon_Circle_White.svg" width="32" height="32" alt="Twitter-icon">
        </div>
      </div>
      <div class="LinksContainer">
        <div class="LinksBlock">
          <p class="LinksTitleItem">Home</p>
          <p class="LinkTextItem">情報技術研究部</p>
          <p class="LinkTextItem">最新のお知らせ</p>
          <p class="LinkTextItem">アクセス</p>
          <p class="LinkTextItem">コンタクト</p>
        </div>
        <div class="LinksBlock">
          <p class="LinksTitleItem">Contents</p>
          <p class="LinkTextItem">
            <NuxtLink to="/about">About Us</NuxtLink>
          </p>
          <p class="LinkTextItem">
            <NuxtLink to="/member">メンバー</NuxtLink>
          </p>
          <p class="LinkTextItem">
            <NuxtLink to="/activity">活動ログ</NuxtLink>
          </p>
        </div>
      </div>
    </div>
    <div class="CopyrightText">
      <small>Copyright &copy; ITRC 情報技術研究部 2020</small>
    </div>
  </footer>
</template>

<script>
  // 現状ここは無視でいいよ
  export default {};
</script>


<style scoped>
  /* ここにCSS書いてね */
  @font-face {
    font-family: 'Rationale';
    src: url(../assets/fonts/Rationale-Regular.ttf);
  }


/* ここにCSS書いてね */
  footer {
    width: 100%;
    background-color: #5a5a5a;
    padding: 2rem 0 1rem 0;
  }
  .footer-content {
    margin-bottom: 2rem;
    text-align: center;
  }
  .flex {
    display: flex;
    flex-flow: row wrap;
    margin-bottom: 1rem;
  }

  .footer-subcontent {
    margin: 0 auto;
    text-align: center;
  }

  .footer-title {
    font-size: 34px;
    font-weight: bold;
    color: #fff;
  }

  .footer-main {
    color: #fff;
  }

  .footer-tops,
  .footer-searches,
  .footer-links {
    padding-left: 0;
    margin: 20px auto;
    list-style: none;
  }

  .footer-top > *:hover,
  .footer-link > *:hover,
  .footer-search > *:hover {
    border-bottom: 1px solid black;
    padding-bottom: 3px;
  }

  .footer-top,
  .footer-link {
    margin-bottom: 16px;
    font-weight: bold;
  }
  .link-decoration {
    text-decoration: none;
    color: #e6e6e6;
  }
  .footer-search {
    margin-bottom: 20px;
    font-weight: bolder;
  }

  .footer-subtitle {
    font-size: 30px;
  }
  .SectionContainer {
    padding-top: 4rem;
    padding-bottom: 4rem;
    display: flex;
    flex-direction: row;
    color: #C4C4C4;
  }

  .LogoContainer {
    width: 50%;
    text-align: center;
    justify-content: center;
  }

  .LogoContainer > .FooterTitleItem {
    font-size: 4rem;
    font-family: 'Rationale', sans-serif;
    letter-spacing: 6px;
    width: 112px;
    margin-left: auto;
    margin-right: auto;
  }

  .LogoContainer > .SubTitleItem {
    font-size: 16px;
    width: 112px;
    margin-left: auto;
    margin-right: auto;
  }

  .LogoContainer > .IconsItem {
    margin-top: 1rem;
  }

  img {
    margin-left: 12px;
    margin-right: 12px;
  }

  .LinksContainer {
    width: 50%;
    display: flex;
    flex-direction: row;
    color: white;
  }

  .LinksBlock {
    margin-left: 20%;
  }

  .LinksTitleItem {
    font-size: 2rem;
    font-family: 'Rationale', sans-serif;
  }

  .LinkTextItem {
    margin-top: 1rem;
    font-size: 14px;
  }

  .LinkTextItem > a {
    color: white;
    text-decoration: none;
  }

  .CopyrightText {
    width: 100%;
    padding-top: 1rem;
    padding-bottom: 1rem;
    text-align: center;
    color: white;
  }

  @media screen and (max-width: 784px) {
    .SectionContainer {
      display: flex;
      flex-direction: column;
    }

    .LogoContainer {
      width: 100%;
    }

    .LinksContainer {
      margin-top: 2rem;
      width: 100%;
    }

    .LinksBlock {
      margin-left: auto;
      margin-right: auto;
    }
  }
</style>
