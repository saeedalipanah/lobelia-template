<template>
  <div class="navbar">
    <v-app-bar
      app
      elevate-on-scroll
      height="80"
      class="app-bar"
      color="#061162"
    >
      <v-toolbar-title class="text-uppercase">
        <img src="@/assets/logo/logo-white2x.png" alt="" class="logo-image" />
      </v-toolbar-title>
      <v-spacer></v-spacer>
      <v-app-bar-nav-icon
        class="app-bar-icon pa-7"
        color="white"
        @click.stop="drawer = !drawer"
      ></v-app-bar-nav-icon>

      <ul class="nav-items d-flex items-center">
        <li class="nav-button"><a href="#sec-2">WHAT IS ICO</a></li>
        <li class="nav-button"><a href="#sec-8">TOKEN SALE</a></li>
        <li class="nav-button"><a href="#sec-10">ROADMAP</a></li>
        <li class="nav-button"><a href="#sec-11">TEAM</a></li>
        <li class="nav-button"><a href="#sec-12">PARTNERS</a></li>
        <li class="nav-button more-button">
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
        <li class="nav-button" color="white" plain>
          <a href="#sec-15">CONTACT</a>
        </li>
      </ul>

      <v-btn rounded class="end-button mx-4"> whitepaper </v-btn>
      <v-btn rounded class="end-button"> try app </v-btn>
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
  
};
</script>

<style lang="scss" scoped>
.app-bar {
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
        transform: translateY(-20px);
        ul {
          list-style: none;
          li {
            margin: 18px 0;
          }
        }
      }
    }
  }
  .end-button {
    background-color: #0a1992 !important;
    border: 3px solid #3479f5 !important;
    font-size: 12px;
    padding: 16px 20px !important;
    color: white;
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

</style>
