<template>
  <section class="top-image top-section">
    <div class="box">

      <p>{{ pageTitle }}</p>

    </div>
</section>
</template>

<script>
  export default {
    name: "Header",
    props: ['pageTitle']
  }
</script>

<style scoped>
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
.box{
  padding-top: 12rem;
  padding-bottom: 12rem;
}

.box p {
  top: 25%;
  left: 40%;
  font-size: 72px;
  font-weight: bold;
  color: #ffffff;
}

</style>
