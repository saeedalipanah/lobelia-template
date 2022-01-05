<template>
  <div class="page-container">
    <h1 class="title">Don't miss out, Stay updated</h1>
    <div class="content">
      <div class="actions">
        <input
          class="input pl-6"
          type="email"
          name=""
          id=""
          placeholder="Enter your email"
        />
        <v-btn rounded class="subscribe-button">subscribe</v-btn>
      </div>
      <div class="icons">
        <i class="fab fa-facebook-f"></i>
        <i class="fab fa-twitter"></i>
        <i class="fab fa-youtube"></i>
        <i class="fab fa-github"></i>
        <i class="fab fa-bitcoin"></i>
        <i class="fab fa-medium-m"></i>
      </div>
    </div>
    <p class="copy-right text-center">
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
  background-color: #000537;
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
    width: 100%;
    .actions {
      background: #08157a;
      min-width: 580px;
      padding: 4px;
      border-radius: 30px;
      display: flex;
      justify-content: space-between;
      width: 500px;
      margin: 30px 0;
      @media only screen and(max-width : 760px) {
        width: 100%;
      }
      .input {
        padding: 0;
        width: 50%;
        font-size: 16px;
        font-weight: 500;
        &::placeholder {
          color: rgba(255, 255, 255, 0.623);
        }
        @media only screen and(max-width : 760px) {
          width: 28%;
          min-width: 152px;
        }
      }
      .subscribe-button {
        padding: 24px 45px;
        color: white;
        background-image: linear-gradient(to right, #2b56f5 0%, #46bdf4 100%);
        @media only screen and(max-width : 760px) {
          padding: 23px 7% !important;
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
