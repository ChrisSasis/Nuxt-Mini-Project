<template>
    <div>
        <div class="hidden md:block">
            <headerMain/>
        </div>
        <div class="md:hidden">
            <div class="price-float px-3 py-3">
                <div class="flex">
                    <div class="w-1/2">
                        <h1 class="text-2xl font-bold">₱ 14,990 <span class="text-sm font-normal text-gray">/month</span></h1>  
                    </div>
                    <div class="w-1/2 text-right">
                        <button class="inline-block bg-blue-500 hover:bg-blue-700 text-white text-sm font-bold py-2 px-5 rounded roboto mx-auto">
                            Schedule A Viewing
                        </button>
                    </div>
                </div>
            </div>
        </div>
        
        <div class="cover-banner relative">
            <!-- cover -->
            <div class="px-0 lg:px-10 hidden md:block">
                <img src="https://a.storyblok.com/f/93275/1300x478/5a92f0f24e/singlebanner.png" alt="" class="w-full">
            </div>
            <CoolLightBox 
            :items="items" 
            :index="index"
            @close="index = null">
            </CoolLightBox>
            <div class="images-wrapper">
            <div class="md:hidden">
                <swiper ref="mySwiper" :options="swiperOption" class="swiper md:mt-5 md:hidden">
                    <swiper-slide v-for="(image, imageIndex) in items" :key="imageIndex">
                        <div class="img-holder"  @click="index = imageIndex" >
                            <img :src="image.src" alt="">
                        </div>
                    </swiper-slide>
                    <div class="swiper-pagination" slot="pagination"></div>
                </swiper>
                <div class="count text-right">
                    <!-- <button class="border text-base border-blue bg-white text-base py-2 px-3" >Show All Photos</button> -->
                </div>

                <nuxt-link to="/search/result">
                    <button class="md:hidden back-btn text-white rounded-full">
                        <svg width="12" height="20" viewBox="0 0 10 16" fill="none" xmlns="http://www.w3.org/2000/svg">
                            <path d="M3.45881 8.00338L9.44437 2.01756C9.60918 1.85314 9.69985 1.6333 9.69985 1.39889C9.69985 1.16436 9.60918 0.94465 9.44437 0.779967L8.91988 0.25574C8.75533 0.0907967 8.53536 0 8.30095 0C8.06655 0 7.84684 0.0907967 7.68216 0.25574L0.555394 7.38237C0.390061 7.54758 0.299524 7.76832 0.300174 8.00299C0.299524 8.2387 0.38993 8.45919 0.555394 8.62452L7.67552 15.7443C7.84021 15.9092 8.05991 16 8.29445 16C8.52886 16 8.74856 15.9092 8.91338 15.7443L9.43773 15.22C9.77894 14.8788 9.77894 14.3234 9.43773 13.9823L3.45881 8.00338Z" fill="white"/>
                        </svg>
                    </button>
                </nuxt-link>

            </div>
        </div>
    </div>
        <div class="px-3 lg:px-10 mt-5 lg:mt-16">
            <div class="md:flex mb-4">
                <div class="md:w-1/2 lg:w-2/3 pr-10">
                    <h3 class="lg:text-2xl work font-bold text-blue">RESIDENTIAL</h3>
                    <h1 class="text-2xl lg:text-5xl roboto font-bold">Sunny Valley</h1>

                    <div class="pt-10">
                        <h3 class="text-base lg:text-xl roboto font-bold">About the Property</h3>
                        <p class="text-gray work font-md py-5">There are three basic materials for covering: wood, metal and ceramic tiles. We had designed this house with panoramic windows, so we only filled it up with functionality.</p>
                    </div>
                    <div class="pt-5">
                        <h3 class="text-base lg:text-xl  roboto font-bold">Property Highlight</h3>
                        <p class="text-gray work font-md py-5">There are three basic materials for covering: wood, metal and ceramic tiles. We had designed this house with panoramic windows, so we only filled it up with functionality.</p>
                    </div>
                    <div class="pt-5">
                        <h3 class="text-base lg:text-xl roboto font-bold">Nearby Places</h3>
                        <p class="text-gray work font-md py-5">There are three basic materials for covering: wood, metal and ceramic tiles. We had designed this house with panoramic windows, so we only filled it up with functionality.</p>
                    </div>
                </div>
                <div class="md:w-1/2 lg:w-1/3 lg:pt-8">
                    <div class="text-right">
                        <h1 class="roboto font-bold text-sm md:text-3xl lg:text-5xl hidden md:block">14,599 <span class="text-sm">PHP /mo</span></h1>
                        <button class="hidden md:inline-block mt-5 bg-blue-500 hover:bg-blue-700 text-white font-bold py-2 px-8 rounded roboto ">
                            Schedule A Viewing
                        </button>
                        <div>
                            <button class="hidden md:inline-flex mt-3 text-gray work font-normal py-2 px-4 rounded items-center">
                                <!-- <svg class="fill-current w-4 h-4 mr-2" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 20 20"><path d="M13 8V2H7v6H2l8 8 8-8h-5zM0 18h20v2H0v-2z"/></svg> -->
                                <svg class="fill-current w-4 h-4 mr-2" width="30" height="28" viewBox="0 0 30 28" fill="none" xmlns="http://www.w3.org/2000/svg">
                                <path d="M15 27.4043C14.5729 27.4043 14.1611 27.2489 13.8403 26.9666C12.6283 25.9023 11.4599 24.9022 10.429 24.02L10.4237 24.0154C7.40135 21.4287 4.79141 19.1948 2.97546 16.9943C0.945511 14.5343 0 12.2018 0 9.65371C0 7.17803 0.845261 4.89407 2.37991 3.22225C3.93288 1.53065 6.06377 0.598999 8.38074 0.598999C10.1125 0.598999 11.6984 1.14884 13.0943 2.23313C13.7988 2.78044 14.4374 3.45027 15 4.23159C15.5628 3.45027 16.2012 2.78044 16.9059 2.23313C18.3018 1.14884 19.8878 0.598999 21.6195 0.598999C23.9362 0.598999 26.0674 1.53065 27.6203 3.22225C29.155 4.89407 30 7.17803 30 9.65371C30 12.2018 29.0547 14.5343 27.0248 16.9941C25.2088 19.1948 22.5991 21.4284 19.5772 24.0149C18.5445 24.8985 17.3742 25.9003 16.1595 26.9671C15.8389 27.2489 15.4269 27.4043 15 27.4043ZM8.38074 2.36392C6.56044 2.36392 4.88823 3.09352 3.67172 4.41848C2.43713 5.76343 1.75713 7.6226 1.75713 9.65371C1.75713 11.7968 2.5502 13.7134 4.32838 15.8682C6.04706 17.951 8.60344 20.1389 11.5633 22.6722L11.5688 22.6768C12.6036 23.5625 13.7766 24.5666 14.9975 25.6387C16.2257 24.5645 17.4005 23.5588 18.4373 22.6718C21.397 20.1384 23.9532 17.951 25.6718 15.8682C27.4498 13.7134 28.2429 11.7968 28.2429 9.65371C28.2429 7.6226 27.5629 5.76343 26.3283 4.41848C25.112 3.09352 23.4396 2.36392 21.6195 2.36392C20.286 2.36392 19.0617 2.78964 17.9807 3.62911C17.0174 4.37756 16.3463 5.32369 15.9528 5.98571C15.7505 6.32615 15.3944 6.52935 15 6.52935C14.6056 6.52935 14.2495 6.32615 14.0472 5.98571C13.6539 5.32369 12.9829 4.37756 12.0193 3.62911C10.9383 2.78964 9.71397 2.36392 8.38074 2.36392Z" fill="#B3B3B3"/>
                                </svg>
                                <span>Wishlist</span>
                            </button>
                        </div>
                        <ul>
                            <li class="pb-5 pt-8 border-b-2">
                                <div class="flex">
                                    <div class="w-1/2 text-left">
                                        <strong class="roboto">Location</strong>
                                    </div>
                                    <div class="w-1/2">
                                        <span class="work text-gray">Alabang, Muntinlupa</span>
                                    </div>
                                </div>
                            </li>
                            <li class="pb-5 pt-8 border-b-2">
                                <div class="flex">
                                    <div class="w-1/2 text-left">
                                        <strong class="roboto">Owner</strong>
                                    </div>
                                    <div class="w-1/2">
                                        <span class="work text-gray">John Appleased</span>
                                    </div>
                                </div>
                            </li>
                            <li class="pb-5 pt-8 border-b-2">
                                <div class="flex">
                                    <div class="w-1/2 text-left">
                                        <strong class="roboto">Property Type</strong>
                                    </div>
                                    <div class="w-1/2">
                                        <span class="work text-gray">Residential</span>
                                    </div>
                                </div>
                            </li>
                        </ul>
                    </div>
                </div>
            </div>
            <div class="pt-0 hidden md:block">
                <h3 class="text-xl roboto font-bold">Gallery</h3>
                <swiper ref="mySwiper" :options="swiperOption" class="swiper mt-5" >
                    <swiper-slide v-for="(image, imageIndex) in items" :key="imageIndex">
                        <img :src="image.src" alt="" @click="index = imageIndex">
                    </swiper-slide>
                    <div class="swiper-pagination" slot="pagination"></div>
                </swiper>
            </div>
        </div>
        <!-- footer -->
        <footerMain class="mt-10"/>
    </div>
