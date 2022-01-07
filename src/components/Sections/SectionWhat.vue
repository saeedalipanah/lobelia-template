<template>
  <div class="page-container">
    <div class="page-title-container">
      <h1 class="page-title observe d-flex">THE ICO APP</h1>
      <p class="page-title-text observe">
        Once you’ve entered into our ecosystem, you can mange every thing.
        Anyone with a smartphone and an internet connection can partici pate in
        global marketplace.
      </p>
    </div>
    <div class="content">
      <v-container>
        <v-row>
          <v-col cols="12" md="6" class=" d-flex justify-center align-center">
            <img class="image observe" src="@/assets/logo/gfx-v.png" width="90%">
          </v-col>
          <v-col cols="12" md="6" class=" d-flex flex-column justify-center ">
            <div class="parent d-flex observe" v-for="(item, i) in items" :key="i">
              <div class="icon">
                <img :src="item.iconUrl" alt="" class="mx-5" width="80" />
              </div>
              <div class="text">
                <h1>{{ item.title }}</h1>
                <p>{{ item.text }}</p>
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
    return {
      items: [
        {
          iconUrl:
            "http://wpdemo.oceanthemes.net/icos-lobelia/wp-content/uploads/sites/25/2018/06/icon-decentralized.png",
          title: "Decentralized Platform",
          text: "Blockchain-based Lorem ipsum dolor sit amet, consectetur adipiscing elit.",
        },
        {
          iconUrl:
            "http://wpdemo.oceanthemes.net/icos-lobelia/wp-content/uploads/sites/25/2018/06/icon-crowd.png",
          title: "Crowd Wisdom",
          text: "Blockchain-based Lorem ipsum dolor sit amet, consectetur adipiscing elit.",
        },
        {
          iconUrl:
            "http://wpdemo.oceanthemes.net/icos-lobelia/wp-content/uploads/sites/25/2018/06/icon-reward.png",
          title: "Rewards MeAchanism",
          text: "Blockchain-based Lorem ipsum dolor sit amet, consectetur adipiscing elit.",
        },
      ],
    };
  },
};
</script>

<style lang="scss" scoped>
.page-container {
  background-color: #091685;
  .page-title{
    position: relative;
    &::before{
      content: 'WHAT';
    }
  }
  .content {
    .image{
      max-width: 500px;
      
    }
    .parent {
      .icon {
      }
      .text {
        h1 {
          color: #ffffff;
          font-size: 22px;
          font-weight: 600;
          line-height: 28.6px;
          margin: 0px 0px 9.6px;
          text-align: left;
        }
        p {
          color: #d2d3ff;
          font-size: 15px;
          font-weight: 300;
          line-height: 25.2px;
          text-align: left;
        }
      }
    }
  }
}
</style>
