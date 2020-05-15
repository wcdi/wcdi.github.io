<template>
  <nav id="navbar navbar-defalut wrapper">
    <link href="https://fonts.googleapis.com/icon?family=Material+Icons" rel="stylesheet">
    <ul id="headerLists">
      <li class="headerList">
        <a href="/" class="headerText" id="top"><i class="material-icons">home</i> Top</a>
      </li>
      <li class="headerList marginLeft">
        <a href="/" class="headerText" id="explanation"><i class="material-icons">computer</i> ITRCとは</a>
      </li>
      <li class="headerList marginLeft">
        <a href="/" class="headerText" id="news"><i class="material-icons">volume_up</i> お知らせ</a>
      </li>
      <li class="headerList marginLeft">
        <a href="/" class="headerText" id="access"><i class="material-icons">location_on</i> アクセス</a>
      </li>
      <li class="headerList marginLeft" id="marginRight">
        <a href="/" class="headerText" id="address"><i class="material-icons">contact_mail</i> 連絡先</a>
      </li>
    </ul>
  </nav>
</template>

<script>
// 現状ここは無視でいいよ
export default {};
</script>

<style>
@charset "UTF-8";

@font-face {
    font-family: 'Material Icons';
    font-style: normal;
    font-weight: 400;
    src: url(https://example.com/MaterialIcons-Regular.eot); /* For IE6-8 */
    src: local('Material Icons'),
        local('MaterialIcons-Regular'),
        url(https://example.com/MaterialIcons-Regular.woff2) format('woff2'),
        url(https://example.com/MaterialIcons-Regular.woff) format('woff'),
        url(https://example.com/MaterialIcons-Regular.ttf) format('truetype');
}

.material-icons {
    font-family: 'Material Icons';
    font-weight: normal;
    font-style: normal;
    font-size: 24px;  /* Preferred icon size */
    display: inline-block;
    line-height: 1;
    text-transform: none;
    letter-spacing: normal;
    word-wrap: normal;
    white-space: nowrap;
    direction: ltr;
    /* Support for all WebKit browsers. */
    -webkit-font-smoothing: antialiased;
    /* Support for Safari and Chrome. */
    text-rendering: optimizeLegibility;
    /* Support for Firefox. */
    -moz-osx-font-smoothing: grayscale;
    /* Support for IE. */
    font-feature-settings: 'liga';
}

.material-icons {
  
}

nav {
  width: auto;
  height: 81px;
  background: #201D1D;
}

#headerLists {
  list-style: none;
  display: flex;
  justify-content: center;
  font-size: 1.25rem;
  text-transform: uppercase;
}


.marginLeft {
  margin-left: 36px;
}

#marginRight {
  margin-right: 40px;
}

.headerList {
  margin-top: 15px;
  padding: 10px;
}

.headerText {
  color: white;
  text-decoration: none;
}

.material-icons {
  display: flex;
  justify-content: space-between;
}

.wrapper {
  max-width: 1440px;
  margin: 0 auto;
  padding: 0 4%;
}
</style>