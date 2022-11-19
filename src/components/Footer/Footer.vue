<template>
    <footer>
        <div class="container">
            <div class="row">
                <div class="col-12 text-center">
                    <div class="btn py-3 px-4 my-5">View Our Hospice Service Menu</div>
                    <div class="line mb-2"></div>
                    <p class="text-light mb-5 mt-3">© Copyright 2021 White Orchid Hospice <span class="d-block">All
                            trademarks and copyrights belong
                            to their respective owners.</span></p>
                </div>
            </div>
        </div>
    </footer>
</template>
<script>
import PhoneButton from '../PhoneButton/PhoneButton.vue';

export default {
    name: "Footer",
    components: { PhoneButton }
}
</script>
<style lang="scss" scoped>
@import '@/Scss/Main.scss';

footer {
    background-color: $Main-Color;

    .btn {
        border: 3px solid $Text-Color;
        border-radius: 20px;
        font-size: 18px;
        color: $Text-Color ;
        font-weight: bold;
    }

    .line {
        border-top: 1px solid $Text-Color;
        width: 100%;

    }
    p{
        font-size: 14px;
    }
}
</style>