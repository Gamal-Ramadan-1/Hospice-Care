<template>
  <Header />
  <ContactUs />
  <ComfortableCare />
  <OrchidHospice />
  <OurServeces />
</template>

<script>
import OrchidHospice from "./components/InformationAboutUs/InfosUs.vue";
import ComfortableCare from "./components/ComfortableCare/ComfortableCare.vue";
import ContactUs from "./components/ContactUs/ContactUs.vue";
import Header from "./components/Header/Header.vue";
import OurServeces from "./components/OurServeces/OurServeces.vue";
export default {
  components: { Header, ContactUs, ComfortableCare, OrchidHospice, OurServeces },
  name: "App",
};
</script>

<style lang="scss">

</style>
