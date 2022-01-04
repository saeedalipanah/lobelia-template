<template>
  <div class="page-container">
    <div class="page-title-container">
      <h1 class="page-title">THE ICO APP</h1>
      <p class="page-title-text">
        The Cryptocurrency industry is one of the Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.
      </p>
    </div>
    <div class="content">
      <v-container>
        <v-row>
          <v-col class="red">
            <v-img src="@/assets/logo/large-dark.png"></v-img>
          </v-col>
          <v-col class="grey">
            <p>
              Lorem ipsum dolor sit amet, consectetur adipis cing elit, sed do
              eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut
              enim ad minim veniam, quis nostrud exerc itation ullamco laboris
              nisi commodo consequat.
            </p>
            <ul>
              <li>Crypto-news curation</li>
              <li>Natural Language Understanding</li>
              <li>Wallet aggregation</li>
              <li>Professional Network</li>
              <li>No more expensive fees</li>
            </ul>
            <div class="actions d-flex justify-space-between ">
              <v-btn rounded>get the app now</v-btn>
              <div class="icons">
                <i class="fab fa-apple"></i>
                <i class="fab fa-android"></i>
                <i class="fab fa-windows"></i>
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
  
  .content {
    .actions{
      width: 80%;
      background: red;
    }
  }
}
ul {
  li {
    &::marker {
      content: "✔   ";
      color: red;
      font-size: 15px;
    }
  }
}
i {
  font-size: 25px;
}
</style>
