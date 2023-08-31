<template>
  <div class="home-section">
    <!-- header section component start -->
    <div>
      <header-section></header-section>
    </div>
    <!-- header section component end -->

    <!-- crisalid section component start -->
    <div>
      <crisalid-section></crisalid-section>
    </div>
    <!-- crisaild section component end -->

    <!-- crisalid details component start -->
    <div>
      <crisalidDetails v-bind:navigations="navigations" />
    </div>
    <!-- crisalid details component end -->
  </div>
</template>
<script>
import headerSection from "~/components/header-section.vue";
import crisalidSection from "~/components/crisalid-section.vue";
import crisalidDetails from "~/components/crisalid-details.vue";
import homeImage from "~/assets/images/home.svg";
export default {
  data() {
    return {
      navigations: [
        {
          img: homeImage,
          title: "our mission",
          content:
            "to enrich customer experiences by enhancing brand-customer relationships through tailor-made programs"
        }
      ]
    };
  },
  components: {
    headerSection,
    crisalidSection,
    crisalidDetails
  }
};
</script>
<style lang="scss">
@import "~/assets/scss/variable";
@import "~/assets/scss/mobile";
</style>