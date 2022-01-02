<template>
<div class="navbar">
  <v-app-bar app elevate-on-scroll height="90" class="app-bar">
    <v-app-bar-nav-icon
      class="app-bar-icon pa-7"
      @click.stop="drawer = !drawer"
    ></v-app-bar-nav-icon>
    <v-toolbar-title class="text-uppercase grey--text text-h5">
      <img src="@/assets/logo/logo-white2x.png" alt="" class="logo-image" />
    </v-toolbar-title>
    <v-spacer></v-spacer>
    <div class="nav-items">
      <v-btn class="nav-button" color="white" plain>WHAT IS ICO</v-btn>
      <v-btn class="nav-button" color="white" plain>TOKEN SALE</v-btn>
      <v-btn class="nav-button" color="white" plain>ROADMAP</v-btn>
      <v-btn class="nav-button" color="white" plain>TEAM</v-btn>
      <v-btn class="nav-button" color="white" plain>PARTNERS</v-btn>
    <v-menu offset-y>
      <template v-slot:activator="{ on, attrs }">
        <v-btn
          class="text-lowercase mx-2 grey--text"
          color="grey lighten-2"
          dark
          v-bind="attrs"
          v-on="on"
          plain
        >
         
          fsdafa
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
    <v-btn class="nav-button" color="white" plain>contact</v-btn>
    </div>
    <v-btn
      rounded
      color="primary"
      dark
      class="end-button"
    >
       Button
    </v-btn>
    <v-btn
      rounded
      color="primary"
      dark
    >
       Button
    </v-btn>
  </v-app-bar>
</div>
</template>

<script>
export default {};
</script>

<style lang="scss" scoped>
.app-bar {
  background-color: #06116f !important;
  .app-bar-icon {
    display: none;
    color: white !important;
    @media only screen and(max-width:800px) {
      display: block;
    }
  }
  .logo-image {
    width: 142px;
    height: 32px;
  }
  .nav-items {
    .nav-button {
      padding: 2px 10px;
    }
  }
  .end-button{
    border: 2px solid red !important;
  }
}
</style>
