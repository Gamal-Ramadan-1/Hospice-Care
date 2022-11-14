<template>
  <div class="row">
    <div class="col-12 text-center">
      <h1 class="mt-5 mb-3">{{ Text.toUpperCase() }}</h1>
      <div :class="LineColor + ' line'"></div>
    </div>
  </div>
</template>
<script>
export default {
  name: "Head",
  props: {
    Text: String,
    LineColor: String,
  },
};
</script>
<style lang="scss" scoped>
@import "@/Scss/Main.scss";
h1 {
  color: $Text-Color;
}
.line {
  width: 10%;
  border-top: 1px solid $Line-Head-Color;
  margin: 1px auto;
}
@media only screen and (max-width: 1440px) {
  h1 {
    font-size: 50px;
    font-weight: 600;
  }
}

@media only screen and (max-width: 426px) {
  h1 {
    font-size: 36px;
    font-weight: 600;
  }
}
</style>
