<template>
  <v-app class="app">
    <div v-if="isLoading" class="loading">
      <loading-spinner></loading-spinner>
    </div>

    <div v-else>
      <header>
        <Navbar class="navigation"></Navbar>
      </header>
      <v-main>
        <section-one id="sec-1"> </section-one>
        <section-two id="sec-2"></section-two>
        <section-three id="sec-3"></section-three>
        <section-four id="sec-4"></section-four>
        <section-five id="sec-5"></section-five>
        <section-six id="sec-6"></section-six>
        <section-seven id="sec-7"></section-seven>
        <section-eight id="sec-8"></section-eight>
        <section-nine id="sec-9"></section-nine>
        <section-ten id="sec-10"></section-ten>
        <section-eleven id="sec-11"></section-eleven>
        <section-twelve id="sec-12"></section-twelve>
        <section-twelve-sub-logo id="sec-13"></section-twelve-sub-logo>
        <section-thirteen id="sec-14"></section-thirteen>
        <section-fourteen id="sec-15"></section-fourteen>
        <section-fifteen id="sec-16"></section-fifteen>
      </v-main>

      <footer></footer>
    </div>
  </v-app>
</template>

<script>
import Navbar from "@/components/UI/Navbar.vue";
import LoadingSpinner from "@/components/UI/LoadingSpinner.vue";
import SectionOne from "@/components/Sections/SectionOne.vue";
import SectionTwo from "@/components/Sections/SectionTwo.vue";
import SectionThree from "@/components/Sections/SectionThree.vue";
import SectionFour from "@/components/Sections/SectionFour.vue";
import SectionFive from "@/components/Sections/SectionFive.vue";
import SectionSix from "@/components/Sections/SectionSix.vue";
import SectionSeven from "@/components/Sections/SectionSeven.vue";
import SectionEight from "@/components/Sections/SectionEight.vue";
import SectionNine from "@/components/Sections/SectionNine.vue";
import SectionTen from "@/components/Sections/SectionTen.vue";
import SectionEleven from "@/components/Sections/SectionEleven.vue";
import SectionTwelve from "@/components/Sections/SectionTwelve.vue";
import SectionTwelveSubLogo from "./components/Sections/SectionTwelveSubLogo.vue";
import SectionThirteen from "./components/Sections/SectionThirteen.vue";
import SectionFourteen from "./components/Sections/SectionFourteen.vue";
import SectionFifteen from "./components/Sections/SectionFifteen.vue";
export default {
  name: "App",

  data: () => ({
    isLoading: true,
  }),
  mounted() {
    this.load().then(() => {
      this.slideInAnimation();
    });
  },
  methods: {
    slideInAnimation() {
      const cards = document.getElementsByClassName("observe");
      this.observer = new IntersectionObserver((enteries) => {
        enteries.forEach((entery) => {
          if (entery.isIntersecting) {
            entery.target.classList.add("show");
          }
        });
      });
      for (let i = 0; i < cards.length; i++) {
        console.log(cards[i]);
        this.observer.observe(cards[i]);
      }
    },
    load() {
      return new Promise((resolve) => {
        setTimeout(() => {
          this.isLoading = false;
          resolve();
        }, 1000);
      });
    },
  },
  components: {
    Navbar,
    LoadingSpinner,
    SectionOne,
    SectionTwo,
    SectionThree,
    SectionFour,
    SectionFive,
    SectionSix,
    SectionSeven,
    SectionEight,
    SectionNine,
    SectionTen,
    SectionEleven,
    SectionTwelve,
    SectionTwelveSubLogo,
    SectionThirteen,
    SectionFourteen,
    SectionFifteen,
  },
};
</script>

<style lang="scss">
@import url("https://fonts.googleapis.com/css2?family=Poppins:ital,wght@0,100;0,200;0,300;0,400;0,500;0,600;1,100;1,200;1,300;1,400;1,500;1,600&display=swap");
* {
  font-family: "Poppins", sans-serif;
}
.app {
  background-image: linear-gradient(
    135deg,
    #0a1992 0%,
    #000537 100%
  ) !important;
  .loading {
    height: 100vh;
    width: 100%;
    display: flex;
    justify-content: center;
    align-items: center;
  }
  .observe {
    transform: translateY(80px);
    opacity: 0;
    &.show {
      transition: all 1s ease;
      transform: translateY(0);
      opacity: 1;
    }
    
    &.observe-1 {
      transition-delay: .2s;
    }
    &.observe-2 {
      transition-delay: .4s;
    }
    &.observe-3 {
      transition-delay: .6s;
    }
    &.observe-4 {
      transition-delay: .2s;
    }
    &.observe-5 {
      transition-delay: .4s;
    }
    &.observe-6 {
      transition-delay: .6s;
    }
    &.observe-7 {
      transition-delay: .8s;
    }
  }
}
</style>
