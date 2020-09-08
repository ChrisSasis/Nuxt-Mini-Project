<template>
    <div>
        <div class="md:flex w-full items-center hidden">
            <div class="w-full md:w-1/2">
                <nuxt-link to="/rent/test">
                <img src="~/assets/img/result.jpg" alt="" class="w-full">
                </nuxt-link>
            </div>
            <div class="md:w-1/2 p-5">
                <nuxt-link to="/rent/test">
                <h3 class="work font-bold text-blue">RESIDENTIAL</h3>  
                <h1 class="roboto text-4xl font-bold">Sunny Valley</h1>  
                <p class="work text-gray py-3">Nemo enim ipsam voluptatem quia voluptas sit aspernatur aut odit aut fugit, sed quia onse quuntur magnidolores eos qui ratione voluptate.</p>
                <p class="text-gray work">4 hours ago</p>
                </nuxt-link>
            </div>
            <div class="md:w-1/4 p-5 md:text-center">
                <h1 class="roboto text-2xl xl:text-4xl font-bold">14,599 <span class="text-sm">PHP /mo</span> </h1>
                <nuxt-link to="/rent/test">
                <button class="block mt-5 bg-blue-500 hover:bg-blue-700 text-white font-bold py-2 px-8 rounded roboto md:mx-auto">
                    View Property
                </button>
                </nuxt-link>
                <button class="mt-3 text-gray work font-normal py-2 px-4 rounded inline-flex items-center">
                    <svg class="fill-current w-4 h-4 mr-2" width="30" height="28" viewBox="0 0 30 28" fill="none" xmlns="http://www.w3.org/2000/svg">
                    <path d="M15 27.4043C14.5729 27.4043 14.1611 27.2489 13.8403 26.9666C12.6283 25.9023 11.4599 24.9022 10.429 24.02L10.4237 24.0154C7.40135 21.4287 4.79141 19.1948 2.97546 16.9943C0.945511 14.5343 0 12.2018 0 9.65371C0 7.17803 0.845261 4.89407 2.37991 3.22225C3.93288 1.53065 6.06377 0.598999 8.38074 0.598999C10.1125 0.598999 11.6984 1.14884 13.0943 2.23313C13.7988 2.78044 14.4374 3.45027 15 4.23159C15.5628 3.45027 16.2012 2.78044 16.9059 2.23313C18.3018 1.14884 19.8878 0.598999 21.6195 0.598999C23.9362 0.598999 26.0674 1.53065 27.6203 3.22225C29.155 4.89407 30 7.17803 30 9.65371C30 12.2018 29.0547 14.5343 27.0248 16.9941C25.2088 19.1948 22.5991 21.4284 19.5772 24.0149C18.5445 24.8985 17.3742 25.9003 16.1595 26.9671C15.8389 27.2489 15.4269 27.4043 15 27.4043ZM8.38074 2.36392C6.56044 2.36392 4.88823 3.09352 3.67172 4.41848C2.43713 5.76343 1.75713 7.6226 1.75713 9.65371C1.75713 11.7968 2.5502 13.7134 4.32838 15.8682C6.04706 17.951 8.60344 20.1389 11.5633 22.6722L11.5688 22.6768C12.6036 23.5625 13.7766 24.5666 14.9975 25.6387C16.2257 24.5645 17.4005 23.5588 18.4373 22.6718C21.397 20.1384 23.9532 17.951 25.6718 15.8682C27.4498 13.7134 28.2429 11.7968 28.2429 9.65371C28.2429 7.6226 27.5629 5.76343 26.3283 4.41848C25.112 3.09352 23.4396 2.36392 21.6195 2.36392C20.286 2.36392 19.0617 2.78964 17.9807 3.62911C17.0174 4.37756 16.3463 5.32369 15.9528 5.98571C15.7505 6.32615 15.3944 6.52935 15 6.52935C14.6056 6.52935 14.2495 6.32615 14.0472 5.98571C13.6539 5.32369 12.9829 4.37756 12.0193 3.62911C10.9383 2.78964 9.71397 2.36392 8.38074 2.36392Z" fill="#B3B3B3"/>
                    </svg>
                    <span>Wishlist</span>
                </button>
            </div>
        </div>
        <div class="md:hidden">
            <div class="w-full">
                <nuxt-link to="/rent/test">
                <img src="~/assets/img/result.jpg" alt="" class="w-full">
                </nuxt-link>
            </div>
            <div class="flex py-2">
                <div class="w-3/4">
                    <nuxt-link to="/rent/test">
                    <h3 class="work text-sm font-normal text-blue">Residential</h3>
                    <h1 class="roboto font-bold text-xl">Sunny Valley</h1>
                    <p class="text-gray work text-sm">4 hours ago</p>
                    </nuxt-link>
                </div>
                <div class="w-1/4 text-right">
                    <h1 class="roboto text-xl font-bold">14,599 <span class="text-sm text-gray">PHP /mo</span> </h1>
                </div>
            </div>
            <div class="flex">
                <div class="w-1/2">
                    <nuxt-link to="/rent/test">
                    <button class="block bg-blue-500 hover:bg-blue-700 text-white font-bold py-2 px-8 rounded roboto md:mx-auto">
                        View Property
                    </button>
                    </nuxt-link>
                </div>
                <div class="w-1/2 text-right">
                    <button class=" text-gray work font-normal py-2 px-4 rounded inline-flex items-center text-center">
                        <svg class="fill-current w-4 h-4 mr-2" width="30" height="28" viewBox="0 0 30 28" fill="none" xmlns="http://www.w3.org/2000/svg">
                        <path d="M15 27.4043C14.5729 27.4043 14.1611 27.2489 13.8403 26.9666C12.6283 25.9023 11.4599 24.9022 10.429 24.02L10.4237 24.0154C7.40135 21.4287 4.79141 19.1948 2.97546 16.9943C0.945511 14.5343 0 12.2018 0 9.65371C0 7.17803 0.845261 4.89407 2.37991 3.22225C3.93288 1.53065 6.06377 0.598999 8.38074 0.598999C10.1125 0.598999 11.6984 1.14884 13.0943 2.23313C13.7988 2.78044 14.4374 3.45027 15 4.23159C15.5628 3.45027 16.2012 2.78044 16.9059 2.23313C18.3018 1.14884 19.8878 0.598999 21.6195 0.598999C23.9362 0.598999 26.0674 1.53065 27.6203 3.22225C29.155 4.89407 30 7.17803 30 9.65371C30 12.2018 29.0547 14.5343 27.0248 16.9941C25.2088 19.1948 22.5991 21.4284 19.5772 24.0149C18.5445 24.8985 17.3742 25.9003 16.1595 26.9671C15.8389 27.2489 15.4269 27.4043 15 27.4043ZM8.38074 2.36392C6.56044 2.36392 4.88823 3.09352 3.67172 4.41848C2.43713 5.76343 1.75713 7.6226 1.75713 9.65371C1.75713 11.7968 2.5502 13.7134 4.32838 15.8682C6.04706 17.951 8.60344 20.1389 11.5633 22.6722L11.5688 22.6768C12.6036 23.5625 13.7766 24.5666 14.9975 25.6387C16.2257 24.5645 17.4005 23.5588 18.4373 22.6718C21.397 20.1384 23.9532 17.951 25.6718 15.8682C27.4498 13.7134 28.2429 11.7968 28.2429 9.65371C28.2429 7.6226 27.5629 5.76343 26.3283 4.41848C25.112 3.09352 23.4396 2.36392 21.6195 2.36392C20.286 2.36392 19.0617 2.78964 17.9807 3.62911C17.0174 4.37756 16.3463 5.32369 15.9528 5.98571C15.7505 6.32615 15.3944 6.52935 15 6.52935C14.6056 6.52935 14.2495 6.32615 14.0472 5.98571C13.6539 5.32369 12.9829 4.37756 12.0193 3.62911C10.9383 2.78964 9.71397 2.36392 8.38074 2.36392Z" fill="#B3B3B3"/>
                        </svg>
                        <span>Wishlist</span>
                    </button>
                </div>
            </div>
        </div>
    </div>
</template>

<script>
export default {
    name: "resultList"
}
</script>