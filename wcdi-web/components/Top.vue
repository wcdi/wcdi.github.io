<template>
  <section id="topText" class="topImage">
    <div id="topTitleText">
      ITRC
    </div>
    <ul id="topExplanationBox">
      <li>
        <div class="topExplanation" id="topInformation"><span id="topSpan">I</span>nformation</div>
      </li>
      <li>
        <div class="topExplanation" id="topTechnology"><span id="topSpan">T</span>echnology</div>
      </li>
      <li>
        <div class="topExplanation" id="topResearch"><span id="topSpan">R</span>esearch</div>
      </li>
      <li>
        <div class="topExplanation" id="topClub"><span id="topSpan">C</span>lub</div>
      </li>
    </ul>
  </section>
</template>

<script>
// 現状ここは無視でいいよ
export default {};
</script>



<style>
.topImage {
  background-image: url(../static/wcdi-top1-before.jpg);
  background-repeat: no-repeat;
  background-size: cover;
  background-color: #2b2b2b;
  background-blend-mode: soft-light;
}

#topText {
  display: flex;
  justify-content: space-around;
}

#topTitleText {
  font-size: 12rem;
  padding: 1rem;
  margin: 1rem 0 0 5rem;
  color: #FFFFFF;
}

#topExplanationBox {
  list-style: none;
  display: flex;
  flex-direction: column;
  font-size: 4rem;
  margin: 12rem 1rem 4rem 0;
}

.topExplanation {
  color: #FFFFFF;
}

#topSpan {
  color: #F80C0C;
  margin-right: 0.5rem;
}
</style>