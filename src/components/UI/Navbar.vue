<template>
  <div class="navbar">
    <v-app-bar app elevate-on-scroll height="90" class="app-bar">
      <v-toolbar-title class="text-uppercase">
        <img src="@/assets/logo/logo-white2x.png" alt="" class="logo-image" />
      </v-toolbar-title>
      <v-spacer></v-spacer>
      <v-app-bar-nav-icon
        class="app-bar-icon pa-7"
        color="white"
        @click.stop="drawer = !drawer"
      ></v-app-bar-nav-icon>

      <ul class="nav-items d-flex items-center ">
        <li class="nav-button">WHAT IS ICO</li>
        <li class="nav-button" >TOKEN SALE</li>
        <li class="nav-button" >ROADMAP</li>
        <li class="nav-button" >TEAM</li>
        <li class="nav-button" >PARTNERS</li>
        <li>

        <v-menu offset-y>
          <template v-slot:activator="{ on, attrs }">
            <v-btn
              class=""
              color="grey lighten-2"
              dark
              v-bind="attrs"
              v-on="on"
              plain
            >
              more
              <v-icon color="grey darken-2" left right>mdi-chevron-down</v-icon>
            </v-btn>
          </template>
          <v-list>
            <v-list-item>
              <v-list-item-title
                style="cursor: pointer"
                @click="changeLanguage('en')"
                >English</v-list-item-title
              >
            </v-list-item>
            <v-list-item>
              <v-list-item-title
                style="cursor: pointer"
                @click="changeLanguage('fa')"
                >فارسی</v-list-item-title
              >
            </v-list-item>
          </v-list>
        </v-menu>
        </li>
        <li class="nav-button" color="white" plain>contact</li>
      </ul>
      <v-btn rounded color="primary" dark class="end-button mx-4 "> Button </v-btn>
      <v-btn rounded color="primary" dark class="end-button  "> Button </v-btn>
    </v-app-bar>
  </div>
</template>

<script>
export default {};
</script>

<style lang="scss" scoped>
.app-bar {
  background-color: #06116f !important;
  padding: 0 60px;
    @media only screen and(max-width:1100px) {
      padding: 0 15px;
    }
    @media only screen and(max-width:990px) {
      padding: 0 50px;
    }
  .app-bar-icon {
    display: none;
    @media only screen and(max-width:990px) {
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
    list-style: none;
    padding-left: 0;
    @media only screen and(max-width:990px) {
      display: none !important;
    }
    .nav-button {
      color: white !important;
      padding: 2px 8px;
      font-size: 12px;
      @media only screen and(max-width:1200px) {
        padding: 2px 4px;
      }
    }
  }
  .end-button {
    border: 2px solid red !important;
    @media only screen and(max-width:990px) {
      display: none !important;
    }
  }
}
</style>
