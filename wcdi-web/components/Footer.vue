<template>
  <!-- ここにHTML書いてね -->
  <footer>
    <div class="footer-content">
      <h2 class="footer-title">Sitemap & Links </h2>

    </div>
    <div class="footer-main">
      <div class="flex">
        <section class="footer-subcontent">
          <h2 class="footer-subtitle">Top</h2>
          <ul class="footer-tops">
            <li class="footer-top"><a href="/" class="link-decoration">ITRCとは</a></li>
            <li class="footer-top"><a href="/" class="link-decoration">お知らせ</a></li>
            <li class="footer-top"><a href="/" class="link-decoration">アクセス</a></li>
            <li class="footer-top"><a href="/" class="link-decoration">連絡先</a></li>
          </ul>
        </section>
        <section class="footer-subcontent">
          <h2 class="footer-subtitle">探索</h2>
          <ul class="footer-searches">
            <li class="footer-search"><a href="/" class="link-decoration">メンバー</a></li>
            <li class="footer-search"><a href="/" class="link-decoration">過去のお知らせ</a></li>
            <li class="footer-search"><a href="/" class="link-decoration">過去の活動ブログ</a></li>
            <li class="footer-search"><a href="/" class="link-decoration">連絡フォーム</a></li>
          </ul>
        </section>
        <section class="footer-subcontent">
          <h2 class="footer-subtitle">Links</h2>
          <ul class="footer-links">
            <li class="footer-link"><a href="/" class="link-decoration">twitter</a></li>
            <li class="footer-link"><a href="/" class="link-decoration">GitHub</a></li>
          </ul>
        </section>
      </div>
    </div>
  </footer>
</template>

<script>
// 現状ここは無視でいいよ
export default {};
</script>




<style>
/* ここにCSS書いてね */
footer {
  width: 100%;
 background-color: #5caceb;
}
.footer-content{
  margin: 20px auto;
  padding-top: 20px;
  text-align: center;
}
.flex {
  display: flex;
  flex-flow: row wrap;

}
.footer-main {
  margin: 
}
.footer-subcontent {
  margin: 0 auto;
  text-align: center;
}

.footer-tops, .footer-searches, .footer-links {
  padding-left: 0px;
  margin: 20px auto;
  list-style: none;
}

.footer-top > *:hover, .footer-link > *:hover, .footer-search > *:hover {
  border-bottom: 1px solid black;
}

.footer-top, .footer-link{
  margin-bottom: 10px;
  font-weight: bold;
}
.link-decoration {
  text-decoration: none;
  color: #E6E6E6;
}
.footer-search {
  margin-bottom: 20px;
  font-weight: bolder;
}



</style>