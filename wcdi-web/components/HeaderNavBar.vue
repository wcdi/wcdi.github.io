<template>
  <header class="header-background sp-container">
    <nav>
      <ul class="header-ul">
        <li class="header-li">
          <nuxt-link to="/" class="header-text">
            <i class="material-icons fixed-icons">home</i> TOP
          </nuxt-link>
        </li>
        <li class="header-li margin-left">
          <nuxt-link to="/about" class="header-text">
            <i class="material-icons fixed-icons">computer</i> About Us
          </nuxt-link>
        </li>
        <li class="header-li margin-left">
          <nuxt-link to="member" class="header-text">
            <i class="material-icons fixed-icons">group</i> メンバー
          </nuxt-link>
        </li>
        <li class="header-li margin-left margin-right">
          <nuxt-link to="activity" class="header-text">
            <i class="material-icons fixed-icons">pets</i> 活動ログ
          </nuxt-link>
        </li>
      </ul>
      <div class="nav-drawer">
        <input id="nav-input" type="checkbox" class="nav-unshown" />
        <label id="nav-open" for="nav-input">
          <span>
            <i class="material-icons hamburger-menu">menu</i>
          </span>
        </label>
        <label class="nav-unshown" id="nav-close" for="nav-input"></label>
        <div id="nav-content">
          <ul class="header-mobile-ul">
            <li class="header-li">
              <nuxt-link to="/" class="header-text">
                <i class="material-icons fixed-icons">home</i> TOP
              </nuxt-link>
            </li>
            <li class="header-li">
              <nuxt-link to="/about" class="header-text">
                <i class="material-icons fixed-icons">computer</i> About Us
              </nuxt-link>
            </li>
            <li class="header-li">
              <nuxt-link to="/member" class="header-text">
                <i class="material-icons fixed-icons">group</i> メンバー
              </nuxt-link>
            </li>
            <li class="header-li">
              <nuxt-link to="/activity" class="header-text">
                <i class="material-icons fixed-icons">pets</i> 活動ログ
              </nuxt-link>
            </li>
          </ul>
        </div>
      </div>
    </nav>
  </header>
</template>

<script>
// 現状ここは無視でいいよ
export default {
  head: {
    link: [
      { rel: 'stylesheet', href: 'https://fonts.googleapis.com/icon?family=Material+Icons' }
    ]
  }
};
</script>

<style scoped>

.fixed-icons {
  display: inline-flex;
  vertical-align: text-bottom;
}

.header-background {
  height: 81px;
  background: #201d1d;
}

.header-ul {
  list-style: none;
  display: flex;
  justify-content: center;
  font-size: 1.25rem;
}

.header-li {
  margin-top: 16px;
  padding: 12px;
}

.header-text {
  color: #ffffff;
  text-decoration: none;
  display: flex;
  align-items: center;
  transition: 400ms ease all;
  text-decoration: none;
  position: relative;
  display: inline-block;
  text-decoration: none;
}
.header-text::after {
  position: absolute;
  bottom: -4px;
  left: 0;
  content: "";
  width: 100%;
  height: 2px;
  background: rgb(221, 220, 220);
  transform: scale(0, 1);
  transform-origin: left top;
  transition: transform 0.3s;
}
.header-text:hover::after {
  transform: scale(1, 1);
}


.header-text > i {
  margin-right: 0.5rem;
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
  .sp-container {
    position: fixed;
    width: 100%;
    z-index: 999;
  }
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
  .hamburger-menu #nav-open span,
  #nav-open span:before,
  #nav-open span:after {
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
    transition: 0.3s ease-in-out;
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
    background-color: #201d1d;
    transition: 0.3s ease-in-out;
    -webkit-transform: translateX(105%);
    transform: translateX(105%);
  }
  #nav-input:checked ~ #nav-close {
    display: block;
    opacity: 0.5;
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
