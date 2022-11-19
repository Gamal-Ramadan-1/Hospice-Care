<template>
  <section class="header">
    <div class="container">
      <div class="row">
        <div class="col-lg-6 col-md-6 col-sm-12 text-md-start text-center">
          <a href="#">
            <img src="@/Imgs/98958a1d-7255-435d-a2b6-bf79c6ed1797.png" class="py-4" />
          </a>
        </div>
        <div class="col-lg-6 col-md-6 col-sm-12 text-md-end text-center">
          <div class="py-4">
            <PhoneButton PhoneNumber="(281)688-6783" Color="text-light" Icon="fa-solid fa-phone" />
          </div>
        </div>
      </div>
    </div>
  </section>
</template>
<script>
import PhoneButton from "../PhoneButton/PhoneButton.vue";

export default {
  name: "Header",
  components: { PhoneButton },
};
</script>
<style lang="scss" scoped>
@import "@/Scss/Main.scss";

.header {
  background-color: $Main-Color;

  img {
    object-fit: cover;
  }
}

@media only screen and (max-width: 768px) {
  img {
    width: 100%;
  }
}
</style>