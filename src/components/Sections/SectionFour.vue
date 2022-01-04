<template>
  <div class="page-container">
    44444444
   <div class="page-title-container">
     <h1 class="page-title">HOW IT WORKS</h1>
     <p class="page-title-text">ICO brings together the best of both traditional business and agile crypto models Sed ut pers piciatis unde omnis iste natus error sit voluptatem accusantium.</p>
   </div>
   <div class="content">
     <v-container>
       <v-row>
         <v-col cols="12" md="6" order="12" order-md="1" class="cols col-1 blue darken-4 ">
           <p class="content-text">At vero eos et accusamus et iusto odio dignissimos ducimus qui blan ditiis praes entium volup tatum deleniti atque corrupti quos dolores et quas mole stias excepturi sint occa ecati cupid itate non provident, similique sunt in culpa qui officia dese runt mollitia animi, id est laborum et dolorum fuga. Et harum quidem rerum facilis est et expedita distinctio.</p>
           <ol>
             <li class="content-text-items">The Platform will earn premium libero tempore, cum soluta nobis est eligendi optio.</li>
             <li class="content-text-items">The ICO Marketplace rerum hic tenetur a sapiente delectus, ut aut reiciendis voluptatibus maiores alias conse quatur aut perferendis.</li>
             <li class="content-text-items">Contributor payouts perfectly simple and easy awaywe denounce with righteous indigo</li>
             <li class="content-text-items">Owners of cryptocurrency keep their digital coins in ICO digital wallet. A coin-holder’s identification is stored in an encrypted address that they have control over – it is not attached to a person’s identity.</li>
           </ol>
         </v-col>
         <v-col cols="12" md="6" order="1" order-md="12" class="cols grey d-flex align-center justify-center">
           <v-img contain class="recycle-image" src="@/assets/logo/gfx-w-dark.png" max-width="500"></v-img>
         </v-col>
       </v-row>
     </v-container>
   </div>
  </div>
</template>

<script>
export default {};
</script>

<style lang="scss" scoped>
.page-container{
  
  .content{
    .col-1{
      @media only screen and(max-width :960px){
        padding: 0 10%;
      }
      @media only screen and(max-width :560px){
        padding: 0 4%;
      }
    }
    .content-text{
      font-size: 15px;
      font-weight: 300;
      line-height: 25.2px;
      color: #d2d3ff;
    }
    .content-text-items{
      font-size: 15px;
      font-weight: 300;
      line-height: 28px;
      color: #d2d3ff;
    }
    .recycle-image{
    }
  }
}
ol li{
  margin: 15px;
&::marker {
    font-size: 35px;
    font-weight: 900;
    color: #2b56f5;
    font-family: 'Poppins', sans-serif !important;
}
}

</style>
