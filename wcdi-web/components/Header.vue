<template>
  <header class="header-background">
    <link href="https://fonts.googleapis.com/icon?family=Material+Icons" rel="stylesheet">
    <nav>
      <ul class="header-ul">
        <li class="header-li">
          <a href="#" class="header-text header-top"><i class="material-icons">home</i> Top</a>
        </li>
        <li class="header-li margin-left">
          <a href="#" class="header-text header-itrc"><i class="material-icons">computer</i> ITRCとは</a>
        </li>
        <li class="header-li margin-left">
          <a href="#" class="header-text header-news"><i class="material-icons">volume_up</i> お知らせ</a>
        </li>
        <li class="header-li margin-left">
          <a href="#" class="header-text header-access"><i class="material-icons">location_on</i> アクセス</a>
        </li>
        <li class="header-li margin-left margin-right">
          <a href="#" class="header-text header-form"><i class="material-icons">contact_mail</i> 連絡先</a>
        </li>
      </ul>
      <div class="nav-drawer">
        <input id="nav-input" type="checkbox" class="nav-unshown">
        <label id="nav-open" for="nav-input"><span><i class="material-icons humberger-menu">menu</i> </span></label>
        <label class="nav-unshown" id="nav-close" for="nav-input"></label>
        <div id="nav-content">
          <ul class="header-mobile-ul">
            <li class="header-li">
              <a href="#" class="header-text header-top"><i class="material-icons">home</i> Top</a>
            </li>
            <li class="header-li">
              <a href="#" class="header-text header-itrc"><i class="material-icons">computer</i> ITRCとは</a>
            </li>
            <li class="header-li">
              <a href="#" class="header-text header-news"><i class="material-icons">volume_up</i> お知らせ</a>
            </li>
            <li class="header-li">
              <a href="#" class="header-text header-access"><i class="material-icons">location_on</i> アクセス</a>
            </li>
            <li class="header-li">
              <a href="#" class="header-text header-form"><i class="material-icons">contact_mail</i> 連絡先</a>
            </li>
          </ul>
        </div>
      </div>
    </nav>
  </header>
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

.header-background {
  height: 81px;
  background: #201D1D;
}

.header-ul {
  list-style: none;
  display: flex;
  justify-content: center;
  font-size: 1.25rem;
  text-transform: uppercase;
}

.header-li {
  margin-top: 16px;
  padding: 12px;
}

.header-text {
  color: #ffffff;
  text-decoration: none;
}

.margin-left {
  margin-left: 36px;
}

.margin-right {
  margin-right: 40px;
}

.nav-drawer {
  display: none;
}

@media screen and (max-width: 1000px) {
  .header-ul {
    display: none;
  }
  .material-icons {
    color: #ffffff;
  }
  .nav-drawer {
    height: 81px;
    display: flex;
    justify-content: flex-end;
    align-items: center;
    margin-right: 1.5rem;
  }
  .nav-unshown {
    display: none;
  }
  #nav-open {
    display: inline-block;
    width: 30px;
    height: 22px;
    vertical-align: middle;
  }
  .humberger-menu #nav-open span, #nav-open span:before, #nav-open span:after {
    display: flex;
  }
  #nav-open span:before {
    bottom: -8px;
  }
  #nav-open span:after {
    bottom: -16px;
  }
  #nav-close {
    display: none;
    position: fixed;
    z-index: 99;
    top: 0;
    right: 0;
    width: 100%;
    height: 100%;
    background-color: #000000;
    opacity: 0;
    transition: .3s ease-in-out;
  }
  #nav-content {
    overflow: auto;
    position: fixed;
    top: 81px;
    right: 0;
    z-index: 9999;
    width: 90%;
    max-width: 59.2vw;
    height: 100%;
    background-color: #201D1D;
    transition: .3s ease-in-out;
    -webkit-transform: translateX(105%);
    transform: translateX(105%);
  }
  #nav-input:checked ~ #nav-close {
    display: block;
    opacity: .5;
  }
  #nav-input:checked ~ #nav-content {
    -webkit-transform: translateX(0%);
    transform: translateX(0%);
    box-shadow: 6px 0 25px #000000;
  }
  .header-mobile-ul {
    list-style: none;
    display: flex;
    flex-direction: column;
    font-size: 1.25rem;
    text-transform: uppercase;
    margin: 2rem 0 2rem 6rem;
    padding-right: 40px;
  }
}
@media screen and (max-width: 427px) {
  #nav-content {
    max-width: 66.5vw;
  }
  .header-mobile-ul {
    margin: 2rem 0 2rem 2rem;
  }
}
@media screen and (max-width: 376px) {
  #nav-content {
    max-width: 68.7vw;
  }
  .header-mobile-ul {
    margin: 2rem 0 2rem 1.5rem;
  }
}
@media screen and (max-width: 321px) {
  #nav-content {
    max-width: 72.1vw;
  }
  .header-mobile-ul {
    margin: 2rem 0 2rem 0.5rem;
  }
}
</style>