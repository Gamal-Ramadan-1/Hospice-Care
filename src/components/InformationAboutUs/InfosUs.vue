<template>
  <section>
    <div class="container">
      <Head Text="about white orchid hospice" />
      <div class="row pb-5 mb-3">
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