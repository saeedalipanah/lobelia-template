<template>
  <div class="page-container">
    <v-container>
      <v-row>
        <v-col md="6" class=" d-flex flex-column align-center">
          <div class="header-container">
            <h1>Distribution of tokens</h1>
          </div>
          <v-img contain src="@/assets/logo/chart-1.png" class="image"></v-img>
        </v-col>
        <v-col md="6" class=" d-flex flex-column align-center">
          <div class="header-container">
            <h1>Use of proceeds</h1>
          </div>
          <v-img contain src="@/assets/logo/chart-2.png" class="image"></v-img>
        </v-col>
      </v-row>
    </v-container>
  </div>
</template>

<script>
export default {
  data() {
    return {};
  },
};
</script>

<style lang="scss" scoped>
.page-container {
  background-color: #0a1992;
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
}
</style>
