<template>
  <section class="container">
    <div>
      <Header />
      <Explanation />
      <Announce />
      <Access />
      <Contact />
      <Footer />
    </div>
  </section>
</template>

<script>
import Access from "~/components/Access.vue";
import Announce from "~/components/Announce.vue";
import Contact from "~/components/Contact.vue";
import Explanation from "~/components/Explanation.vue";
import Footer from "~/components/Footer.vue";
import Header from "~/components/Header.vue";

export default {
  components: {
    Access,
    Announce,
    Contact,
    Explanation,
    Footer,
    Header
  }
};
</script>

<style></style>
