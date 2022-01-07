<template>
  <div class="page-container">
    <div class="observe-object"></div>
    <vue-particles
      style="position: absolute; width: 100%; margin-top: -90px; height: 100vh"
      color="#0175fa"
      :particleOpacity="0.4"
      :particlesNumber="40"
      shapeType="circle"
      :particleSize="7"
      linesColor="#0175fa"
      :linesWidth="2"
      :lineLinked="true"
      :lineOpacity="0.1"
      :linesDistance="150"
      :moveSpeed="5"
      :hoverEffect="false"
      hoverMode="grab"
      :clickEffect="false"
      clickMode="push"
    >
    </vue-particles>
    <v-img
      contain
      src="@/assets/logo/gfx-c.png"
      class="blockchain-img"
      width="80%"
      min-width="290"
      max-width="920"
    ></v-img>
    <div class="content">
      <h1 class="content-title">Powering Data for the new equity blockchain</h1>
      <p class="content-text my-5">
        Global decentralize network to buy & sell shares. Solving the
        Cryptocurrency Trust problems.
      </p>
      <div class="buttons">
        <v-btn rounded class="button button-signup observe observe-7"
          >sign up to join</v-btn
        >
        <v-btn
          rounded
          class="button button-token-distribution observe observe-7"
          >token distribution</v-btn
        >
      </div>
    </div>
  </div>
</template>

<script>
export default {
  mounted() {
    const blockchainImage = document.querySelector(".blockchain-img");
    const content = document.querySelector(".content");
    blockchainImage.classList.add("slide-up");
    content.classList.add("slide-up");
  },
};
</script>

<style lang="scss" scoped>
.page-container {
  background: url("http://wpdemo.oceanthemes.net/icos-lobelia/wp-content/themes/icos-lobelia/assets/images/header-shape-lobelia.png")
      no-repeat,
    linear-gradient(to top left, #000537 0%, #0a1992 100%);
  background-size: contain;
  background-position: top left;
  padding-top: 90px;
  position: relative;
  &::before {
    position: absolute;
    left: 0;
    bottom: 0;
    height: 70%;
    width: 100%;
    content: "";
    background: linear-gradient(to top, #0a1992 0%, rgba(0, 0, 0, 0) 100%);
  }
  .observe-object {
    position: absolute !important;
    top: 1px;
    height: 1px;
    width: 1px;
  }
  .blockchain-img {
    margin: 20px 0;
    min-height: 390px;
    @media only screen and(max-width:800px) {
      min-height: 160px;
    }
  }
  .slide-up {
    animation: moveDown 1s ease;
  }

  .content {
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: center;
    width: 90%;
    max-width: 600px;
    z-index: 2;
    .content-title {
      color: #ffffff;
      font-size: 35.2px;
      font-weight: 600;
      line-height: 52.8px;
      text-align: center;
      @media only screen and(max-width : 560px) {
        font-size: 24.5px;
      }
    }
    .content-text {
      color: #8ca2e5;
      font-size: 17.6px;
      font-weight: 300;
      line-height: 29.92px;
      text-align: center;
      @media only screen and(max-width : 560px) {
        font-size: 15.5px;
      }
    }
    .buttons {
      display: flex;
      @media only screen and(max-width : 430px) {
        flex-direction: column;
        align-items: center;
        justify-content: center;
      }
      .button {
        border-radius: 44px !important;
        color: #ffffff;
        font-size: 12px;
        font-weight: 500;
        justify-content: center;
        letter-spacing: 1.2px;
        line-height: 24px;
        padding: 23px 30px !important;
        text-align: center;
        margin: 5px 15px !important;
        @media only screen and(max-width : 560px) {
          padding: 20px 17px !important;
          margin: 0 8px;
        }
      }
      .button-signup {
        background: linear-gradient(to right, #2b56f5 0%, #46bdf4 100%);
        &:hover {
          background: linear-gradient(to right, #46bdf4 0%, #2b56f5 100%);
        }
      }
      .button-token-distribution {
        background: linear-gradient(to right, #7a0fff 0%, #2b56f5 100%);
        &:hover {
          background: linear-gradient(to right, #2b56f5 0%, #7a0fff 100%);
        }
      }
    }
  }
}
@keyframes moveDown {
  0% {
    transform: translateY(200px);
    opacity: 0;
  }
  100% {
    transform: translateY(0);
    opacity: 1;
  }
}
</style>
