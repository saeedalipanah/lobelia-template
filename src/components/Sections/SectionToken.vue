<template>
  <div class="page-container">
    <div class="page-title-container">
      <h1 class="page-title observe">TOKEN SALE</h1>
      <p class="page-title-text observe">
        The Cryptocurrency industry is one of the Lorem ipsum dolor sit amet,
        consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore
        et dolore magna aliqua.
      </p>
    </div>
    <div class="content">
      <v-container>
        <v-row>
          <v-col class="d-flex justify-center">
            <div class="items d-flex">
              <ul>
                <li class="observe">
                  <h3>Start</h3>
                  <p>Feb 8, 2018 (9:00AM GMT)</p>
                </li>
                <li class="observe">
                  <h3>End</h3>
                  <p>Feb 20, 2018 (11:00AM GMT)</p>
                </li>
                <li class="observe">
                  <h3>Acceptable currencies</h3>
                  <p>ETH, BTC, LTC</p>
                </li>
              </ul>
              <ul>
                <li class="observe observe-1">
                  <h3>Number of tokens for sale</h3>
                  <p>900,000 ICC (9%)</p>
                </li>
                <li class="observe observe-1">
                  <h3>Tokens exchange rate</h3>
                  <p>1 ETH = 650 ICC, 1 BTC = 1940 ICC</p>
                </li>
                <li class="observe observe-1">
                  <h3>Minimal transaction amount</h3>
                  <p>1 ETH/ 1 BTC/ 1 LTC</p>
                </li>
              </ul>
            </div>
          </v-col>
          <v-col class="d-flex flex-column align-center justify-center">
            <v-card class="card px-5 py-9 observe observe-2">
              <Timer class="" />
              <div class="d-flex flex-column align-center">
                <v-btn class="btn mt-4" rounded>join & buy token</v-btn>
                <div class="icons d-flex justify-center mt-4">
                  <i class="fab fa-bitcoin"></i>
                  <i class="fas fa-won-sign"></i>
                  <i class="fab fa-cc-visa"></i>
                  <i class="fab fa-cc-mastercard"></i>
                </div>
              </div>
            </v-card>
          </v-col>
        </v-row>
      </v-container>
    </div>
  </div>
</template>

<script>
import Timer from "@/components/UI/Timer.vue";
export default {
  data() {
    return {};
  },
  components: {
    Timer,
  },
};
</script>

<style lang="scss" scoped>
.page-container {
  background-color: #0a1992;
  padding-bottom: 0;
  .page-title {
    position: relative;
    &::before {
      content: "token";
      position: absolute;
      opacity: 0.04;
      font-size: 130px;
      text-transform: uppercase;
      font-weight: 900;
      left: -50%;
      right: -50%;
    }
  }
  .content {
    .items {
      ul {
        li {
          min-height: 100px;
          margin: 20px;
          h3 {
            color: #ffffff;
            font-size: 17.6px;
            font-weight: 600;
            line-height: 22.88px;
            // margin: 0px 0px 8px;
            text-align: left;
          }
          p {
            color: #d2d3ff;
            font-size: 15px;
            font-weight: 300;
            line-height: 25.2px;
            text-align: left;
          }
          &::marker {
            color: #2b56f5;
          }
        }
      }
    }
    .card {
      background: #08157a;
      .btn {
        background-image: linear-gradient(to right, #7a0fff 0%, #2b56f5 100%);
        color: #ffffff;
        font-size: 12px;
        font-weight: 500;
        letter-spacing: 1.2px;
        line-height: 24px;
        padding: 22px 30px;
        text-align: center;
        text-transform: uppercase;
      }
      .fab,
      .fas {
        color: #f5f7fe;
        font-size: 17px;
        font-weight: 300;
        line-height: 26.88px;
        text-align: left;
        margin: 0 5px;
      }
    }
  }
}
</style>
