<template>
  <section class="top-section top-image">
    <div class="top-title">
      ITRC
    </div>
    <ul class="top-ul">
      <li class="top-li">
        <div><span class="top-span information">I</span>nformation</div>
      </li>
      <li class="top-li">
        <div><span class="top-span technology">T</span>echnology</div>
      </li>
      <li class="top-li">
        <div><span class="top-span research">R</span>esearch</div>
      </li>
      <li class="top-li">
        <div><span class="top-span">C</span>lub</div>
      </li>
    </ul>
  </section>
</template>

<script>
// 現状ここは無視でいいよ
export default {};
</script>



<style>
.top-image {
  background-image: url(../static/wcdi-top1.jpg);
  background-repeat: no-repeat;
  background-size: cover;
  background-position: center top;
  background-color: #2b2b2b;
  background-blend-mode: soft-light;
}

.top-section {
  display: flex;
  justify-content: space-around;
}

.top-title {
  font-size: 12rem;
  padding: 1rem;
  margin: 1rem 0 0 5rem;
  color: #FFFFFF;
}

.top-ul {
  list-style: none;
  display: flex;
  flex-direction: column;
  font-size: 4rem;
  margin: 6rem 0;
  padding: 40px;
}

.top-li {
  color: #FFFFFF;
}

.top-span {
  color: #F80C0C;
  margin-right: 0.5rem;
}

.information {
  margin-left: 0.6rem;
}

.technology {
  margin-left: 0.2rem;
}

.research {
  margin-left: 0.2rem;
}

@media screen and (max-width: 1000px) {
  .top-section {
    flex-direction: column;
    align-items: center;
    align-content: space-around;
  }
  .top-title {
    font-size: 6.5rem;
    margin: 0;
    padding: 0;
  }
  .top-ul {
    font-size: 2rem;
    margin: 0 0 1.55rem 0;
    padding: 0;
  }
  .information {
    margin-left: 0.3rem;
  }
  .technology {
    margin-left: 0.1rem;
  }
  .research {
    margin-left: 0.1rem;
  }
}
</style>