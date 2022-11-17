<template>
    <section class="pb-4 mt-5">
        <div class="container">
            <div class="row header">
                <div class="col-12">

                    <Head Text="FULL SERVICE HOSPICE CARE" LineColor="border-light" />
                </div>
                <div class="col-12 text-center">
                    <p class="text-light pt-4">Providing Personalized, Intentional Care Curated to Every Patient and
                        Family’s Distinctive <span class="d-lg-block d-inline-block">Set of Needs:</span>
                    </p>
                </div>
            </div>
            <div class="row gy-4 content mt-4">
                <div class="col-lg-4 col-md-6 col-sm-12 text-center text-light" v-for="Service in Services">
                    <img :src="require(`@/Imgs/${Service.ImgSrc}`)">
                    <h4 class="py-3 text-uppercase">{{ Service.Header }}</h4>
                    <p class="py-1 text-capitalize">{{ Service.Descrption }}</p>
                </div>
                <div class="text-center py-4">
                    <PhoneButton PhoneNumber="(281)688-6783" />
                </div>
            </div>
        </div>
    </section>
</template>
<script>
import Head from '../HeadEachSection/Head.vue';
import PhoneButton from '../PhoneButton/PhoneButton.vue';

export default {
    name: "OurServeces",
    components: { Head, PhoneButton },
    data() {
        return {
            Services: [
                {
                    ImgSrc: 'location_Jp4vBwWWQJdspq8YagE9_images_8d6a83cf-7f30-487c-bd44-7bf28ddd5d6c.png',
                    Header: 'WIDE SPECTRUM OF THERAPY',
                    Descrption: 'Physical therapy, respiratory therapy, occupational therapy, and music therapy'
                },
                {
                    ImgSrc: 'location_Jp4vBwWWQJdspq8YagE9_images_977f2275-843e-493d-91b3-ac86e81c1d62.png',
                    Header: 'PHYSICAL COMFORT',
                    Descrption: 'Pain treatment is given so patients can be emotionally and spiritually present.'
                },
                {
                    ImgSrc: 'location_Jp4vBwWWQJdspq8YagE9_images_69f4f4cb-8555-472d-9e0e-afe539064d39.png',
                    Header: 'EMOTIONAL AND SPIRITUAL CARE',
                    Descrption: 'Get the emotional and spiritual support you need to get through this difficult time.'
                },
                {
                    ImgSrc: 'location_Jp4vBwWWQJdspq8YagE9_images_9c865477-382d-46d7-8caa-0e3c47125b4a.png',
                    Header: 'IN-HOME CARE',
                    Descrption: 'We wll make arrangements to come to serve patients in the comfort of their own home.'
                },
                {
                    ImgSrc: 'location_Jp4vBwWWQJdspq8YagE9_images_638c6cdd-63ad-4596-8b90-bc8a5d5cbbad.png',
                    Header: 'Medical Staff ON-CALL',
                    Descrption: 'Fully licensed staff is available 24/7'
                },
                {
                    ImgSrc: 'location_Jp4vBwWWQJdspq8YagE9_images_b452c491-def7-4e72-97cb-3c1d31643d52.png',
                    Header: 'EXPERT PHYSICIAN ADVICE + SUPPORT',
                    Descrption: 'Our goal is to ease any suffering and your dedicated physician will help make informed recommendations.'
                },
            ]
        }
    },
}
</script>
<style lang="scss" scoped>
@import '@/Scss/Main.scss';

section {
    background-color: $Main-Color;

    .header {
        p {
            font-size: 25px;
        }
    }

    .content {
        img {
            filter: grayscale(100%);
            width: 130px;
            height: 130px;
            object-fit: contain;
        }
    }
}

@media only screen and (max-width:1025px) {
    .header {
        p {
            span {
                display: inline-block !important;
            }
        }
    }
}
</style>