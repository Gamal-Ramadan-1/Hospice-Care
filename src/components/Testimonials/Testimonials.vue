<template>
    <section>
        <div class="container">
            <div class="row">
                <div class="col-12">

                    <Head Text="Testimonials" />
                </div>
                <div class="col-12 text-center my-4">
                    <h3 class="text-dark">
                        It's Rewarding To Be Able To Help Patients & Their Families. See What Some Have To Say About Our
                        Compassionate Team & Care...

                    </h3>
                </div>
            </div>
            <div class="row justify-content-center align-items-center my-5 gy-4">
                <div class="col-lg-4 col-md-6 col-sm-12" v-for="Testimonial in Testimonials">
                    <div class="w-100">
                        <i class="fa-solid fa-quote-left mb-2"></i>
                    </div>
                    <div class="text-center">
                        <p>{{ Testimonial.Description }}</p>
                        <h3>{{ Testimonial.Name }}</h3>
                        <h4 class="fw-bold">Texas</h4>
                        <img src="@/Imgs/f9708100-c2e7-405e-a683-130f8252bb91.jpeg">
                    </div>
                </div>
            </div>
            <div class="text-center my-5">

                <PhoneButton PhoneNumber="(281)688-6783" Icon="fa-solid fa-phone" />
            </div>
        </div>
    </section>
</template>
<script>
import Head from '../HeadEachSection/Head.vue';
import PhoneButton from '../PhoneButton/PhoneButton.vue';

export default {
    components: { Head, PhoneButton },
    data() {
        return {
            Testimonials: [
                {
                    Description: 'Awesome patient care services, excellent staff and promptly responds to calls from patients and other people.',
                    Name: 'Ngozi Iroha'
                },
                {
                    Description: 'I enjoy working with this staff. They are compassionate and helpful—here to care for the patients!',
                    Name: 'Steve Jeavons'
                },
                {
                    Description: 'Great all-around people to work with fast simple and efficient. I will be reaching out to these guys again for sure!',
                    Name: 'Kumeh Emmet'
                },
                {
                    Description: 'Great staff, they went above and beyond for us. I am looking forward to doing business with again',
                    Name: 'Manny Kumeh'
                },
                {
                    Description: 'Will travel anywhere for patients, wherever they live!',
                    Name: 'Anthony Neubecker'
                },
                {
                    Description: 'PLEASE FEEL FREE TO SEND ME MORE like Rose she has been very helpful and answered all my questions and has been very kind to me in every way. Please dont let her get away, and Melissa my aide has also been very helpful with cleaning, laundry, and anything I have asked of her she has done and with diligence.',
                    Name: 'Jack Hinman'
                },
            ]
        }
    },
}
</script>
<style lang="scss" scoped>
@import "@/Scss/Main.scss";

section {

    i,
    svg {
        font-size: 40px;
        color: $Text-Color;
    }

    p {
        padding: 15px;
        border: 2px solid black;
        border-radius: 6px;
        font-style: italic;
    }

    h3 {
        font-weight: bolder;
        text-transform: capitalize;
        color: $Text-Color;
    }

    h4 {
        color: rgb(80, 79, 79);
    }

    img {
        width: 130px;
        object-fit: contain;
    }

    .btn:hover,
    .btn:active {
        border: 3px solid $Text-Color;
        color: $Text-Color;
    }
}
</style>