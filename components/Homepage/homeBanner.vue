<template>
    <div>
        <div class="homeBanner py-20 px-10 md:px-24 md:py-48 lg:py-48 lg:px-32 xl:p-48">
            <h1 class="text-3xl lg:text-4xl xl:text-5xl text-center font-bold">Find the right place to stay</h1>
            <div class="pt-5">
                <searchSelection/>
            </div>
        </div>
    </div>
</template>

<script>
import searchSelection from '~/components/searchSelection.vue';
export default {
    name: "homeBanner",
    components: {
        searchSelection
    }
}
</script>

<style scoped>
.homeBanner {
    background:url("~assets/img/homebanner.jpg");
    background-size: cover;
    background-repeat: no-repeat;
}
.text-4xl {
    color:#272727;
}
</style>
