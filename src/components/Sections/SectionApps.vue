<template>
  <div class="page-container">
    <div class="page-title-container">
      <h1 class="page-title observe">THE ICO APP</h1>
      <p class="page-title-text observe">
        The Cryptocurrency industry is one of the Lorem ipsum dolor sit amet,
        consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore
        et dolore magna aliqua.
      </p>
    </div>
    <div class="content">
      <v-container>
        <v-row>
          <v-col cols="12" sm="6" class="d-flex justify-center align-end">
            <v-img
              class="image observe"
              contain
              src="@/assets/logo/large-dark.png"
            ></v-img>
          </v-col>
          <v-col cols="12" sm="6" class="d-flex flex-column justify-center">
            <div class="text">
              <p class="observe">
                Lorem ipsum dolor sit amet, consectetur adipis cing elit, sed do
                eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut
                enim ad minim veniam, quis nostrud exerc itation ullamco laboris
                nisi commodo consequat.
              </p>
              <ul>
                <li class="observe">Crypto-news curation</li>
                <li class="observe">Natural Language Understanding</li>
                <li class="observe">Wallet aggregation</li>
                <li class="observe">Professional Network</li>
                <li class="observe">No more expensive fees</li>
              </ul>
              <div class="actions d-flex align-center">
                <v-btn class="btn observe" rounded>get the app now</v-btn>
                <div class="icons observe observe-1">
                  <i class="fab fa-apple"></i>
                  <i class="fab fa-android"></i>
                  <i class="fab fa-windows"></i>
                </div>
              </div>
            </div>
          </v-col>
        </v-row>
      </v-container>
    </div>
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
  background-color: #000537;
  .page-title {
    position: relative;
    &::before {
      content: "apps";
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
    .image {
      width: 100%;
      max-width: 400px !important;
      min-height: 500px;
      @media only screen and(max-width : 420px) {
        width: 70%;
        height: 70%;
      }
    }
    .text {
      width: 100%;
      p {
        color: #d2d3ff;
        font-size: 15px;
        font-weight: 300;
        line-height: 25.2px;
        text-align: left;
      }
      ul {
        li {
          color: #d2d3ff;
          display: list-item;
          font-size: 15px;
          font-weight: 300;
          line-height: 22.68px;
          padding: 5px 0px 5px 10px;
          text-align: left;
          &::marker {
            content: "✔   ";
            font-size: 15px;
          }
        }
      }
    }
    .actions {
      margin: 20px 0;
      .btn {
        margin-right: 20px;
        background-image: linear-gradient(to right, #46bdf4 0%, #2b56f5 100%);
        color: #ffffff;
        font-size: 12px;
        font-weight: 500;
        letter-spacing: 1.2px;
        line-height: 24px;
        padding: 20px 30px;
        text-align: center;
        text-transform: uppercase;
      }
    }
  }
}

i {
  font-size: 15px;
  color: white;
  margin: 0 5px;
}
</style>
