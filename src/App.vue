<template>
  <Header />
  <ContactUs />
</template>

<script>
import ContactUs from "./components/ContactUs/ContactUs.vue";
import Header from "./components/Header/Header.vue";
export default {
  components: { Header, ContactUs },
  name: "App",
};
</script>

<style lang="scss">
</style>
