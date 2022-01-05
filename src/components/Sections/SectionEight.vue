<template>
  <div class="page-container">
    <div class="page-title-container">
      <h1 class="page-title">TOKEN SALE</h1>
      <p class="page-title-text">
        The Cryptocurrency industry is one of the Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.
      </p>
    </div>
    <div class="content">
      <v-container>
        <v-row>
          <v-col class="red">
            <div class="items d-flex ">
              <ul>
                <li class="white">
                  <h3>Start</h3>
                  <p>Feb 8, 2018 (9:00AM GMT)</p>
                </li>
                <li>
                  <h3>End</h3>
                  <p>Feb 20, 2018 (11:00AM GMT)</p>
                </li>
                <li>
                  <h3>Acceptable currencies</h3>
                  <p>ETH, BTC, LTC</p>
                </li>
              </ul>
              <ul>
                <li>
                  <h3>Number of tokens for sale</h3>
                  <p>900,000 ICC (9%)</p>
                </li>
                <li>
                  <h3>Tokens exchange rate</h3>
                  <p>1 ETH = 650 ICC, 1 BTC = 1940 ICC</p>
                </li>
                <li>
                  <h3>Minimal transaction amount</h3>
                  <p>1 ETH/ 1 BTC/ 1 LTC</p>
                </li>
              </ul>
            </div>
          </v-col>
          <v-col class="blue d-flex flex-column align-center">
            <v-card>
              <Timer/>
              <v-btn rounded color="red">join & buy token</v-btn>
              <div class="icons d-flex justify-center">
                <i class="fab fa-bitcoin"></i>
                <i class="fas fa-won-sign"></i>
                <i class="fab fa-cc-visa"></i>
                <i class="fab fa-cc-mastercard"></i>
              </div>
            </v-card>
          </v-col>
        </v-row>
      </v-container>
    </div>
  </div>
</template>

<script>
import Timer from '@/components/UI/Timer.vue'
export default {
  data() {
    return {};
  },
  components:{
    Timer
  }
};
</script>

<style lang="scss" scoped>
.page-container {
 
  .content {
    .actions{
      width: 80%;
      background: red;
    }
    
  }
}
</style>
