<template>
  <Header />
  <ContactUs />
  <ComfortableCare />
</template>

<script>
import ComfortableCare from "./components/ComfortableCare/ComfortableCare.vue";
import ContactUs from "./components/ContactUs/ContactUs.vue";
import Header from "./components/Header/Header.vue";
export default {
  components: { Header, ContactUs, ComfortableCare },
  name: "App",
};
</script>

<style lang="scss">
</style>
