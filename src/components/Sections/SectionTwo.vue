<template>
  <div class="page-container">
    
    <v-row class="px-10">
      <v-col class="px-5 d-flex align-center justify-center" cols="12" md="6">
        <div class="video observe">
          <play-icon class="far"></play-icon>
          <img
            src="@/assets/cover/video-cover.jpg"
            alt=""
            width="100%"
            height="100%"
          />
        </div>
      </v-col>
      <v-col class="px-5 d-flex flex-column justify-center" cols="12" md="6">
        <div class="text-content observe observe-1">
          <h1>We’ve built a platform to buy and sell shares.</h1>
          <p>
            We’re reinventing the global equity blockchian – that is secure,
            smart and easy-to-use platform, and completely disrupting the way
            businesses raise capital and the way investors buy and sell shares.
          </p>
        </div>
      </v-col>
    </v-row>
  </div>
</template>

<script>
import PlayIcon from '@/components/UI/PlayIcon.vue'
export default {
  components:{
    PlayIcon
  }
};
</script>

<style lang="scss" scoped>
.page-container {
  padding-bottom: 0 ;
  background-color: #0a1992;
    .video {
      position: relative;
      border-radius: 5px;
      &::before {
        content: "";
        position: absolute;
        top: 0;
        left: 0;
        height: 100%;
        width: 100%;
        background: rgba(0, 0, 0, 0.329);
        border-radius: 5px;
      }
      img {
        border-radius: 5px;
      }
      .far {
        position: absolute;
        font-size: 60px;
        color: #3682f5;
        font-weight: 100;
        border-radius: 50%;
        left: 50%;
        top: 50%;
        transform: translate(-50%, -50%);
      }
    }
    .text-content {
      h1 {
        color: #ffffff;
        font-size: 36px;
        font-weight: 600;
        line-height: 46.8px;
        margin: 0px 0px 20px;
        text-align: left;
      }
      p {
        color: #d2d3ff;
        font-size: 19.2px;
        font-weight: 300;
        line-height: 32.256px;
        text-align: left;
      }
    }
  }
</style>
