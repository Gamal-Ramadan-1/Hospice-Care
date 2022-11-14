<template>
  <section>
    <div class="container">
      <Head Text="about white orchid hospice" />
      <div class="row pb-2">
        <div class="col-lg-12">
          <h3 class="pt-3 pb-2">
            We are committed to the comfort and serenity of ALL patients.
          </h3>
          <h3 class="py-3">
            From the physical to the emotional and spiritual, we handle
            EVERYTHING involved in end of life care so our patients and their
            families don’t have do so themselves.
          </h3>
        </div>
      </div>
      <Head Text="what you can expect" />
      <div class="row justify-content-center align-items-center mt-lg-2 mt-3 gy-5">
        <div class="col-lg-4 col-md-6 col-sm-12 text-center">
          <img
            src="@/Imgs/location_Jp4vBwWWQJdspq8YagE9_images_5cfb2eb6-f0d9-40d7-a514-63c5db354e99.png"
            style="filter: grayscale(100%)"
          />
          <h3 class="mt-3">COMPLETE COMFORT</h3>
        </div>
        <div class="col-lg-4 col-md-6 col-sm-12 text-center">
          <img
            src="@/Imgs/location_Jp4vBwWWQJdspq8YagE9_images_1ba99a6e-b596-4206-b837-3005f3512f77.png"
            style="filter: grayscale(100%)"
          />
          <h3 class="mt-3">KINDNESS FROM ALL STAFF</h3>
        </div>
        <div class="col-lg-4 col-md-6 col-sm-12 text-center">
          <img
            src="@/Imgs/location_Jp4vBwWWQJdspq8YagE9_images_fde222ab-9a7a-4bf4-b024-01758716c8a3.png"
            style="filter: grayscale(100%)"
          />
          <h3 class="mt-3">NOURISHMENT</h3>
        </div>
      </div>
    </div>
  </section>
</template>
<script>
import Head from "../HeadEachSection/Head.vue";

export default {
  name: "InfosUs",
  components: { Head },
};
</script>
<style lang="scss" scoped>
@import "@/Scss/Main.scss";
section {
  h3 {
    font-weight: 400;
  }
}
</style>