<template>
  <section>
    <div class="container">
      <div class="row">
        <div class="col-12 text-center">
          <h1 class="text-light pt-4 header">
            Get The Most Comfortable & Compassionate Care
            <span class="d-lg-block d-inline">
              That You & Your Loved Ones Deserve</span
            >
          </h1>
          <img
            src="@/Imgs/68fdcfd8-6343-4cc8-ae00-d76515003c1b.png"
            class="py-2 img-fluid"
          />
          <div class="line"></div>
        </div>
      </div>
    </div>
  </section>
</template>
<script>
export default {
  name: "ComfortableCare",
};
</script>
<style lang="scss" scoped>
@import "@/Scss/Main.scss";
section {
  background-color: $Main-Color;
  .header {
    font-size: 45px;
    font-weight: 600;
  }
  .line {
    width: 10%;
    height: 2px;
    background-color: transparent;
    border-top: 1px solid #eee;
    margin: 5px auto;
  }
}
</style>