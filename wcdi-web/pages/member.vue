<template>
  <div>
    <Header pageTitle="メンバー"></Header>
    <div class="Container">
      <h2 class="title">メンバー一覧</h2>
      <p class="backtotop">Top→</p>
    </div>
  </div>
</template>

<script>
  import Header from '../components/Header';
  export default {
    name: "member",
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
</style>
