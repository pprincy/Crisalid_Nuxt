<template>
  <div class="header-section">
    <div class="d-flex justify-content-between header-fixed fixed-top px-4 py-2">
      <!-- logo section start -->

      <div class="logo cursor-pointer pt-2">
        <nuxt-link to="/">
          <b-img src="~/assets/images/crisalid-logo.png" class="logo-section" alt="logo" />

        </nuxt-link>
      </div>

      <!-- logo section end -->

      <!-- hamburger section start -->
      <div
        class="hamburger cursor-pointer pt-1"
        @click="headerMenu()"
        v-bind:class="{'close':show}"
      >
        <div class="bar1"></div>
        <div class="bar2"></div>
        <div class="bar3"></div>
      </div>
      <!-- hamburger section end -->
    </div>

    <!-- navigation section start -->
    <div class="nav-hide fixed-top" v-bind:class="{'nav-show':show}">
      <div class="header-bg-section">
        <div class="header-menu-section">
          <!-- <div class="close text-right text-white cursor-pointer" @click="headerMenu()">close</div> -->
          <div>
            <ul class="pl-0 pt-5">
              <li
                v-for="navigation in navigations"
                v-bind:key="navigation.name"
                class="inside-game"
              >
                <div v-if="navigation.link">
                  <nuxt-link :to="navigation.link">{{navigation.name}}</nuxt-link>
                </div>
                <div v-if="!navigation.link">
                  <a
                    href="mailto:luxuryexperience@crisalidindia.com?subject=Website: Connecting with Crisalid India"
                  >{{navigation.name}}</a>
                </div>
              </li>
            </ul>
          </div>
        </div>
      </div>
    </div>
    <!-- navigation section end -->
  </div>
</template>
<script>
export default {
  data() {
    return {
      show: false,
      navigations: [
        {
          name: "home",
          link: "/"
        },
        {
          name: "about",
          link: "/about-us"
        },
        {
          name: "services",
          link: "/service"
        },
        {
          name: "contact us",
          email: ""
        },
        {
          name: "work with us",
          link: "/work-with-us"
        }
      ]
    };
  },
  methods: {
    headerMenu() {
      this.show = !this.show;
    }
  }
};
</script>
<style lang="scss">
@import "~/assets/scss/variable";

.header-section {
  color: $white;
  // position: fixed;
  // width: 100%;
  // height: 100vh;
  // z-index: 999;
  // top: 0;
  .header-fixed {
    z-index: 1031;
    background: $bg-black;
  }
  .nav-hide {
    top: 0;
    transition: all ease 300ms;
    transform: translateY(-150%);
    &.nav-show {
      transform: translateY(0);
    }
  }
  .logo {
    width: 40px;
    .logo-section {
      width: 100%;
    }
  }
  .hamburger {
    .bar1,
    .bar2,
    .bar3 {
      height: 5px;
      border-radius: 15px;
      margin: 6px 0;
      background-color: $white;
      transition: all ease 500ms;
    }
    .bar1 {
      width: 35px;
    }
    .bar2 {
      width: 25px;
    }
    .bar3 {
      width: 15px;
    }
    &.close {
      .bar1,
      .bar2,
      .bar3 {
        width: 25px;
        transform-origin: -5%;
      }
      .bar1 {
        transform: rotate(52deg);
      }
      .bar2 {
        opacity: 0;
      }
      .bar3 {
        transform: rotate(-52deg);
      }
    }
  }
  .header-bg-section {
    background: url("~@/assets/images/bg-blur-img.jpg") no-repeat center center
      $bg-black;
    background-size: contain;
    position: relative;
    height: 100vh;
    padding-top: 100px;

    .header-menu-section {
      border: 2px solid $white;
      width: 50%;
      margin: 0px auto 0;
      font-size: $font-26;
      padding: 40px;
      text-align: center;

      a {
        color: $white;
        &:hover {
          text-decoration: none;
        }
      }

      ul li {
        position: relative;
        text-decoration: none;
        list-style: none;
        padding: 8px;
        &::after {
          content: "";
          position: absolute;
          left: 48%;
          bottom: 0;
          width: 16px;
          border-radius: 20px;
          background-color: $white;
          border: 1px solid $white;
        }
      }
    }
  }
}

@import "~/assets/scss/mobile";
</style>