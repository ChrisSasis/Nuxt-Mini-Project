<template>
    <div>
        <div class="border-blue-500 border-4 py-10 px-5">
            <h1 class="text-center text-4xl roboto font-bold">What We Offer</h1>
            <div class="md:flex mb-4 mt-4 ">
                <div class="md:w-1/3 p-5 flex items-center justify-center">
                    <div class="w-1/6 img-holder inline-block align-middle">
                        <img src="~assets/img/moneybank.svg" alt="">
                    </div>
                    <span class="w-5/6 pl-5 text inline-block align-middle text-xl lg:text-2xl font-bold">
                        Money-back Guaranteed
                    </span>
                </div>
                <div class="md:w-1/3 p-5 flex items-center justify-center">
                    <div class="w-1/6 img-holder inline-block align-middle">
                        <img src="~assets/img/like.svg" alt="">
                    </div>
                    <span class="w-5/6 pl-5 text inline-block align-middle text-xl lg:text-2xl font-bold">
                        Hassle-fee Transaction
                    </span>
                </div>
                <div class="md:w-1/3 p-5 flex items-center justify-center">
                    <div class="w-1/6 img-holder inline-block align-middle">
                        <img src="~assets/img/chat.svg" alt="">
                    </div>
                    <span class="w-5/6 pl-5 text inline-block align-middle text-xl lg:text-2xl font-bold">
                        24/7 Customer Support
                    </span>
                </div>
                <!-- <div class="md:w-1/3 bg-gray-500">
                    <img src="~assets/img/like.svg" alt="">
                </div>
                <div class="md:w-1/3 bg-gray-400">
                    <img src="~assets/img/chat.svg" alt="">
                </div> -->
            </div>
        </div>
    </div>
</template>

<script>
export default {
    name: "offerSection"
}
</script>