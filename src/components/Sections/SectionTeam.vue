<template>
  <div class="page-container">
    <div class="page-title-container">
      <h1 class="page-title page-title-team observe">HOW IT WORKS</h1>
      <p class="page-title-text observe">
        ICO brings together the best of both traditional business and agile
        crypto models Sed ut pers piciatis unde omnis iste natus error sit
        voluptatem accusantium.
      </p>
    </div>
    
    <v-container fluid>
      <v-row >
        <v-col class=" d-flex justify-center" cols="12" sm="6" md="3" v-for="(user,i) in users" :key="i">
          <v-card class="observe cards d-flex flex-column align-center " :class="`observe-${i}`" max-width="344" >
            <v-avatar size="150">
            <v-img contain
              :src="user.avatarImage"
              height="200px" class="red"
            ></v-img>

            </v-avatar>
            <v-card-title class="username text-center white--text"> {{user.name}} </v-card-title>
            <v-card-subtitle class="stack"> {{user.stack}} </v-card-subtitle>

            <v-card-text class="description text-center">{{user.description}}</v-card-text>

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
    <div class="page-title-container ">
      <h1 class="page-title pb-0 mb-0 observe">ADVISORS</h1>
    </div>
    <v-container fluid>
      <v-row justify="center">
        <v-col class=" d-flex justify-center" cols="12" sm="6" md="3" v-for="(advisor,i) in advisors" :key="i">
          <v-card class="observe cards d-flex flex-column align-center " max-width="344" :class="`observe-${i}`">
            <v-avatar size="150">
            <v-img contain
              :src="advisor.avatarImage"
              height="200px" class=""
            ></v-img>

            </v-avatar>
            <v-card-title class="username text-center white--text"> {{advisor.name}} </v-card-title>
            <v-card-subtitle class="stack"> {{advisor.stack}} </v-card-subtitle>

            <v-card-text class="description text-center">{{advisor.description}}</v-card-text>

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
  
  
};
</script>

<style lang="scss" scoped>
.page-container{
  background-color: #0a1992;
  padding-bottom: 0;
    .page-title-team{
    position: relative;
    &::before{
      content: 'team';
    }
  }
  .cards{
    
    background: #08157a;
    padding: 20px 0;
    .stack{
      color: #46bdf4 ;
    }
    .description{
      color: #d2d3ff;
    }
    .fab{
      color: #d2d3ff;
      margin: 0 3px;
    }
    
  }
  
}
</style>
