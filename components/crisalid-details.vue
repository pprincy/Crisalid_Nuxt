<template>
  <div class="crisalid-details-section">
    <div class="container">
      <div class="row justify-content-center align-items-center">
        <div class="content-section">
          <div v-for="navigation in navigations" v-bind:key="navigation" class="white">
            <div class="content">
              <div class="logo-content">
                <b-img :src="navigation.img" class="content-logo-section" alt="logo" />
              </div>
              <div class="title-section text-uppercase p-3">
                <div>{{navigation.title}}</div>
              </div>
            </div>

            <div class="vision-content p-3" :class="navigation.class" v-html="navigation.content"></div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>
<script>
export default {
  props: ["navigations"]
};
</script>
<style lang="scss">
@import "~/assets/scss/variable";
.crisalid-details-section {
  .content-section {
    margin: 220px auto 0;
    .content {
      position: relative;
      text-decoration: none;
      text-align: center;
      .title-section::after {
        content: "";
        position: absolute;
        left: 46%;
        bottom: 0;
        width: 16px;
        border-radius: 20px;
        background-color: $white;
        border: 1px solid $white;
      }
      .logo-content {
        .content-logo-section {
          width: 100px;
        }
      }
    }
    .vision-content {
      width: 335px;
      margin: 0 auto;
      text-align: center;
    }
  }
}
@import "~/assets/scss/mobile";
</style>
