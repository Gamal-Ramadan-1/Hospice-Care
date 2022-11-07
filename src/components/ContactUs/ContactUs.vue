<template>
  <section>
    <div class="layout"></div>
    <div class="container">
      <div class="row">
        <h1 class="text-light text-center py-5">
          #1 Hospice Care Provider in the Greater Houston Area
        </h1>
      </div>
      <div class="row"></div>
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
  background-position: center center;
  background-attachment: fixed;
  background-size: cover;
  clear: both;
  object-fit: cover;
  height: 800px;
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
  h1{
    text-shadow: 0px 0px 2px black;
  }
}
</style>