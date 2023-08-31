<template>
  <div class="home-section">
    <!-- header section component start -->
    <div>
      <header-section></header-section>
    </div>
    <!-- header section component end -->

    <!-- crisalid section component start -->
    <div>
      <crisalid-img-section></crisalid-img-section>
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
import crisalidImgSection from "~/components/crisalid-img-section.vue";
import crisalidDetails from "~/components/crisalid-details.vue";
import homeImage from "~/assets/images/home.svg";
export default {
  data() {
    return {
      navigations: [
        {
          class: 'crisalid',
          img: homeImage,
          title: "welcome to the experience age",
          content:
            "Today, a customer's interaction with a luxury brand goes much beyond the tangible; they want to live your brand. <br/><br/> That is where we come in. <br/><br/> <i>'European Standards, Indian Understanding'</i> <br/><br/> We are Crisalid"
        }
      ]
    };
  },
  components: {
    headerSection,
    crisalidImgSection,
    crisalidDetails
  }
};
</script>
<style lang="scss">
@import "~/assets/scss/variable";
.crisalid {
  font-size: $font-12;
}
@import "~/assets/scss/mobile";
</style>