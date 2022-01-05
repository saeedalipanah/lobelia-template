<template>
  <div class="sub-logos page-container">
    <h3 class="observe">as seen in</h3>
    <v-container fluid>
      <v-row justify="center">
        <v-col class="" cols="6" sm="2" v-for="(logo, i) in subLogos" :key="i">
          <v-img :src="logo.url" class="observe" :class="`delay-${i}`"></v-img>
        </v-col>
      </v-row>
    </v-container>
  </div>
</template>

<script>
export default {
  data() {
    return {
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
.page-container {
  h3 {
    color: #ffffff;
    font-size: 14.08px;
    font-weight: 600;
    letter-spacing: 2.816px;
    line-height: 18.304px;
    text-align: center;
    text-transform: uppercase;
    margin-bottom: 20px;
  }
  background-color: #000537;
  .delay-1 {
    transition-delay: 0.2 !important;
  }
  .delay-2 {
    transition-delay: 0.4s !important;
  }
  .delay-3 {
    transition-delay: 0.6s !important;
  }
  .delay-4 {
    transition-delay: 0.8s !important;
  }
  .delay-5 {
    transition-delay: 1s !important;
  }
  .delay-6 {
    transition-delay: 0.2s !important;
  }
  .delay-7 {
    transition-delay: 0.4s !important;
  }
  .delay-8 {
    transition-delay: 0.6s !important;
  }
  .delay-9 {
    transition-delay: 0.8s !important;
  }
}
</style>
