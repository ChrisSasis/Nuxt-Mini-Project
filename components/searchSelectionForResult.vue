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
        <div class="md:hidden">
            <div class="flex">
                <div class="w-4/5 pr-2 text-center">
                    <input type="text" class="location-field roboto py-3 px-3 w-full appearance-none block w-full text-gray-700 rounded-lg border bg-gray leading-tight focus:outline-none focus:bg-white" placeholder="Enter Location">
                </div>
                <div class="w-1/5 text-center">
                    <button class="w-full inline-block bg-blue-500 hover:bg-blue-700 py-4 px-3 rounded text-center">
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
.location-field {
    background-color:#f6f6f6;
}
</style>