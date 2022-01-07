<template>
  <div class="navbar">
    <v-app-bar
      app
      fixed
      elevate-on-scroll
      height="80"
      class="app-bar"
    >
      <v-toolbar-title class="text-uppercase">
        <img
          src="@/assets/logo/logo-white2x.png"
          alt=""
          class="logo-image animate"
        />
      </v-toolbar-title>
      <v-spacer></v-spacer>
      <v-app-bar-nav-icon
        class="app-bar-icon pa-7"
        color="white"
        @click.stop="drawer = !drawer"
      ></v-app-bar-nav-icon>

      <ul class="nav-items d-flex items-center">
        <li class="nav-button animate"><a href="#sec-2">WHAT IS ICO</a></li>
        <li class="nav-button animate"><a href="#sec-8">TOKEN SALE</a></li>
        <li class="nav-button animate"><a href="#sec-10">ROADMAP</a></li>
        <li class="nav-button animate"><a href="#sec-11">TEAM</a></li>
        <li class="nav-button animate"><a href="#sec-12">PARTNERS</a></li>
        <li class="nav-button animate more-button">
          MORE
          <i class="fas fa-chevron-down"></i>
          <!-- menu items -->
          <div class="menu-items">
            <ul>
              <li><a href="#sec-13">Media Partners</a></li>
              <li><a href="#sec-14">Faqs</a></li>
            </ul>
          </div>
          <!-- end of menu items -->
        </li>
        <li class="nav-button animate" color="white" plain>
          <a href="#sec-15">CONTACT</a>
        </li>
      </ul>

      <v-btn rounded class="end-button mx-4 animate"> whitepaper </v-btn>
      <v-btn rounded class="end-button animate"> try app </v-btn>
    </v-app-bar>

    <!-- navigation-drawer -->
    <v-navigation-drawer
      color="#000751"
      class="navigation-drawer"
      width="340"
      v-model="drawer"
      app
      temporary
    >
      <v-btn
        @click="drawer = !drawer"
        class="mt-2 mx-2 float-right"
        fab
        dark
        small
        color="#33386b"
      >
        <i
          class="fas fa-times white--text"
          style="font-size: 20px; font-weight: 200"
        ></i>
      </v-btn>

      <ul class="drawer-nav-items">
        <li class="drawer-nav-button"><a href="#sec-2">WHAT IS ICO</a></li>
        <li class="drawer-nav-button"><a href="#sec-8">TOKEN SALE</a></li>
        <li class="drawer-nav-button"><a href="#sec-10">ROADMAP</a></li>
        <li class="drawer-nav-button"><a href="#sec-11">TEAM</a></li>
        <li class="drawer-nav-button"><a href="#sec-12">PARTNERS</a></li>
        <li>
          <v-list-group :value="true" no-action class="list-group">
            <template v-slot:activator>
              <v-list-item-title class="white--text title"
                >MORE</v-list-item-title
              >
            </template>
            <li class="white--text px-3" style="font-weight: 300">
              <a href="#sec-13">Media Partners</a>
            </li>
            <li
              class="white--text px-3"
              style="font-weight: 300; border: none; padding-bottom: 0"
            >
              <a href="#sec-14">Faqs</a>
            </li>
          </v-list-group>
        </li>
        <li class="drawer-nav-button" color="white" plain>
          <a href="#sec-15">CONTACT</a>
        </li>
      </ul>
      <v-btn rounded class="end-button mx-4"> whitepaper </v-btn>
      <v-btn rounded class="end-button"> try app </v-btn>
    </v-navigation-drawer>
  </div>
</template>

<script>
export default {
  data() {
    return {
      drawer: false,
    };
  },
  mounted() {
    const navItems = document.querySelectorAll(".animate");
    navItems.forEach((element) => {
      element.classList.add("slide-down");
    });
  },
};
</script>

