<template>
    <section>
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
        </div>
    </section>
</template>
<script>
import Head from '../HeadEachSection/Head.vue';

export default {
    name: "OurServeces",
    components: { Head }
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
}
</style>