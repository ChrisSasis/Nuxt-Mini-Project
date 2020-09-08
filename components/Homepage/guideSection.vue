<template>
    <div>
        <div class="md:flex items-center">
            <div class="md:w-1/2">
                <h3 class="text-md font-bold work text-blue">HERE’S OUR</h3>
                <h1 class="text-4xl font-bold roboto">Neighborhood Guide</h1>
            </div>
            <div class="md:w-1/2 md:px-5">
                <p class="work content">We’ve curated top cities to choose from. From urban area to near business district, we’ve got it.</p>
            </div>
        </div>
        <div class="md:flex mb-4 mt-4">
            <div class="md:w-1/2 p-5 ">
                <div class="img-pseudo relative">
                    <img src="~assets/img/guideSection.png" alt="">
                </div>
            </div>
            <div class="md:w-1/2 p-5">
                <div class="border-4 border-blue-500 w-10"></div>
                <h1 class="text-2xl font-bold roboto pt-5">Fort Bonifacio Global City, Taguig</h1>
                <p class="pt-5 work content">
                    Bonifacio Global City is a commercial hub known
                    for glitzy shopping areas like Bonifacio High Street,
                    filled with big-name brands and flagship stores.
                    Upscale global restaurants mix with cocktail bars,
                    hip cafes, and mainstream nightclubs.
                    <br/><br/>

                    The Mind Museum offers hands-on science displays,
                    while the Manila American Cemetery honors WWII soldiers. Colorful street murals make the area popular for strolling.

                    <button class="block mt-5 bg-blue-500 hover:bg-blue-700 text-white font-bold py-2 px-8 rounded roboto">
                        View More
                    </button>
                </p>
            </div>
        </div>
    </div>
</template>

<script>
export default {
    name: "guideSection"
}
</script>

<style scoped>
.text-blue {
    color:#56D2DA;
}
.content {
    color:#848484;
}
.img-pseudo:before {
    content: "";
    width:80%;
    height:100px;
    background-color: #56D2DA;
    position:absolute;
    bottom:-50px;
    left:-25px;
    z-index: -1;
}
</style>