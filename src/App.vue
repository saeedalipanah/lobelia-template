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
        <section-what id="sec-3"></section-what>
        <section-process id="sec-4"></section-process>
        <section-problem id="sec-5"></section-problem>
        <section-solution id="sec-6"></section-solution>
        <section-apps id="sec-7"></section-apps>
        <section-token id="sec-8"></section-token>
        <section-nine id="sec-9"></section-nine>
        <section-roadmap id="sec-10"></section-roadmap>
        <section-team id="sec-11"></section-team>
        <section-partners id="sec-12"></section-partners>
        <section-twelve-sub-logo id="sec-13"></section-twelve-sub-logo>
        <section-faqs id="sec-14"></section-faqs>
        <section-contact id="sec-15"></section-contact>
        <section-fifteen id="sec-16"></section-fifteen>
        <div  class="cover-top" id="cover-top"></div>
        <div  class="cover-bottom" id="cover-bottom"></div>
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
import SectionWhat from "@/components/Sections/SectionWhat.vue";
import SectionProcess from "@/components/Sections/SectionProcess.vue";
import SectionProblem from "@/components/Sections/SectionProblem.vue";
import SectionSolution from "@/components/Sections/SectionSolution.vue";
import SectionApps from "@/components/Sections/SectionApps.vue";
import SectionToken from "@/components/Sections/SectionToken.vue";
import SectionNine from "@/components/Sections/SectionNine.vue";
import SectionRoadmap from "@/components/Sections/SectionRoadmap.vue";
import SectionTeam from "@/components/Sections/SectionTeam.vue";
import SectionPartners from "@/components/Sections/SectionPartners.vue";
import SectionTwelveSubLogo from "./components/Sections/SectionTwelveSubLogo.vue";
import SectionFaqs from "./components/Sections/SectionFaqs.vue";
import SectionContact from "./components/Sections/SectionContact.vue";
import SectionFifteen from "./components/Sections/SectionFifteen.vue";
export default {
  name: "App",

  data: () => ({
    isLoading: true,
    // coverIsShow:true,
  }),
  mounted() {
    this.load().then(() => {
      this.slideInAnimation();
      const coverTop = document.getElementById('cover-top');
      const coverBottom = document.getElementById('cover-bottom');
      const body = document.querySelector('body');
      console.log(body);
      coverTop.classList.add('move-up');
      coverBottom.classList.add('move-down');
        body.style.height = "100vh"
        body.style.overflow = 'hidden'
      setTimeout(() => {
        body.style.height = "auto"
        body.style.overflow = 'auto'
        
      }, 900);
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
        this.observer.observe(cards[i]);
      }
    },
    load() {
      return new Promise((resolve) => {
        setTimeout(() => {
          this.isLoading = false;
          resolve();
        }, 3000);
      });
    },
  },
  components: {
    Navbar,
    LoadingSpinner,
    SectionOne,
    SectionTwo,
    SectionWhat,
    SectionProcess,
    SectionProblem,
    SectionSolution,
    SectionApps,
    SectionToken,
    SectionNine,
    SectionRoadmap,
    SectionTeam,
    SectionPartners,
    SectionTwelveSubLogo,
    SectionFaqs,
    SectionContact,
    SectionFifteen,
  },
};
</script>

<style lang="scss">

.app {
 overflow: hidden;
 position: relative;
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
  .cover-top{
    width: 100%;
    height: 50vh;
    background-color: rgb(255, 255, 255);
    position: absolute;
    top: -90px;
    z-index: 100;
  }
  .move-up{
    animation: moveUp .6s ease-in forwards ;
  }
  .move-down{
    animation: moveDown .6s ease-in  forwards ;
  }
  .cover-bottom{
    width: 100%;
    height: 60vh;
    background-color: rgb(253, 255, 253);
    position: absolute;
    top: 39vh;
    z-index: 100;
  }
}
@keyframes moveUp {
  0%{
    transform: translate(0,0);
  }
  99%{
    transform: translate(0,-600px);
  }
  100%{
    transform: translate(10000px,0);
  }
}
@keyframes moveDown {
  0%{
    transform: translate(0,0);
  }
  99%{
    transform: translate(0,600px);
  }
  100%{
    transform: translate(10000px,0);
  }
}
</style>
