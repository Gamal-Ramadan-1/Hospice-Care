<template>
  <Header />
  <ContactUs />
  <ComfortableCare />
  <OrchidHospice />
  <OurServeces />
  <Insurances />
  <Testimonials />
  <Footer />
</template>

<script>
import OrchidHospice from "./components/InformationAboutUs/InfosUs.vue";
import ComfortableCare from "./components/ComfortableCare/ComfortableCare.vue";
import ContactUs from "./components/ContactUs/ContactUs.vue";
import Header from "./components/Header/Header.vue";
import OurServeces from "./components/OurServeces/OurServeces.vue";
import Insurances from "./components/Insurances/Insurances.vue";
import Testimonials from "./components/Testimonials/Testimonials.vue";
import Footer from "./components/Footer/Footer.vue";
export default {
  components: { Header, ContactUs, ComfortableCare, OrchidHospice, OurServeces, Insurances, Testimonials, Footer },
  name: "App",
};
</script>

<style lang="scss">

</style>
