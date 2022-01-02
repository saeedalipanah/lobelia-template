<template>
  <v-app class="">
    <header>
      <Navbar></Navbar>
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
    </v-main>

    <footer></footer>
  </v-app>
</template>

<script>
import Navbar from '@/components/UI/Navbar.vue'
import SectionOne from '@/components/Sections/SectionOne.vue'
import SectionTwo from '@/components/Sections/SectionTwo.vue'
import SectionThree from '@/components/Sections/SectionThree.vue'
import SectionFour from '@/components/Sections/SectionFour.vue'
import SectionFive from '@/components/Sections/SectionFive.vue'
import SectionSix from '@/components/Sections/SectionSix.vue'
import SectionSeven from '@/components/Sections/SectionSeven.vue'
import SectionEight from '@/components/Sections/SectionEight.vue'
import SectionNine from '@/components/Sections/SectionNine.vue'
import SectionTen from '@/components/Sections/SectionTen.vue'
import SectionEleven from '@/components/Sections/SectionEleven.vue'
export default {
  name: "App",

  data: () => ({
    //
  }),

  components:{
    Navbar,
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
  }
};
</script>
