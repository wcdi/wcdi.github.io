<template>
  <section class="container">
    <div>
      <HeaderNavBar/>
      <TheHeroSection/>
      <TheExplanationSection/>
      <TheAnnounceSection/>
      <TheAccessSection/>
      <TheContactSection/>
      <Footer/>
    </div>
  </section>
</template>

<script>
  import Footer from "~/components/Footer.vue";
  import HeaderNavBar from "~/components/HeaderNavBar.vue";
  import TheAccessSection from "~/components/TheAccessSection";
  import TheAnnounceSection from "~/components/TheAnnounceSection.vue";
  import TheContactSection from "~/components/TheContactSection.vue";
  import TheExplanationSection from "~/components/TheExplanationSection.vue";
  import TheHeroSection from "~/components/TheHeroSection";


  export default {
    components: {
      TheAnnounceSection,
      TheAccessSection,
      TheHeroSection,
      TheExplanationSection,
      TheContactSection,
      Footer,
      HeaderNavBar
    }
  };
</script>

<style></style>
