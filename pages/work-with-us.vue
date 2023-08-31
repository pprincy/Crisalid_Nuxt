<template>
  <div class="work-with-us-section">
    <!-- header section component start -->
    <div>
      <header-section></header-section>
    </div>
    <!-- header section component end -->

    <!-- work-with-us-section start -->
    <div class="work-with-us-content">
      <div class="container">
        <div class="row">
          <div class="bg-overlay text-center">
            <div class="work text-capitalize">work with us</div>
          </div>
        </div>
        <div class="row justify-content-center pt-5">
          <div class="resume-section">
            <b-button squared class="upload-btn">
              <a href="mailto:bloom@crisalidindia.com?subject=Website: Resume Submission">Upload your resume</a>
            </b-button>
          </div>
        </div>
      </div>
    </div>
    <!-- work-with-us-section end -->
  </div>
</template>
<script>
import headerSection from "~/components/header-section.vue";
export default {
  components: {
    headerSection
  }
};
</script>
<style lang="scss">
@import "~/assets/scss/variable";
.work-with-us-section {
  background: $black;
  height: 100vh;
  .work-with-us-content {
    padding-top: 150px;
    color: $white;
    .bg-overlay {
      background: linear-gradient(rgba(0, 0, 0, 0.7), rgba(0, 0, 0, 0.7)),
        url("~@/assets/images/new-triangle.png") no-repeat center center;
      height: 320px;
      padding-top: 90px;
      width: 100%;
      color: $white;
      .work {
        font-size: $font-46;
      }
    }
    .resume-section {
      .upload-btn {
        font-size: $font-20;
        color: $white;
      }
      .btn-secondary {
        background-color: $black;
      }
      a {
        color: $white;
        text-decoration: none;
        background-color: transparent;
      }
    }
  }
}
@import "~/assets/scss/mobile";
</style>