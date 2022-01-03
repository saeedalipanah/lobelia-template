<template>
  <div class="contanier ">
    <div class="title">
      <h1>HOW IT WORKS</h1>
      <p>
        ICO brings together the best of both traditional business and agile
        crypto models Sed ut pers piciatis unde omnis iste natus error sit
        voluptatem accusantium.
      </p>
    </div>
    
    <v-container fluid>
      <v-row >
        <v-col class="grey d-flex justify-center" cols="12" sm="6" md="3" v-for="(user,i) in users" :key="i">
          <v-card class="cards d-flex flex-column align-center " :class="`card-${i}`" max-width="344" >
            <v-avatar size="150">
            <v-img contain
              :src="user.avatarImage"
              height="200px" class="red"
            ></v-img>

            </v-avatar>
            <v-card-title class="text-center"> {{user.name}} </v-card-title>
            <v-card-subtitle> {{user.stack}} </v-card-subtitle>

            <v-card-text class="text-center">{{user.description}}</v-card-text>

            <v-card-actions>
             <i class="fab fa-linkedin"></i>
             <i class="fab fa-facebook"></i>
             <i class="fab fa-twitter"></i>
            </v-card-actions>
          </v-card>
        </v-col>
      </v-row>
    </v-container>
    <div class="title">
      <!-- ADVISORS -->
      <h1>ADVISORS</h1>
    </div>
    <v-container fluid>
      <v-row justify="center">
        <v-col class="grey d-flex justify-center" cols="12" sm="6" md="3" v-for="(advisor,i) in advisors" :key="i">
          <v-card class="cards d-flex flex-column align-center " max-width="344" :class="`card-${i}`">
            <v-avatar size="150">
            <v-img contain
              :src="advisor.avatarImage"
              height="200px" class="red"
            ></v-img>

            </v-avatar>
            <v-card-title class="text-center"> {{advisor.name}} </v-card-title>
            <v-card-subtitle> {{advisor.stack}} </v-card-subtitle>

            <v-card-text class="text-center">{{advisor.description}}</v-card-text>

            <v-card-actions>
             <i class="fab fa-linkedin"></i>
             <i class="fab fa-facebook"></i>
             <i class="fab fa-twitter"></i>
            </v-card-actions>
          </v-card>
        </v-col>
      </v-row>
    </v-container>
    <!-- ADVISORS -->
  </div>
</template>

<script>
export default {
  data() {
    return {
      users: [
        {
          avatarImage: "https://demo.themenio.com/ico/images/team/sq-a.jpg",
          name: "Waylon Dalton",
          stack: "CEO & Lead Blockchain",
          description: "Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incide.",
        },
        {
          avatarImage: "https://demo.themenio.com/ico/images/team/sq-b.jpg",
          name: "Stefan Harary",
          stack: "CEO & Lead Blockchain",
          description: "Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incide.",
        },
        {
          avatarImage: "https://demo.themenio.com/ico/images/team/sq-c.jpg",
          name: "Moises Teare",
          stack: "CEO & Lead Blockchain",
          description: "Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incide.",
        },
        {
          avatarImage: "https://demo.themenio.com/ico/images/team/sq-d.jpg",
          name: "Gabriel Bernal",
          stack: "CEO & Lead Blockchain",
          description: "Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incide.",
        },
      ],
      advisors:[
        {
          avatarImage: "https://demo.themenio.com/ico/images/team/sq-a.jpg",
          name: "Waylon Dalton",
          stack: "CEO & Lead Blockchain",
          description: "Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incide.",
        },
        {
          avatarImage: "https://demo.themenio.com/ico/images/team/sq-d.jpg",
          name: "Gabriel Bernal",
          stack: "CEO & Lead Blockchain",
          description: "Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incide.",
        },
        {
          avatarImage: "https://demo.themenio.com/ico/images/team/sq-b.jpg",
          name: "Stefan Harary",
          stack: "CEO & Lead Blockchain",
          description: "Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incide.",
        },
      ],
      observer: null
    };
  },
  mounted(){
    this.slideInAnimation()
  },
  methods:{
    slideInAnimation(){
      const cards = document.getElementsByClassName('cards');
      this.observer = new IntersectionObserver((enteries)=>{
        enteries.forEach(entery => {
          if(entery.isIntersecting){
            entery.target.classList.add('show')
          }
        })
      });
      for (let i = 0; i < cards.length; i++) {
        this.observer.observe(cards[i])
      }
    },

  }
  
};
</script>

<style lang="scss" scoped>
.contanier {
  .title {
    display: flex;
    flex-direction: column;
    align-items: center;
    text-align: center;
  }
  .cards{
    transform: translateY(80px);
    opacity: 0;
    &.show{
      transition: all 1s ease;
      transform: translateY(0);
      opacity: 1;
    }
    &.card-1 {
      transition-delay: .1s;
    }
    &.card-2 {
      transition-delay: .2s;
    }
    &.card-3 {
      transition-delay: .3s;
    }
    
  }
  
}
</style>
