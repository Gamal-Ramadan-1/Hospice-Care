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
        <div class="col-12 pb-md-0 pb-5 mb-md-0 mb-3">
          <h3 class="my-3 text-light fw-bolder">
            We Understand the Pain You're Going Through:
          </h3>
          <h3
            v-for="info in infos"
            :key="info"
            class="d-flex align-items-md-center text-capitalize mb-4"
          >
            <i v-if="info.icon" class="fa-solid fa-xmark px-2 py-1 X-mark me-1 mt-md-0 mt-1"></i>
            <p class="text-light m-0">
              {{ info.discription }}
            </p>
          </h3>
          <div class="text-center my-5">
            <PhoneButton
              PhoneNumber="(281)688-6783"
              class="d-md-inline-block d-none"
              Color="text-light"
              Icon="fa-solid fa-phone"
            />
          </div>
        </div>
      </div>
    </div>
  </section>
</template>
<script>
import PhoneButton from "../PhoneButton/PhoneButton.vue";

export default {
  name: "ComfortableCare",
  data() {
    return {
      infos: [
        {
          icon: true,
          discription: "Dealing With The Emotional Burden Of A Loved One",
        },
        {
          icon: true,
          discription: "Lack Of Support & Care During This Tough Time",
        },
        {
          icon: true,
          discription: "Helping A Loved One With Their Pain",
        },
        {
          icon: true,
          discription: "Dealing With A Terminal Illness",
        },
        {
          icon: true,
          discription: "Expensive Cost of Healthcare",
        },
        {
          icon: true,
          discription: "Everything Else That is stressful...",
        },
        {
          icon: false,
          discription:
            "Don't worry. Rest easy and let our trusted team take care of everything.",
        },
        {
          icon: false,
          discription:
            "Get peace of mind with an end-of-life support team, pain management & symptom control, homemaking services, respite care, bereavement support, and spiritual support providers.",
        },
        {
          icon: false,
          discription:
            "At White Orchid Hospice, you can trust us to alleviate as much pain, worry, and inconvenience from your life as possible if you're faced with the realities of death, illness, and grief.",
        },
        {
          icon: false,
          discription:
            "At White Orchid Hospice, You Can Trust Us To Alleviate As Much Pain, Worry, And Inconvenience From Your Life As Possible If You're Faced With The Realities Of Death, Illness, And Grief.",
        },
      ],
    };
  },
  components: { PhoneButton },
};
</script>
<style lang="scss" scoped>
@import "@/Scss/Main.scss";
section {
  background-color: $Main-Color;
  .header {
    font-size: 44px;
    font-weight: 600;
  }
  .line {
    width: 10%;
    height: 2px;
    background-color: transparent;
    border-top: 1px solid #eee;
    margin: 5px auto;
  }
  .X-mark {
    background-color: white;
    border-radius: 5px;
    color: $Main-Color;
    font-size: 18px;
    font-weight: bolder;
  }
}
</style>