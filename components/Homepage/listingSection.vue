<template>
    <div>
        <div class="lg:w-4/6 mx-auto px-6">
            <div class="md:flex items-center">
                <div class="md:w-2/5">
                    <h1 class="text-5xl roboto font-bold">Want to list<br/> your property?</h1>
                    <div class="cta pt-5">
                        <button class="text-blue text-gray-800 font-bold py-2 px-0 rounded inline-flex items-center">
                        <!-- <svg class="fill-current w-4 h-4 mr-2" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 20 20"><path d="M13 8V2H7v6H2l8 8 8-8h-5zM0 18h20v2H0v-2z"/></svg> -->
                        <span class="pr-2">Sign Up Now</span><img src="~assets/img/arrow.svg" alt="">
                        </button>
                    </div>
                </div>
                <div class="w-3/5 mx-auto pt-5">
                    <div class="img-pseudo relative">
                        <img src="~assets/img/propertySection.png" alt="">
                    </div>
                </div>
            </div>
        </div>
    </div>
</template>

<script>
export default {
    name: "listingSection"
}
</script>

<style scoped>
.img-pseudo:before {
    content:"";
    width:89%;
    min-height:80%;
    max-height:400px;
    background-color:#56D2DA;
    position:absolute;
    bottom:-50px;
    left:-50px;
    z-index: -1;
}
.text-blue {
    color:#56D2DA;
}
</style>