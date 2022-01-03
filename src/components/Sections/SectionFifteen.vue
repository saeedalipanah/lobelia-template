<template>
  <div class="container">
    <div class="title">
      <h1>Don't miss out, Stay updated</h1>
    </div>
    <div class="content">
      <div class="actions">
        <input
          class="px-6"
          type="email"
          name=""
          id=""
          placeholder="Enter your email"
        />
        <v-btn rounded class="px-10 py-6">submit</v-btn>
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
    return {
      
    };
  },
};
</script>

<style lang="scss" scoped>
.container {
  .title {
    display: flex;
    flex-direction: column;
    align-items: center;
    text-align: center;
  }
  .content {
    display: flex;
    flex-direction: column;
    align-items: center;
    .actions {
      background: red;
      width: 60%;
      padding: 4px;
      border-radius: 30px;
      display: flex;
      justify-content: space-between;
      overflow: hidden;
    }
    .icons {
      .fab {
        margin: 0 4px;
        font-size: 20px;
        padding: 10px;
        border-radius: 50%;
        background: rgb(21, 21, 107);
        color: white;
        &:nth-child(1) {
          padding: 10px 15px;
        }
      }
    }
  }
}
</style>
