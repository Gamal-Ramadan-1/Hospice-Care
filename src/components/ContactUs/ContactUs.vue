<template>
  <section>
    <div class="layout"></div>
    <div class="container">
      <div class="row">
        <h1 class="text-light text-md-center py-5">
          #1 Hospice Care Provider in the Greater Houston Area
        </h1>
      </div>
      <div class="row gy-4 py-4">
        <div class="col-lg-6">
          <h2>
            <i class="fa-solid fa-check"></i>
            No Cost To You, $0 Out of Pocket
          </h2>
          <h2>
            <i class="fa-solid fa-check"></i>
            Focused on Quality & Comfort
          </h2>
          <h2>
            <i class="fa-solid fa-check"></i>
            Complete, Experienced End-Of-
            <span class="d-lg-block d-inline-block">
              Life Care Support Team
            </span>
          </h2>
          <h2>
            <i class="fa-solid fa-check"></i>
            In-Home Care By Medical Staff
          </h2>
          <h2>
            <i class="fa-solid fa-check"></i>
            24/7 Support
          </h2>
          <h2>
            <i class="fa-solid fa-check"></i>
            Covered By Most Insurances
          </h2>
          <h2 class="py-5">Don't Go Through Any Pain Alone</h2>
          <h2>
            Rest Easy As We're Here For You & Your Loved Ones During This
            Difficult Time
          </h2>
        </div>
        <div class="col-lg-6"></div>
      </div>
    </div>
  </section>
</template>
<script>
export default {
  name: "ContactUs",
};
</script>
<style lang="scss" scoped>
@import "@/Scss/Main.scss";
section {
  background-image: url("@/Imgs/5a203b3f-611e-4164-b2ba-7be12359e580.png");
  background-position: 70% 50%;
  background-attachment: fixed;
  background-size: cover;
  clear: both;
  object-fit: cover;
  position: relative;
  z-index: 0;
  .layout {
    position: absolute;
    z-index: -1;
    width: 100%;
    height: 100%;
    background-color: $Text-Color;
    opacity: 0.7;
  }
  h1,
  h2 {
    text-shadow: 0px 0px 2px black;
    color: white;
    i,
    svg {
      font-weight: bolder;
      font-size: 40px;
      color: $Main-Color;
    }
  }
}
</style>