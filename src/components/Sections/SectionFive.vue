<template>
  <div class="contanier red">
    <div class="title">
      <h1>THE MAGOR PROBLEM</h1>
      <p>
        The Cryptocurrency industry is one of the Lorem ipsum dolor sit amet,
        consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore
        et dolore magna aliqua.
      </p>
    </div>
    <div class="content">
      <v-container>
        <v-row>
          <v-col cols="12" md="6" class="cols blue darken-4">
            <div class="items-container">
                <v-img src="@/assets/logo-icon/icon-k.png"></v-img>
              <div class="caption">
                <h1 class="caption-title">Crypto Investors</h1>
                <ul>
                  <li>What is the crypto tech? Lorem ipsum dolor sit amet, consectetur.</li>
                  <li>Natural Language Understanding</li>
                  <li>How to network with other investors / like-minded people?</li>
                </ul>
              </div>
            </div>
          </v-col>
          <v-col cols="12" md="6" class="cols grey">
            <div class="items-container">
                <v-img src="@/assets/logo-icon/icon-l.png"></v-img>
              <div class="caption">
                <h1 class="caption-title">Centralize Network</h1>
                <ul>
                  <li>What is the crypto tech? Lorem ipsum dolor sit amet, consectetur.</li>
                  <li>Natural Language Understanding</li>
                  <li>How to network with other investors / like-minded people?</li>
                </ul>
              </div>
            </div>
          </v-col>
        </v-row>
        <v-row>
          <v-col cols="12" md="6" class="cols blue darken-4">
            <div class="items-container">
                <v-img src="@/assets/logo-icon/icon-m.png"></v-img>
              <div class="caption">
                <h1 class="caption-title">Crypto Developers</h1>
                <ul>
                  <li>What is the crypto tech? Lorem ipsum dolor sit amet, consectetur.</li>
                  <li>Natural Language Understanding</li>
                  <li>How to network with other investors / like-minded people?</li>
                </ul>
              </div>
            </div>
          </v-col>
          <v-col cols="12" md="6" class="cols grey">
            <div class="items-container">
                <v-img src="@/assets/logo-icon/icon-n.png"></v-img>
              <div class="caption">
                <h1 class="caption-title">General Payment</h1>
                <ul>
                  <li>What is the crypto tech? Lorem ipsum dolor sit amet, consectetur.</li>
                  <li>Natural Language Understanding</li>
                  <li>How to network with other investors / like-minded people?</li>
                </ul>
              </div>
            </div>
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
