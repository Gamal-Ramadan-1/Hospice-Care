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
        <div class="col-lg-6 col-md-6 col-sm-12">
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
        <div class="col-lg-6 col-md-6 col-sm-12">
          <h4 class="text-light text-capitalize">
            Contact Us to start hospice care
          </h4>
          <label class="d-block text-light text-capitalize mt-3"
            >first name *</label
          >
          <input
            class="d-block form-control py-3 mt-3 first-name"
            type="text"
            placeholder="First Name"
          />
          <p class="text-capitalize text-danger m-0 first-name">
            <i class="fa-solid fa-circle-exclamation"></i>
            first name requird...
          </p>

          <p class="text-capitalize text-danger m-0 first-name-correct">
            <i class="fa-solid fa-circle-exclamation"></i>
            enter your first name correctly
          </p>

          <label class="d-block text-light text-capitalize mt-3"
            >last name *</label
          >
          <input
            class="d-block form-control py-3 mt-3 last-name"
            type="text"
            placeholder="Last Name"
          />
          <p class="text-capitalize text-danger m-0 last-name">
            <i class="fa-solid fa-circle-exclamation"></i>
            last name requird...
          </p>

          <p class="text-capitalize text-danger m-0 last-name-correct">
            <i class="fa-solid fa-circle-exclamation"></i>
            enter your last name correctly
          </p>

          <label class="d-block text-light text-capitalize mt-3">phone *</label>
          <vue-tel-input
            v-model="phone"
            mode="international"
            class="border-0 chose-number"
          ></vue-tel-input>
          <label class="d-block text-light text-capitalize mt-3">
            email *
          </label>
          <input
            class="d-block form-control py-3 mt-3 email"
            type="text"
            placeholder="Please Double Check Your Email"
          />
          <p class="text-capitalize text-danger m-0 email">
            <i class="fa-solid fa-circle-exclamation"></i>
            email requird...
          </p>

          <p class="text-capitalize text-danger m-0 email-correct">
            <i class="fa-solid fa-circle-exclamation"></i>
            enter your email corectly
          </p>

          <label class="d-block text-light text-capitalize mt-3"
            >Insurance Provider *</label
          >
          <input
            class="d-block form-control py-3 mt-3 insurance-provider"
            type="text"
            placeholder="Insurance Provider"
          />
          <p class="text-capitalize text-danger m-0 insurance-provider">
            <i class="fa-solid fa-circle-exclamation"></i>
            Insurance Provider requird...
          </p>

          <p class="text-capitalize text-danger m-0 insurance-provider-correct">
            <i class="fa-solid fa-circle-exclamation"></i>
            enter your insurance provider corectly
          </p>

          <label class="d-block text-light text-capitalize mt-3">
            how can we help you? *
          </label>
          <textarea class="form-control mt-3" rows="3"></textarea>
          <p class="text-capitalize text-danger m-0 message">
            <i class="fa-solid fa-circle-exclamation"></i>
            how can we help you? requird...
          </p>
          <p class="text-capitalize text-danger m-0 donnot-space">
            <i class="fa-solid fa-circle-exclamation"></i>
            don't inter space
          </p>

          <div
            class="btn git-in-touch text-uppercase text-light fw-bold py-2 mt-4"
            @click="GitInTouch()"
          >
            get in touch !
          </div>
        </div>
      </div>
    </div>
  </section>
</template>
<script>
import { onMounted, ref } from "vue";
import { VueTelInput } from "vue-tel-input";
import "vue-tel-input/dist/vue-tel-input.css";
export default {
  name: "ContactUs",
  components: {
    VueTelInput,
  },
  setup() {
    onMounted(() => {
      $(".first-name").hide();
      $(".last-name").hide();
      $(".phone").hide();
      $(".email").hide();
      $(".insurance-provider").hide();
      $(".message").hide();

      $(".first-name-correct").hide();
      $(".last-name-correct").hide();
      $(".phone-correct").hide();
      $(".email-correct").hide();
      $(".insurance-provider-correct").hide();
      $(".donnot-space").hide();
    });
    const phone = ref(null);
    return {
      phone,
    };
  },
  methods: {
    GitInTouch() {
      if ($("input.first-name").val() === "") {
        $("p.first-name").show();
        $("p.first-name-correct").hide();
      } else if ($("input.first-name").val() === " ") {
        $("p.first-name").hide();
        $("p.first-name-correct").show();
      } else {
        $("p.first-name").hide();
        $("p.first-name-correct").hide();
      }

      if ($("input.last-name").val() === "") {
        $("p.last-name").show();
        $("p.last-name-correct").hide();
      } else if ($("input.last-name").val() === " ") {
        $("p.last-name").hide();
        $("p.last-name-correct").show();
      } else {
        $("p.last-name").hide();
        $("p.last-name-correct").hide();
      }

      if ($("input.email").val() === "") {
        $("p.email").show();
        $("p.email-correct").hide();
      } else if ($("input.email").val() === " ") {
        $("p.email").hide();
        $("p.email-correct").show();
      } else {
        $("p.email").hide();
        $("p.email-correct").hide();
      }

      if ($("input.insurance-provider").val() === "") {
        $("p.insurance-provider").show();
        $("p.insurance-provider-correct").hide();
      } else if ($("input.insurance-provider").val() === " ") {
        $("p.insurance-provider").hide();
        $("p.insurance-provider-correct").show();
      } else {
        $("p.insurance-provider").hide();
        $("p.insurance-provider-correct").hide();
      }

      if ($("textarea").val() === "") {
        $("p.message").show();
        $("p.donnot-space").hide();
      } else if ($("textarea").val() === " ") {
        $("p.message").hide();
        $("p.donnot-space").show();
      } else {
        $("p.message").hide();
        $("p.donnot-space").hide();
      }
    },
  },
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
  input,
  textarea {
    width: 60%;
    transition: all 0.3s ease-in-out;
  }
  input:focus,
  textarea:focus {
    background-color: rgb(243, 242, 242);
    outline: none;
    box-shadow: none;
    border-color: transparent;
    transition: all 0.3s ease-in-out;
  }
  .git-in-touch {
    width: 60%;
    background-color: $Main-Color;
  }
}
.vue-tel-input {
  width: 60%;
  background-color: white;
  padding: 13px 10px;
  border-radius: 8px;
  transition: all 0.3s ease-in-out;
}

@media only screen and (max-width: 768px) {
  input,
  textarea,
  .vue-tel-input,
  .git-in-touch {
    width: 80% !important;
  }
}
@media only screen and (max-width: 426px) {
  input,
  textarea,
  .vue-tel-input,
  .git-in-touch {
    width: 100% !important;
  }
}
</style>