<template>
  <div class="about-us-section main-bg">
    <!-- header section component start -->
    <div>
      <header-section></header-section>
    </div>
    <!-- header section component end -->

    <!-- about-us-section start -->
    <div class="about-us-content white pt-90 pb-5">
      <div class="container">
        <div class="row">
          <div class="col-md-8">
            <div class="luxury-section">
              A luxury consultancy tailor - made
              for the Indian market
            </div>
          </div>
        </div>

        <div class="luxury-description-section pt-5">
          <div class="row">
            <div class="col-md-8">
              <div>
                One of the world's most diverse countries, India is home to scores of languages,
                cultures and religions. An in-depth understanding of the Indian domestic market
                is absolutely essential for luxury brands to create an impact here.
              </div>
            </div>
            <div class="col-md-8">
              <div class="pt-4">
                At Crisalid, we understand the nuances of the Indian market.
                Our 360-degree approach is aimed at enriching customer experiences
                and building strong relationships between the customers and your brand.
              </div>
            </div>
          </div>
        </div>

        <div class="row pt-5">
          <div class="col-md-6">
            <div class="global-expertise-section">
              A rare mix of global to local
              and local to global expertise
            </div>
          </div>
        </div>

        <div class="journey-section pt-4">
          We began our journey of redefining luxury in 2019. Our founders, Sandra Howlett &amp; Aishwarya Shinde,
          have a cumulative experience of 30 years in the French and Indian luxury markets.
        </div>

        <div class="experience-section pt-5">
          <div class="row justify-content-between">
            <div class="col-md-5">
              <div class="about-title-section">ABOUT AISHWARYA</div>
              <div class="about-content-section pt-3 pb-4">
                Aishwarya is an experienced creative planner
                with a diverse career in India, comprising
                of key roles in Public Relations, Design and
                Relationship Management. Having studied
                in London and worked with European &amp; Indian
                luxury brands in India, she brings with her the
                'local to global' expertise that are essential for
                International luxury brands to make a mark
                in India.
              </div>
            </div>
            <div class="border-left"></div>
            <div class="col-md-5">
              <div class="about-title-section">ABOUT SANDRA</div>
              <div class="about-content-section pt-3 pb-4">
                Sandra is a luxury experience specialist.
                With an extensive experience of 20 years
                in Paris, she has had the fortune of working
                with some of the world's leading luxury brands. Sandra's experience covers
                but is not limited to managing celebrity clients,
                store launches, recruitment, training &amp; events.
                Now residing in India, she brings with her the
                'global to local' expertise necessary to help
                luxury brands flourish in the Indian market.
              </div>
            </div>
          </div>
        </div>

        <div class="strength-section pt-5">
          <div>Crisalid's strength lies in Aishwarya and Sandra's partnership.</div>
          <div>A combination of European proficiency merged with the knowledge and experience of India.</div>
        </div>
      </div>
    </div>
    <!-- about-us-section end -->
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
.about-us-section {
  .about-us-content {
    .luxury-section {
      font-size: $font-36;
    }
    .global-expertise-section {
      font-size: $font-30;
    }
    .experience-section {
      .about-title-section {
        font-size: $font-30;
      }
    }
  }
}
@import "~/assets/scss/mobile";
</style>