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
            class="d-block form-control py-3 my-3"
            type="text"
            placeholder="First Name"
          />
          <label class="d-block text-light text-capitalize mt-3"
            >last name *</label
          >
          <input
            class="d-block form-control py-3 my-3"
            type="text"
            placeholder="Last Name"
          />

          <label class="d-block text-light text-capitalize my-3">phone *</label>

          <vue-tel-input
            v-model="phone"
            mode="international"
            class="border-0"
          ></vue-tel-input>

          <label class="d-block text-light text-capitalize mt-3">email *</label>
          <input
            class="d-block form-control py-3 my-3"
            type="text"
            placeholder="Please Double Check Your Email"
          />
          <label class="d-block text-light text-capitalize mt-3"
            >Insurance Provider *</label
          >
          <input
            class="d-block form-control py-3 my-3"
            type="text"
            placeholder="Insurance Provider"
          />
          <label class="d-block text-light text-capitalize mt-3">
            how can we help you? *
          </label>
          <textarea class="form-control my-3" rows="3"></textarea>
          <div
            class="btn git-in-touch text-uppercase text-light fw-bold py-2 mb-2"
          >
            get in touch !
          </div>
        </div>
      </div>
    </div>
  </section>
</template>
<script>
import { ref } from "vue";
import { VueTelInput } from "vue-tel-input";
import "vue-tel-input/dist/vue-tel-input.css";
export default {
  name: "ContactUs",
  components: {
    VueTelInput,
  },
  setup() {
    const phone = ref(null);
    return {
      phone,
    };
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