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
  }
};
</script>
