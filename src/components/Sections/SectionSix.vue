<template>
  <div class="contanier blue lighten-2">
    <div class="title">
      <h1>THE CRYPTO SOLUTION</h1>
      <p>
        The Cryptocurrency industry is one of the Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.
      </p>
    </div>
    <div class="content">
      <v-container>
        <v-row>
          <v-col cols="12" sm="6" md="3" class="cols yellow darken-4" v-for="(item,i) in items" :key="i">
            <div class="content red d-flex flex-column align-center">
              <h5>{{item.iconUrl}}</h5>
              <h3>{{item.title}}</h3>
              <p class="text-center">{{item.textContent}}</p>
            </div>
          </v-col>
        </v-row>
      </v-container>
    </div>
  </div>
</template>

<script>
export default {
  data(){
    return{
      items:[
        {
          iconUrl:'this is a icon',
          title:'Relational Blockchain',
          textContent:'Contributors and members est et expedita distinctio. Nam libero tempore'
        },
        {
          iconUrl:'this is a icon',
          title:'Fraud Reduction',
          textContent:'Contributors and members est et expedita distinctio. Nam libero tempore'
        },
        {
          iconUrl:'this is a icon',
          title:'Next Generation Wallet',
          textContent:'Contributors and members est et expedita distinctio. Nam libero tempore'
        },
        {
          iconUrl:'this is a icon',
          title:'Recovery Nodes',
          textContent:'Contributors and members est et expedita distinctio. Nam libero tempore'
        },
        {
          iconUrl:'this is a icon',
          title:'Relational Blockchain',
          textContent:'Contributors and members est et expedita distinctio. Nam libero tempore'
        },
        {
          iconUrl:'this is a icon',
          title:'Fraud Reduction',
          textContent:'Contributors and members est et expedita distinctio. Nam libero tempore'
        },
        {
          iconUrl:'this is a icon',
          title:'Next Generation Wallet',
          textContent:'Contributors and members est et expedita distinctio. Nam libero tempore'
        },
        {
          iconUrl:'this is a icon',
          title:'Recovery Nodes',
          textContent:'Contributors and members est et expedita distinctio. Nam libero tempore'
        },
      ]
    }
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
  .content {
    .items-container{
      display: flex;
      
      .caption{
        &-title{
          background: red;
        }
      }
    }
  }
}
ul{
  li::marker{
    color: red;
  }
}
</style>
