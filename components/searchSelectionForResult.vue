<template>
    <div>
        <div class="hidden md:flex">
            <div class="w-full pb-5 lg:pb-0 lg:w-1/2 px-3">
                <input type="text" class="roboto w-full appearance-none block w-full text-gray-700 rounded-lg  leading-tight focus:outline-none focus:bg-white" placeholder="Enter Location">
            </div>
            <div class="w-full pb-5 lg:pb-0 lg:w-64 px-3">
                <div class="select-holder">
                <select class="roboto block appearance-none w-full border-gray-200 text-gray-700 rounded-lg leading-tight focus:outline-none focus:bg-white focus:border-gray-500">
                    <option>Property Type</option>
                    <option value="">Residential</option>
                    <option value="">Condominium</option>
                    <option value="">Apartment</option>
                </select>
                </div>
            </div>
            <div class="w-full pb-5 lg:pb-0 lg:w-56 px-3">
                <div class="select-holder">
                    <select class="roboto block appearance-none w-full border-gray-200 text-gray-700 rounded-lg leading-tight focus:outline-none focus:bg-white focus:border-gray-500">
                        <option>Price Range</option>
                        <option value="">Any</option>
                        <option value="">P2,000 - P5,000</option>
                        <option value="">P5,000 - P10,000</option>
                    </select>
                </div>
            </div>
            <div class="w-full lg:w-56 px-3">
                <button class="roboto w-full bg-blue-500 hover:bg-blue-700 text-white font-bold py-3 px-4 rounded outline-none">Search</button>
            </div>
        </div>
        <div class="hidden md:flex mt-4 px-3">
            <div class="bg-blue-500 rounded-full py-2 px-4 text-sm text-white mr-2">Condominium</div>
            <div class="bg-blue-500 rounded-full py-2 px-4 text-sm text-white">Residential</div>
        </div>
        <div class="md:hidden">
            <div class="flex">
                <div class="w-4/5 pr-2 text-center">
                    <input type="text" class="location-field roboto py-3 px-3 w-full appearance-none block w-full text-gray-700 rounded-lg border bg-gray leading-tight focus:outline-none focus:bg-white" placeholder="Enter Location">
                </div>
                <div class="w-1/5 text-center">
                    <button class="w-full inline-block bg-blue-500 hover:bg-blue-700 py-4 px-3 rounded text-center focus:outline-none" @click="showFilter()">
                        <svg class="mx-auto" width="17" height="17" viewBox="0 0 17 17" fill="none" xmlns="http://www.w3.org/2000/svg">
                            <rect y="1.78955" width="17" height="1.78947" fill="white"/>
                            <rect y="8.05273" width="17" height="1.78947" fill="white"/>
                            <rect y="14.3159" width="17" height="1.78947" fill="white"/>
                            <ellipse cx="4.24999" cy="2.23684" rx="1.93182" ry="2.23684" fill="white"/>
                            <ellipse cx="12.7501" cy="8.50003" rx="1.93182" ry="2.23684" fill="white"/>
                            <ellipse cx="6.56817" cy="14.7632" rx="1.93182" ry="2.23684" fill="white"/>
                        </svg>
                    </button>
                </div>
            </div>
            <div class="flex mt-4">
                <div class="bg-blue-500 rounded-full py-2 px-4 text-sm text-white mr-2">Condominium</div>
                <div class="bg-blue-500 rounded-full py-2 px-4 text-sm text-white">Residential</div>
            </div>
            <!-- popup -->
            <div class="filter-popup bg-white py-2 px-3 hide" v-bind:class="{ 'show': filterPop }">
                <div class="heading-popup">
                    <div class="flex">
                        <div class="w-1/2">
                            <h1 class="text-3xl font-bold work text-gray-500">Filter</h1>
                        </div>
                        <div class="w-1/2 text-right">
                            <button class="py-3 px-2 focus:outline-none " @click="showFilter()">
                                <svg height="20px" viewBox="0 0 365.696 365.696" width="20px" xmlns="http://www.w3.org/2000/svg"><path d="m243.1875 182.859375 113.132812-113.132813c12.5-12.5 12.5-32.765624 0-45.246093l-15.082031-15.082031c-12.503906-12.503907-32.769531-12.503907-45.25 0l-113.128906 113.128906-113.132813-113.152344c-12.5-12.5-32.765624-12.5-45.246093 0l-15.105469 15.082031c-12.5 12.503907-12.5 32.769531 0 45.25l113.152344 113.152344-113.128906 113.128906c-12.503907 12.503907-12.503907 32.769531 0 45.25l15.082031 15.082031c12.5 12.5 32.765625 12.5 45.246093 0l113.132813-113.132812 113.128906 113.132812c12.503907 12.5 32.769531 12.5 45.25 0l15.082031-15.082031c12.5-12.503906 12.5-32.769531 0-45.25zm0 0"/></svg>
                            </button>
                        </div>
                    </div>
                </div>
                <filterResult />
            </div>
        </div>
    </div>
</template>

<script>
import filterResult from '~/components/filterResult.vue';
export default {
    name: "searchSelection",
    components: {
        filterResult
    },
    data() {
        return {
            filterPop: false
        }
    },
    methods: {
        showFilter() {
            if(this.filterPop == false) {
                this.filterPop = true;
            } else {
                this.filterPop = false;
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
select,input {
    padding: 14px 1rem;
}
.location-field {
    background-color:#f6f6f6;
}
.filter-popup {
    position:fixed;
    top:0;
    left:0;
    width:100%;
    height:100%;
    z-index: 100;
}
</style>