<template>
  <div class="contanier">
   <div class="title">
     <h1>HOW IT WORKS</h1>
     <p>ICO brings together the best of both traditional business and agile crypto models Sed ut pers piciatis unde omnis iste natus error sit voluptatem accusantium.</p>
   </div>
   <div class="content">
     <v-container>
       <v-row>
         <v-col cols="12" md="6" class="cols blue darken-4">
           <p>At vero eos et accusamus et iusto odio dignissimos ducimus qui blan ditiis praes entium volup tatum deleniti atque corrupti quos dolores et quas mole stias excepturi sint occa ecati cupid itate non provident, similique sunt in culpa qui officia dese runt mollitia animi, id est laborum et dolorum fuga. Et harum quidem rerum facilis est et expedita distinctio.</p>
           <ol>
             <li>The Platform will earn premium libero tempore, cum soluta nobis est eligendi optio.</li>
             <li>The ICO Marketplace rerum hic tenetur a sapiente delectus, ut aut reiciendis voluptatibus maiores alias conse quatur aut perferendis.</li>
             <li>Contributor payouts perfectly simple and easy awaywe denounce with righteous indigo</li>
             <li>Owners of cryptocurrency keep their digital coins in ICO digital wallet. A coin-holder’s identification is stored in an encrypted address that they have control over – it is not attached to a person’s identity.</li>
           </ol>
         </v-col>
         <v-col cols="12" md="6" class="cols grey">
           <v-img src="@/assets/logo/gfx-w-dark.png"></v-img>
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
ol li::marker {
    color: red;
}
</style>
