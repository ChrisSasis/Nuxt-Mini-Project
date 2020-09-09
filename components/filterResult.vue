<template>
    <div>
        <div class="bg-white py-5">
            <h1 class="text-xl font-bold roboto">Property Type</h1>
            <div class="flex flex-wrap mt-4">
                <div class="bg-blue-500 rounded-full py-2 px-4 border-2 border-blue-500 text-sm text-white mr-2 work mb-2">All</div>
                <div class="rounded-full py-2 px-4 border-2 text-sm text-blue mr-2 work mb-2">Condominium</div>
                <div class="rounded-full py-2 px-4 border-2 text-sm text-blue work mb-2">Residential</div>
                <div class="rounded-full py-2 px-4 border-2 text-sm text-blue work mb-2">House</div>
            </div>
        </div>
        <div class="bg-white">
            <h1 class="text-xl font-bold roboto">Price Range</h1>
            <select name="" id="" class="w-full border-2 py-3 px-3 mt-4 focus:outline-none">
                <option value="">P2,000 - P5,000</option>
                <option value="">P5,000 - P10,000</option>
                <option value="">P10,000 - P15,000</option>
                <option value="">P15,000 - P20,000</option>
            </select>
        </div>
        <div class="mt-10">
            <button class="roboto w-full bg-blue-500 hover:bg-blue-700 text-white font-bold py-3 px-4 rounded outline-none focus:outline-none">Done</button>
        </div>
    </div>
</template>

<script>
export default {
    name: "filterResult"
}
</script>

<style scoped>
</style>