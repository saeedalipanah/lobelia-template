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
        <section-one></section-one>
        <section-two></section-two>
        <section-three></section-three>
        <section-four></section-four>
        <section-five></section-five>
        <section-six></section-six>
        <section-seven></section-seven>
        <section-eight></section-eight>
        <section-nine></section-nine>
        <section-ten></section-ten>
        <section-eleven></section-eleven>
        <section-twelve></section-twelve>
        <section-thirteen></section-thirteen>
        <section-fourteen></section-fourteen>
        <section-fifteen></section-fifteen>
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
import SectionThirteen from './components/Sections/SectionThirteen.vue';
import SectionFourteen from './components/Sections/SectionFourteen.vue';
import SectionFifteen from './components/Sections/SectionFifteen.vue';
export default {
  name: "App",

  data: () => ({
    isLoading: true,
  }),
  mounted() {
    setTimeout(() => {
      this.isLoading = false;
    }, 1000);
  },
  methods: {
    
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
    SectionThirteen,
    SectionFourteen,
    SectionFifteen,
  },
};
</script>

<style lang="scss" >
@import url('https://fonts.googleapis.com/css2?family=Poppins:ital,wght@0,100;0,200;0,300;0,400;0,500;0,600;1,100;1,200;1,300;1,400;1,500;1,600&display=swap');
*{
  font-family: 'Poppins', sans-serif;
}
.app{
      background-image: linear-gradient(
135deg, #0a1992 0%, #000537 100%) !important;
  .loading{
    height: 100vh;
    width: 100%;
    display: flex;
    justify-content: center;
    align-items: center;
  }
}

</style>