<template>
  <div class="service-section main-bg">
    <!-- header section component start -->
    <header-section></header-section>
    <!-- header section component end -->
    <!-- service section start -->
    <div class="service-content white pt-90 pb-5">
      <div class="container">
        <!-- service description start -->
        <div class="service-details">
          <div>
            <div>
              <div class="service-title-section">Our Services</div>
            </div>
          </div>
          <div class="pt-4">
            <div>
              <p>
                At Crisalid, our core is 'Experience'. Our offers aim to impart the necessary tools
                to equip your company to provide exceptional experiences.
              </p>
              <p>
                Our services span an array of areas for companies within the Luxury Universe.
                We train existing company staff with relevant modules in order to equip
                employees to provide the best brand experience.
              </p>
              <p>
                Along with training, we assist in recruitment to help provide skilled staff
                suitable for the required position.
              </p>
              <p>
                We strive to provide exceptional CRM Events. Crisalid will take care of every step
                from planning to execution, to ensure a flawless experience for your clients.
              </p>
            </div>
          </div>
        </div>
        <!-- service description end -->
        <!-- consulting and training section -->
        <div class="training-section py-3">
          <div class="row justify-content-center pb-1">
            <div class="col-md-6">
              <div class="training-title-section">CONSULTING</div>
              <div class="pt-3">
                <p>
                  Customer Experience centric
                  advice on luxury fashion, lifestyle,
                  hospitality for entities existing in India
                </p>
                <p>Understanding Indian consumers</p>
                <ul class="list-unstyled">
                  Analysis of current scenario
                  <div class="training-content">
                    <li>
                      - Understand brand DNA,
                      history &amp; culture
                    </li>
                    <li>
                      - Identity areas of concern
                      within retail entity
                    </li>
                    <li>
                      - Comprehend expected
                      objectives
                    </li>
                  </div>
                </ul>
              </div>
            </div>
            <div class="col-md-6">
              <div class="training-title-section">TRAINING</div>
              <div class="pt-3">
                <p>
                  Tailor made Retail Excellence
                  training programs
                </p>
                <p>Digital Training Programs</p>
                <p>Education Programs</p>
                <p>
                  Solutions customized to
                  client needs
                </p>
                <p>
                  Follow up &amp; maintenance
                  for continued success
                </p>
              </div>
            </div>
          </div>
          <div>
            <div>
              <div class="border-bottom"></div>
            </div>
          </div>
        </div>
        <!-- consulting and training end -->
        <!-- recruitment and crm section -->
        <div class="crm-section py-3">
          <div class="row justify-content-center">
            <div class="col-md-6">
              <div class="crm-title-section">RECRUITMENT</div>
              <div class="pt-3">
                <ul class="list-unstyled">
                  Identity and provide
                  efficient talent
                  <li class="crm-content">- right people for the right position</li>
                </ul>
              </div>
            </div>
            <div class="col-md-6">
              <div class="crm-title-section">CRM EVENTS</div>
              <div class="pt-3">
                Organizing customer
                focused events from
                inspiration to execution
              </div>
            </div>
          </div>
        </div>
        <!-- recruitment and crm end -->
      </div>
    </div>
    <!-- service section end -->
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
.service-section {
  .service-content {
    .service-details {
      .service-title-section {
        font-size: $font-40;
      }
    }
  }
  .training-section {
    .training-title-section {
      font-size: $font-18;
    }
  }
  .crm-section {
    .crm-title-section {
      font-size: $font-18;
      
    }
  }
}
@import "~/assets/scss/mobile";
</style>