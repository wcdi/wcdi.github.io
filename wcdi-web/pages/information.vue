<template>
  <div>
    <Header pageTitle="Information"></Header>
    <div class="Container">
      <h2 class="title">お知らせ</h2>
      <div class="InformationContainer">
        <div>
          <h3>コミックマーケット98にサークル参加します</h3>
        </div>
        <div>
          <h3>hoge</h3>
        </div>
        <div>
          <h3>fuga</h3>
        </div>
      </div>
      <p class="backtotop">Top→</p>
    </div>
  </div>
</template>

<script>
  import Header from '../components/Header';
  export default {
    name: "information",
    components: {
      Header
    }
  }
</script>

<style scoped>
.Container {
  padding: 3vh 15vw;
  display: flex;
  flex-direction: column;
}
h2.title {
  border-bottom: solid 3px #006F87;
  display: inline-block;
  margin: 0 auto 0;
}
p {
  padding: 1.5vh 0;
}
.backtotop {
  font-weight: bold;
  margin-left: auto;
}
div.InformationContainer {
  display: flex;
  justify-content: space-between;
  flex-wrap: wrap;
  padding-top: 5vh;
}
</style>