</template>

<script>
import headerMain from '~/components/Nav/header.vue';
import footerMain from '~/components/Footer/footer.vue';
import CoolLightBox from 'vue-cool-lightbox';
 
export default {
    name: "slug",
    components: {
        headerMain,
        footerMain,
        CoolLightBox,
    },
    data() {
      return {
        items: [
            {
                id: 1,
                name: 'sas',
                src: '/gallery-1.jpg'
            },
            {
                id: 2,
                name: 'sas',
                src: '/gallery-2.jpg'
            },
            {
                id: 3,
                name: 'sas',
                src: '/gallery-1.jpg'
            },
            {
                id: 4,
                name: 'sas',
                src: '/gallery-2.jpg'
            },
        ],
        total: "",
        swiperOption: {
            // slidesPerView: 1,
            breakpoints: {
                1024: {
                    slidesPerView: 3,
                    spaceBetween: 30,
                },
                650: {
                    slidesPerView: 2,
                    spaceBetween:20
                },
                640: {
                    slidesPerView: 1,
                    spaceBetween: 0,
                }
            },
            pagination: {
                el: '.swiper-pagination',
            },
        },
        index: null
      }
    },
    computed: {
      swiper() {
        return this.$refs.mySwiper.$swiper
      }
    },
    created() {
       this.total =  this.items.length;
    }
}
</script>
<style>
.swiper-slide {
    width: auto;
}
.cool-lightbox {
    background:#fff!important;
}
.cool-lightbox .cool-lightbox__slide img {
    box-shadow: none !important;
}
.cool-lightbox-toolbar .cool-lightbox-toolbar__btn,
.cool-lightbox .cool-lightbox-button>.cool-lightbox-button__icon {
    background:#56D2DA;
    color:#fff !important;
}
.swiper img {
    width: 100%;
    cursor:pointer;
}
</style>

<style scoped>
.cover-banner:before {
    content: '';
    width:100%;
    height:150px;
    background:#56D2DA;
    position:absolute;
    bottom:-30px;
    left:0;
    z-index: -1;
}
.price-float {
    position:fixed;
    background-color: #fff;
    bottom:0;
    left:0;
    width:100%;
    z-index: 100;
    border-top:1px solid #9CDDE1;
}
.img-holder {
    height:220px;
    overflow: hidden;
}
.count {
    position:absolute;
    bottom:0;
    right:0;
    z-index: 10;
}
.back-btn {
    width:35px;
    height:35px;
    text-align:center;
    padding-left:10px;
    position: absolute;
    top:10px;
    left:0.75rem;
    outline:none;
    z-index: 100;
    background:rgba(0,0,0,0.2);
}
@media screen and (max-width: 1023px) {
    .cover-banner:before {
        content:none;
    }
}
</style>