<template>
  <div>
    <headerMain/>
    <div class="px-3 lg:px-10">
      <homeBanner/>
      <offerSection class="mt-10"/>
      <guideSection class="mt-12"/>
      <listingSection class="mt-32 mb-32"/>
    </div>
    <!-- footer -->
    <footerMain class="mt-10"/>
  </div>
</template>

<script>
import headerMain from '~/components/Nav/header.vue';
import footerMain from '~/components/Footer/footer.vue';
import homeBanner from '~/components/Homepage/homeBanner.vue';
import offerSection from '~/components/Homepage/offerSection.vue';
import guideSection from '~/components/Homepage/guideSection.vue';
import listingSection from '~/components/Homepage/listingSection.vue';
  
export default {
  name: "index",
  components: {
    headerMain,
    footerMain,
    homeBanner,
    offerSection,
    guideSection,
    listingSection
  }
}
</script>