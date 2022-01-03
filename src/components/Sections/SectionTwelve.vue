<template>
  <div class="contanier blue lighten-2">
    <div class="section-1 red lighten-4">
      <div class="title">
        <h1>ICO CRYPRO PARTNERS</h1>
        <p>
          The Cryptocurrency industry is one of the Lorem ipsum dolor sit amet,
          consectetur adipiscing elit, sed do eiusmod tempor incididunt ut
          labore et dolore magna aliqua.
        </p>
      </div>
      <div class="main-logos">
        <v-container>
          <v-row justify="center">
            <v-col
              class=""
              cols="6"
              md="4"
              v-for="(logo, i) in mainLogos"
              :key="i"
            >
              <v-img :src="logo.url"></v-img>
            </v-col>
          </v-row>
        </v-container>
      </div>
    </div>
    <div class="sub-logos">
      <v-container fluid>
        <v-row justify="center">
          <v-col
            class=""
            cols="6"
            sm="2"
            v-for="(logo, i) in subLogos"
            :key="i"
          >
            <v-img :src="logo.url"></v-img>
          </v-col>
        </v-row>
      </v-container>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      mainLogos: [
        {
          url: "https://demo.themenio.com/ico/images/partners/a-md.png",
        },
        {
          url: "https://demo.themenio.com/ico/images/partners/b-md.png",
        },
        {
          url: "https://demo.themenio.com/ico/images/partners/c-md.png",
        },
        {
          url: "https://demo.themenio.com/ico/images/partners/d-md.png",
        },
        {
          url: "https://demo.themenio.com/ico/images/partners/d-md.png",
        },
      ],
      subLogos: [
        {
          url: "https://demo.themenio.com/ico/images/partners/a-xs-light.png",
        },
        {
          url: "https://demo.themenio.com/ico/images/partners/b-xs-light.png",
        },
        {
          url: "https://demo.themenio.com/ico/images/partners/c-xs-light.png",
        },
        {
          url: "https://demo.themenio.com/ico/images/partners/d-xs-light.png",
        },
        {
          url: "https://demo.themenio.com/ico/images/partners/e-xs-light.png",
        },
        {
          url: "https://demo.themenio.com/ico/images/partners/f-xs-light.png",
        },
        {
          url: "https://demo.themenio.com/ico/images/partners/a-sm-light.png",
        },
        {
          url: "https://demo.themenio.com/ico/images/partners/b-sm-light.png",
        },
        {
          url: "https://demo.themenio.com/ico/images/partners/c-sm-light.png",
        },
        {
          url: "https://demo.themenio.com/ico/images/partners/d-sm-light.png",
        },
      ],
    };
  },
};
</script>

<style lang="scss" scoped>
.contanier {
  .title {
    display: flex;
    flex-direction: column;
    align-items: center;
    text-align: center;
  }
}
</style>
