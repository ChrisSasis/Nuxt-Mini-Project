<template>
    <div>
        <headerMain/>
        <div class="searchform-holder px-3 py-5 md:p-10">
            <div class="lg:w-3/4 mx-auto">
                <searchSelectionForResult/>
            </div>
        </div>
        <div class="px-3 lg:px-10 pt-0 md:py-5 lg:py-10">
            <div class="flex items-center">
                <div class="w-1/2 md:w-5/6">
                    <div class="search-count roboto text-sm lg:text-xl">
                        <span class="property-count">134 properties found in </span> <strong>Alabang, Muntinlupa</strong>
                    </div>
                </div>
                <div class="w-1/2 md:w-1/6 text-right">
                    <button class="text-gray-800 font-bold text-sm lg:text-xl py-2 px-4 rounded inline-flex items-center">
                        <span class="pr-2">Filter</span>
                        <img src="~/assets/img/sort.svg" alt="" class="w-4">
                    </button>
                </div>
            </div>
            <resultList class="mt-10"/>
            <resultList class="mt-10"/>
        </div>
        <footerMain/>
    </div>
</template>

<script>
import headerMain from '~/components/Nav/header.vue';
import footerMain from '~/components/Footer/footer.vue';
import searchSelectionForResult from '~/components/searchSelectionForResult.vue';
import resultList from '~/components/resultList.vue';
export default {
    name: "result",
    components: {
        headerMain,
        footerMain,
        searchSelectionForResult,
        resultList
    }
}
</script>

<style scoped>
.searchform-holder {
    background-color: #F5F5F5;
}
.property-count {
    color:#848484;
}

@media screen and (max-width:767px) {
    .searchform-holder {
        background-color: #ffff;
    }
}
</style>