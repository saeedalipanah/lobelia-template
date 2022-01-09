<template>
  <div class="page-container">
    <h1 class="title observe">Don't miss out, Stay updated</h1>
    <div class="content">
      <div class="actions observe ">
        <input
          class="input pl-2 pl-sm-6"
          type="email"
          name=""
          id=""
          placeholder="Enter your email"
        />
        <v-btn rounded class="subscribe-button">subscribe</v-btn>
      </div>
      <div class="icons observe">
        <i class="fab fa-facebook-f"></i>
        <i class="fab fa-twitter"></i>
        <i class="fab fa-youtube"></i>
        <i class="fab fa-github"></i>
        <i class="fab fa-bitcoin"></i>
        <i class="fab fa-medium-m"></i>
      </div>
    </div>
    <p class="copy-right text-center observe">
      Copyright © 2019, ICO Crypto. Template Made By Softnio & Handcrafted by
      iO. All trademarks and copyrights belong to their respective owners.
    </p>
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
  // background-color: #000537;
  background: url(//wpdemo.oceanthemes.net/icos-lobelia/wp-content/themes/icos-lobelia/assets/images/footer-bg.png) no-repeat 50% 0%/contain,#10122d;
  .title {
    color: #ffffff;
    font-size: 25px !important;
    font-weight: 500 !important;
    line-height: 28.6px;
    text-align: center;
    font-family: "Poppins";
    margin-top: 50px;
  }
  .content {
    display: flex;
    flex-direction: column;
    align-items: center;
    width: 80%;
      @media only screen and(max-width : 1024px) {
        width: 95%;
      }
    .actions {
      background: #08157a;
      width: 60%;
      max-width: 550px;
      padding: 4px;
      border-radius: 30px;
      display: flex;
      justify-content: space-between;
      margin: 30px 0;
      @media only screen and(max-width : 1024px) {
        width: 100%;
      }
      .input {
        padding: 0;
        width: 50%;
        font-size: 16px;
        font-weight: 500;
          width: 48%;
          min-width: 155px;
        &::placeholder {
          color: rgba(255, 255, 255, 0.623);
        }
        @media only screen and(max-width : 400px) {
          font-size: 14px;
          min-width: 123px;
        }
      }
      .subscribe-button {
        padding: 24px 45px;
        color: white;
        background-image: linear-gradient(to right, #2b56f5 0%, #46bdf4 100%);
        @media only screen and(max-width : 760px) {
          padding: 23px 7% !important;
        }
        @media only screen and(max-width : 400px) {
          padding: 2px 5% !important;
          font-size: 11px;
        }
      }
    }
    .icons {
      .fab {
        margin: 40px 4px 30px 4px;
        font-size: 20px;
        padding: 6px;
        border-radius: 50%;
        background: #262a55;
        color: white;
        &:nth-child(1) {
          padding: 7px 11px;
        }
      }
    }
  }
  .copy-right {
    color: #ffffff;
    font-size: 13px;
    font-weight: 300;
    line-height: 21.84px;
    padding: 0px 0px 3px;
    text-align: center;
    max-width: 550px;
  }
  
}
</style>
