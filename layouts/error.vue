<template>
    <div>
        <headerMain/>
        <div class="px-3">
            <div class="container md:mx-auto border-4 border-blue-500 mt-10 p-10 md:px-22 md:py-24 text-center md:w-9/12">
                <div v-if="error.statusCode === 404">
                    <h1 class="text-2xl md:text-4xl roboto font-bold text-center ">404 Page Not Found</h1>
                    <p class="work text-sm md:text-xl text-center pb-4">Sorry, the page that you’re looking for doesn’t exist.</p>
                    <nuxt-link to="/" class="roboto w-64 bg-blue-500 hover:bg-blue-700 text-white font-bold py-3 px-4 rounded outline-none mx-auto">Back to Home</nuxt-link>
                </div>
                <h1 v-else>An error occurred</h1>
            </div>
        </div>
    </div>
</template>

<script>
import headerMain from '~/components/Nav/header.vue';
export default {
    props: ['error'],
    layout: 'index',
    components: {
        headerMain,
    }
}
</script>