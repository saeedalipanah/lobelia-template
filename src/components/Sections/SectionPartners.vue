<template>
  <div class="page-container">
      <div class="page-title-container">
        <h1 class="page-title observe">ICO CRYPRO PARTNERS</h1>
        <p class="page-title-text observe">
          The Cryptocurrency industry is one of the Lorem ipsum dolor sit amet,
          consectetur adipiscing elit, sed do eiusmod tempor incididunt ut
          labore et dolore magna aliqua.
        </p>
      </div>
    <div class="section-1">
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
              <v-img :src="logo.url" class="partners-img observe" :class="`observe-${i+1}`"></v-img>
            </v-col>
          </v-row>
        </v-container>
      </div>
    </div>
      <base-line class="line"></base-line>
  </div>
</template>

<script>
import BaseLine from "@/components/UI/BaseLine.vue";
export default {
components:{
  BaseLine
},
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
      
    };
  },
};
</script>

<style lang="scss" scoped>
.page-container{
  background-color: #0a1992;
    .page-title{
    position: relative;
    &::before{
      content: 'partners';
    }
  }
  .partners-image{
    min-height: 110px;
    @media only screen and(max-width: 800px){
      min-height: 46px;
    }
  }
}
</style>
