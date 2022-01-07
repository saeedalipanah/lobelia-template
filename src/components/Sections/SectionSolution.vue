<template>
  <div class="page-container">
    <div class="page-title-container">
      <h1 class="page-title observe">THE CRYPTO SOLUTION</h1>
      <p class="page-title-text observe">
        The Cryptocurrency industry is one of the Lorem ipsum dolor sit amet,
        consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore
        et dolore magna aliqua.
      </p>
    </div>
    <div class="content">
      <v-container>
        <v-row>
          <v-col
            cols="12"
            sm="6"
            md="3"
            class=""
            v-for="(item, i) in items"
            :key="i"
          >
            <div
              class="content d-flex flex-column align-center justify-center observe"
              :class="`observe-${i}`"
            >
              <v-img
                :src="item.iconUrl"
                max-width="60"
                max-height="60"
                class=""
              ></v-img>
              <h3 class="">{{ item.title }}</h3>
              <p class="text-center">{{ item.textContent }}</p>
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
    return {
      items: [
        {
          iconUrl:
            "http://wpdemo.oceanthemes.net/icos-lobelia/wp-content/uploads/sites/25/2018/06/icon-relational-blockchain.png",
          title: "Relational Blockchain",
          textContent:
            "Contributors and members est et expedita distinctio. Nam libero tempore",
        },
        {
          iconUrl:
            "http://wpdemo.oceanthemes.net/icos-lobelia/wp-content/uploads/sites/25/2018/06/icon-fund.png",
          title: "Fraud Reduction",
          textContent:
            "Contributors and members est et expedita distinctio. Nam libero tempore",
        },
        {
          iconUrl:
            "http://wpdemo.oceanthemes.net/icos-lobelia/wp-content/uploads/sites/25/2018/06/icon-wallet.png",
          title: "Next Generation Wallet",
          textContent:
            "Contributors and members est et expedita distinctio. Nam libero tempore",
        },
        {
          iconUrl:
            "http://wpdemo.oceanthemes.net/icos-lobelia/wp-content/uploads/sites/25/2018/06/icon-server.png",
          title: "Recovery Nodes",
          textContent:
            "Contributors and members est et expedita distinctio. Nam libero tempore",
        },
        {
          iconUrl:
            "http://wpdemo.oceanthemes.net/icos-lobelia/wp-content/uploads/sites/25/2018/06/icon-connect.png",
          title: "Relational Blockchain",
          textContent:
            "Contributors and members est et expedita distinctio. Nam libero tempore",
        },
        {
          iconUrl:
            "http://wpdemo.oceanthemes.net/icos-lobelia/wp-content/uploads/sites/25/2018/06/icon-cash.png",
          title: "Fraud Reduction",
          textContent:
            "Contributors and members est et expedita distinctio. Nam libero tempore",
        },
        {
          iconUrl:
            "http://wpdemo.oceanthemes.net/icos-lobelia/wp-content/uploads/sites/25/2018/06/icon-decentralize-network.png",
          title: "Next Generation Wallet",
          textContent:
            "Contributors and members est et expedita distinctio. Nam libero tempore",
        },
        {
          iconUrl:
            "http://wpdemo.oceanthemes.net/icos-lobelia/wp-content/uploads/sites/25/2018/06/icon-crypto-currency.png",
          title: "Recovery Nodes",
          textContent:
            "Contributors and members est et expedita distinctio. Nam libero tempore",
        },
      ],
    };
  },
};
</script>

<style lang="scss" scoped>
.page-container {
  background-color: #0a1992;
  .page-title {
    position: relative;
    &::before {
      content: "solution";
    }
  }
  .content {
    h3 {
      color: #ffffff;
      font-size: 18px;
      font-weight: 600;
      line-height: 23.4px;
      margin: 13.6px 0px;
      text-align: center;
    }
    p {
      color: #d2d3ff;
      font-size: 15px;
      font-weight: 300;
      line-height: 25.2px;
      text-align: center;
    }
  }
}
ul {
  li::marker {
    color: red;
  }
}
</style>
