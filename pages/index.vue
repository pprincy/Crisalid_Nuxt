<template>
  <div class="home-section-bg">
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
  </div>
</template>

<script>
import headerSection from "~/components/header-section.vue";
import crisalidSection from "~/components/crisalid-section.vue";
export default {
  components: {
    headerSection,
    crisalidSection
  }
};
</script>

<style lang="scss">
@import "~/assets/scss/variable";
.home-section-bg {
  background: url("~@/assets/images/bg-img.jpg") no-repeat center center $bg-black;
  background-size: contain;
  height: 100vh;
}
</style>
