<template>
  <div class="contanier">
   <div class="title">
     <h1>THE ICO APP</h1>
     <p>Once you’ve entered into our ecosystem, you can mange every thing. Anyone with a smartphone and an internet connection can partici pate in global marketplace.</p>
   </div>
   <div class="content">
     <v-container>
       <v-row>
         <v-col cols="12" md="6" class="cols blue lighten-2">
           <v-img src="@/assets/logo/gfx-v.png"></v-img>
         </v-col>
         <v-col cols="12" md="6" class="cols grey"></v-col>
         
       </v-row>
     </v-container>
   </div>
  </div>
</template>

<script>
export default {};
</script>

<style lang="scss" scoped>
.contanier{
  .title{
    display: flex;
    flex-direction: column;
    align-items: center;
    text-align: center;
  }
  .content{
    .cols{
    }
  }
}
</style>
