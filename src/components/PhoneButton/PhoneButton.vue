<template>
  <div :class="Color + ' btn py-3 px-4'">
    <i :class="Icon + ' me-1'"></i>
    {{ PhoneNumber }}
  </div>
</template>
<script>
export default {
  name: "PhoneButton",
  props: {
    PhoneNumber: String,
    Color: String,
    Icon: String
  },
};
</script>
<style lang="scss" scoped>
@import "@/Scss/Main.scss";

.btn {
  border: 3px solid $Text-Color !important;
  color: $Text-Color;
  font-weight: bolder;
  border-radius: 20px;
  font-size: 18px;
  animation: call 1.5s infinite;
}

.btn:hover,
.btn:active {
  border: 3px solid $Text-Color !important;
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