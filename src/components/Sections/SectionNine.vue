<template>
  <div class="page-container">
    <v-container>
      <v-row>
        <v-col md="6" class=" d-flex flex-column align-center">
          <div class="header-container">
            <h1 class="observe">Distribution of tokens</h1>
          </div>
          <v-img contain src="@/assets/logo/chart-1.png" class="image observe"></v-img>
        </v-col>
        <v-col md="6" class=" d-flex flex-column align-center">
          <div class="header-container">
            <h1 class="observe observe-1">Use of proceeds</h1>
          </div>
          <v-img contain src="@/assets/logo/chart-2.png" class="image observe observe-1"></v-img>
        </v-col>
      </v-row>
    </v-container>
    <base-line class="line"></base-line>
  </div>
</template>

<script>
import BaseLine from "@/components/UI/BaseLine.vue";
export default {
  data() {
    return {};
  },
  components:{
    BaseLine
  }
};
</script>

<style lang="scss" scoped>
.page-container {
  background-color: #0a1992;
  position: relative;
  .header-container{
    display: flex;
    justify-content: center;
    h1 {
      width: 25%;
      min-width: 200px;
      color: #ffffff;
      font-family: "Poppins";
      font-size: 28px;
      font-weight: 600;
      line-height: 36.4px;
      margin-bottom: 50px;
      text-align: center;
      @media only screen and(max-width: 460px){
        font-size: 25px;
        margin-bottom:20px;
        
      }
    }
  }
    .image{
      width: 100%;
      max-width: 690px;
      min-width: 280px;
    }
   .line{
     bottom: -150px;
   }
}
</style>
