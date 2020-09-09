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
                <div class="w-1/2 md:w-1/6 text-right relative">
                    <button @click="showSort()"
                    class="text-gray-800 font-bold text-sm lg:text-xl py-2 px-4 rounded inline-flex items-center outline-none focus:outline-none hover:bg-gray-200">
                        <span class="pr-2">Sort</span>
                        <img src="~/assets/img/sort.svg" alt="" class="w-4">
                    </button>
                    <div class="float-sort shadow rounded hide" v-bind:class="{ 'show': popIn }">
                        <ul>
                            <li>
                                <button class="focus:outline-none w-full block text-center px-10 py-3 roboto bg-gray-200 hover:bg-gray-200">
                                    Most Recent
                                </button>
                            </li>
                            <li>
                                <button class="focus:outline-none w-full block text-center px-10 py-3 roboto hover:bg-gray-200">
                                    Recommended
                                </button>
                            </li>
                            <li>
                                <button class="focus:outline-none w-full block text-center px-10 py-3 roboto hover:bg-gray-200">
                                    Highest Price
                                </button>
                            </li>
                            <li>
                                <button class="focus:outline-none w-full block text-center px-10 py-3 roboto hover:bg-gray-200">
                                    Lowest Price
                                </button>
                            </li>
                        </ul>
                    </div>

                </div>
            </div>
            <resultList class="mt-5 md:mt-10"/>
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
    },
    data() {
        return {
            popIn: false
        }
    },
    methods: {
        showSort() {
            if(this.popIn == false) {
                this.popIn = true;
            } else {
                this.popIn = false;
            }
        }
    }
}
</script>

<style scoped>
.hide {
    display: none !important;
}
.show{
    display:block !important;
}
.searchform-holder {
    background-color: #F5F5F5;
}
.property-count {
    color:#848484;
}
.float-sort {
    position:absolute;
    top:40px;
    right:0;
    z-index: 50;
    background-color: #fff;
}

@media screen and (max-width:767px) {
    .searchform-holder {
        background-color: #ffff;
    }
}
</style>