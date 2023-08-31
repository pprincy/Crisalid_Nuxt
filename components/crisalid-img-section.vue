<template>
  <div class="crisalid-section">
    <div class="d-flex justify-content-between white fixed-bottom p-4">
      <div v-for="cris in crisalid" v-bind:key="cris.name">
        <div :class="cris.crisalidLogo">
          <nuxt-link :to="cris.link">
            <div class="first-name" v-html="cris.name"></div>
            <div v-if="!cris.name">
              <div class="crisalid-home-section">
                <b-img :src="cris.img" class="crisalid-logo-section" alt="logo" />
              </div>
            </div>
            <span></span>
          </nuxt-link>
        </div>
      </div>
    </div>
  </div>
</template>
<script>
import crisLogo from "~/assets/images/crisalid-logo-opaque.png";



export default {
  data() {
    return {
      crisalid: [
        {
          name: "vision",
          link: "/vision"
        },
        {
          crisalidLogo: "crisalid-logo",
          img: crisLogo,
          link: "/crisalid"
        },
        {
          name: "mission",
          link: "/mission"
        }
      ]
    };
  }
};
</script>
<style lang="scss">
@import "~/assets/scss/variable";
.crisalid-section {
  font-size: $font-30;
  .crisalid-home-section {
    width: 100px;
    height: 50%;

    .crisalid-logo-section {
      width: 100%;
      height: 100%;
    }
  }

  a {
    color: $white;
    text-decoration: none;
    background-color: transparent;
    span {
      width: 16px;
      margin-top: -10px;
      display: block;
      margin-left: 2px;
      border-bottom: 1.5px solid transparent;
    }
  }
  a:hover {
    color: $white;
    text-decoration: none;
  }
  .nuxt-link-exact-active {
    span:nth-child(even) {
      border-bottom-color: $white;
    }
  }
  //   .first-name:first-letter {
  //       border-bottom-color: $white;

  // }
}
</style>