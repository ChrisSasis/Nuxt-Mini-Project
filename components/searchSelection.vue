<template>
    <div>
        <div class="lg:flex">
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
                <nuxt-link to="/search/result">
                <button class="roboto w-full bg-blue-500 hover:bg-blue-700 text-white font-bold py-3 px-4 rounded outline-none">Search</button>
                </nuxt-link>
            </div>
        </div>
    </div>
</template>

<script>
export default {
    name: "searchSelection"
}
</script>

<style scoped>
select,input {
    padding: 14px 1rem;
}
</style>