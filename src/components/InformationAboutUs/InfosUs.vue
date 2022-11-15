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
      <div
        class="
          row
          justify-content-center
          align-items-center
          mt-lg-2
          mb-lg-4
          mt-3
          gy-5
        "
      >
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
      <Head Text="why we're different" />
      <div class="row justify-content-center align-items-center gy-4 my-3">
        <div class="col-lg-4 col-md-6 col-sm-12">
          <div class="card text-center">
            <img src="@/Imgs/1d58d4da-62d8-4525-b76d-705ee20025ed.png" />
            <h2 class="text-uppercase py-2">Detail Oriented</h2>
            <p class="p-2">
              We provide in-home services that cater to our patients’ specific
              needs and offer a wide array of therapies to make this time as
              peaceful as possible.
            </p>
          </div>
        </div>
        <div class="col-lg-4 col-md-6 col-sm-12">
          <div class="card text-center">
            <img src="@/Imgs/009b08c3-1a7d-4d27-be43-d03a7194ec62.png" />
            <h2 class="text-uppercase py-2">COMPLETE CARE</h2>
            <p class="p-2">
              We provide in-home services that cater to our patients’ specific
              needs and offer a wide array of therapies to make this time as
              peaceful as possible.
            </p>
          </div>
        </div>
        <div class="col-lg-4 col-md-6 col-sm-12">
          <div class="card text-center">
            <img src="@/Imgs/1c20a021-8e24-4261-ba4f-ffef6a74aa47.png" />
            <h2 class="text-uppercase py-2">HERE FOR THE FAMILY</h2>
            <p class="p-2">
              We provide in-home services that cater to our patients’ specific
              needs and offer a wide array of therapies to make this time as
              peaceful as possible.
            </p>
          </div>
        </div>
      </div>
      <div class="text-center py-4">
        <div class="btn py-3 px-4">
          <i class="fa-solid fa-phone me-1"></i>
          (281)688-6783
        </div>
      </div>
    </div>
  </section>
</template>
<script>
import Head from "../HeadEachSection/Head.vue";
import PhoneButton from "../PhoneButton/PhoneButton.vue";

export default {
  name: "InfosUs",
  components: { Head, PhoneButton },
};
</script>
<style lang="scss" scoped>
@import "@/Scss/Main.scss";
section {
  h3 {
    font-weight: 400;
  }
  .card {
    background-color: $Main-Color;
    color: white;
    p{
      line-height: 1.7;
    }
    img {
      width: 280px;
      height: 200px;
      margin: 10px auto;
      border-radius: 10px;
    }
  }
}

@media only screen and (max-width: 1440px) {
  .card {
    img {
      width: 270px;
      height: 210px;
      margin: 10px auto;
      border-radius: 10px;
    }
  }
}

@media only screen and (max-width: 1025px) {
  .card {
    img {
      width: 250px;
      height: 200px;
      margin: 10px auto;
      border-radius: 10px;
    }
  }
}

.btn {
  border: 3px solid $Text-Color;
  font-weight: bolder;
  border-radius: 20px;
  color: $Text-Color;
  font-size: 18px;
  animation: call 1.5s infinite;
}
.btn:hover,
.btn:active {
  border: 3px solid $Text-Color;
}
@keyframes call {
  15% {
    transform: translate(0px, 0%);
  }
  35% {
    transform: translate(0px, -25%);
  }
  45% {
    transform: translate(0px, 0%);
  }
  55% {
    transform: translate(0px, -15%);
  }
  70% {
    transform: translate(0px, 0%);
  }
  80% {
    transform: translate(0px, -10%);
  }
  90% {
    transform: translate(0px, 0%);
  }
  95% {
    transform: translate(0px, -2%);
  }
  99% {
    transform: translate(0px, 0%);
  }
  100% {
    transform: translate(0px, 0%);
  }
}
</style>