<style lang="scss" scoped>
.app-bar {
  background: #061162 !important;
  padding: 0 200px;
  @media only screen and(max-width:1390px) {
    padding: 0 30px;
  }
  @media only screen and(max-width:1100px) {
    padding: 0 15px;
  }
  @media only screen and(max-width:1000px) {
    padding: 0 50px;
  }
  @media only screen and(max-width:400px) {
    padding: 0 10px;
  }
  .app-bar-icon {
    display: none;
    @media only screen and(max-width:1000px) {
      display: flex !important;
    }
  }
  .logo-image {
    width: 11.3125rem;
    height: 2.5rem;
    @media only screen and(max-width:1200px) {
      width: 9.0625rem;
      height: 2rem;
    }
  }
  .nav-items {
    cursor: pointer;
    list-style: none;
    padding-left: 0;
    @media only screen and(max-width:1000px) {
      display: none !important;
    }
    .nav-button {
      transform: translateY(-80px);
      a {
        color: white;
        text-decoration: none;
        &:hover {
          color: #018ff2;
        }
      }
      color: white !important;
      padding: 20px 8px !important;
      font-size: 12px;
      font-weight: 500;
      position: relative;
      @media only screen and(max-width:1200px) {
        padding: 0px 4px;
      }
      &.more-button {
        &:hover {
          color: #018ff2 !important;
          .menu-items {
            height: 100px;
            opacity: 1;
            transform: none;
            color: #018ff2;
          }
        }
      }
      .menu-items {
        transition: all 0.3s ease;
        position: absolute;
        top: 60px;
        left: 0;
        background: #06116f;
        border-radius: 4px;
        width: 230px;
        opacity: 0;
        height: 90px;
        overflow: hidden;
        ul {
          list-style: none;
          li {
            margin: 18px 0;
          }
        }
      }
    }
  }
  .slide-down {
    animation: moveDown 1s ease forwards;
    &:nth-child(2) {
      animation-delay: 0.05s;
    }
    &:nth-child(3) {
      animation-delay: 0.1s;
    }
    &:nth-child(4) {
      animation-delay: 0.15s;
    }
    &:nth-child(5) {
      animation-delay: 0.2s;
    }
    &:nth-child(6) {
      animation-delay: 0.25s;
    }
    &:nth-child(7) {
      animation-delay: 0.3s;
    }
    &:nth-child(8) {
      animation-delay: 0.35s;
    }
    &:nth-child(9) {
      animation-delay: 0.4s;
    }
    &:nth-child(10) {
      animation-delay: 0.45s;
    }
  }
  .end-button {
    background-color: #0a1992 !important;
    border: 3px solid #3479f5 !important;
    font-size: 12px;
    padding: 16px 20px !important;
    color: white;
    transform: translateY(-80px);
    @media only screen and(max-width:1000px) {
      display: none !important;
    }
    &:hover {
      transition: all 0.5s ease;
      background-color: #3479f5 !important;
    }
  }
}
.navigation-drawer {
  width: 40% !important;
  min-width: 260px;
  max-width: 340px;
  .drawer-nav-items {
    list-style: none;
    padding: 12px 25px;
    padding-top: 50px;
    li {
      a {
        color: white;
        text-decoration: none;
      }
      font-size: 12px;
      font-weight: 500;
      line-height: 16.8px;
      padding: 12px 0;
      color: white;
      border-bottom: 1px solid rgba(219, 228, 247, 0.1);
    }
  }
  .end-button {
    background-color: #0a1992 !important;
    border: 3px solid #3479f5 !important;
    padding: 14px 10px !important;
    font-size: 12px;
    color: white;
  }
  .list-group {
    ::v-deep {
      .v-list-item--link {
        &::before {
          background: transparent !important;
        }
      }
    }
    ::v-deep {
      .v-icon.v-icon {
        color: white;
        font-size: 17px;
      }
    }
    .title {
      font-size: 12px !important;
    }
    ::v-deep {
      .v-list-item {
        padding: 0;
        min-height: 0;
      }
    }
  }
}
@keyframes moveDown {
  0% {
    transform: translateY(-80px);
    opacity: 0;
  }
  100% {
    transform: translateY(0);
    opacity: 1;
  }
}
</style>
