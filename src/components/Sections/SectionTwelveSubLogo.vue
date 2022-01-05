<template>
    <div class="sub-logos page-container">
        <h3>as seen in</h3>
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
</template>

<script>
export default {
data(){
    return{
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
    }
}
}
</script>

<style lang="scss" scoped>
.page-container{
background-color: #000537;
  .sub-logos{
  }
}
</style>