<template>
    <section>
        <div class="container">

            <Head Text="INSURANCES WE ACCEPT" />
            <div class="row justify-content-center align-items-center">
                <div class="col-lg-3 col-md-6 col-sm-12 text-center d-flex justify-content-center align-items-center">
                    <img src="@/Imgs/location_Jp4vBwWWQJdspq8YagE9_images_7f182cd2-26b4-4731-8b5e-4a8a0d694c10.png"
                        class="img-fluid">
                </div>
                <div class="col-lg-3 col-md-6 col-sm-12 text-center d-flex justify-content-center align-items-center">
                    <img src="@/Imgs/25549216-dfa4-4385-ab28-9b0f0fbcc545.png" class="img-fluid">
                </div>
                <div class="col-lg-3 col-md-6 col-sm-12 text-center d-flex justify-content-center align-items-center">
                    <img src="@/Imgs/location_Jp4vBwWWQJdspq8YagE9_images_7f182cd2-26b4-4731-8b5e-4a8a0d694c10.png"
                        class="img-fluid" style="filter: grayscale(100%);">
                </div>
                <div class="col-lg-3 col-md-6 col-sm-12 text-center d-flex justify-content-center align-items-center">
                    <img src="@/Imgs/location_Jp4vBwWWQJdspq8YagE9_images_e3ad4744-ea44-4725-be93-7ea03917616a.png"
                        class="img-fluid">
                </div>
            </div>
            <div class="row">
                <div class="col-12 text-center">
                    <img src="@/Imgs/ca28e34c-f78a-4072-9840-597caeef2e3d.jpeg" class="pt-4">
                    <h4 class="py-4 mb-5">See If We Accept Your Insurance. Call To Learn More!</h4>
                </div>
            </div>
        </div>
    </section>
</template>
<script>
import Head from '../HeadEachSection/Head.vue';

export default {
    name: "Insurances",
    components: { Head }
}
</script>
<style lang="scss" scoped>
@import '@/Scss/Main.scss';

section {
    img {
        object-fit: contain;
        width: 170px;
        height: 150px;
    }
}
</style>