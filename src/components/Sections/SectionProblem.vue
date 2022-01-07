<template>
  <div class="page-container">
    <div class="page-title-container">
      <h1 class="page-title observe">THE MAGOR PROBLEM</h1>
      <p class="page-title-text observe">
        The Cryptocurrency industry is one of the Lorem ipsum dolor sit amet,
        consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore
        et dolore magna aliqua.
      </p>
    </div>
    <div class="content observe">
      <v-container fluid>
        <v-row>
          <v-col cols="12" md="6" class="cols ">
            <div class="items-container observe">
              <div class="d-flex align-start mr-6">
                <v-img contain src="@/assets/logo-icon/icon-k.png" width="95" height="109"></v-img>
              </div>
              <div class="caption">
                <h1 class="caption-title">Crypto Investors</h1>
                <ul>
                  <li>
                    What is the crypto tech? Lorem ipsum dolor sit amet,
                    consectetur.
                  </li>
                  <li>Natural Language Understanding</li>
                  <li>
                    How to network with other investors / like-minded people?
                  </li>
                </ul>
              </div>
            </div>
          </v-col>
          <v-col cols="12" md="6" class="cols">
            <div class="items-container observe observe-1">
              <div class="d-flex align-start mr-6">
              <v-img contain src="@/assets/logo-icon/icon-l.png" width="95" height="109"></v-img>
              </div>
              <div class="caption">
                <h1 class="caption-title">Centralize Network</h1>
                <ul>
                  <li>
                    What is the crypto tech? Lorem ipsum dolor sit amet,
                    consectetur.
                  </li>
                  <li>Natural Language Understanding</li>
                  <li>
                    How to network with other investors / like-minded people?
                  </li>
                </ul>
              </div>
            </div>
          </v-col>
        </v-row>
        <v-row>
          <v-col cols="12" md="6" class="cols ">
            <div class="items-container observe">
              <div class="d-flex align-start mr-6">
              <v-img contain src="@/assets/logo-icon/icon-m.png" width="95" height="109"></v-img>
              </div>
              <div class="caption">
                <h1 class="caption-title">Crypto Developers</h1>
                <ul>
                  <li>
                    What is the crypto tech? Lorem ipsum dolor sit amet,
                    consectetur.
                  </li>
                  <li>Natural Language Understanding</li>
                  <li>
                    How to network with other investors / like-minded people?
                  </li>
                </ul>
              </div>
            </div>
          </v-col>
          <v-col cols="12" md="6" class="cols ">
            <div class="items-container observe observe-1">
              <div class="d-flex align-start mr-6">
              <v-img contain src="@/assets/logo-icon/icon-n.png" width="95" height="109"></v-img>
              </div>
              <div class="caption">
                <h1 class="caption-title">General Payment</h1>
                <ul>
                  <li>
                    What is the crypto tech? Lorem ipsum dolor sit amet,
                    consectetur.
                  </li>
                  <li>Natural Language Understanding</li>
                  <li>
                    How to network with other investors / like-minded people?
                  </li>
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
.page-container {
  background-color: #0a1992;
  padding-bottom: 0;
   .page-title{
    position: relative;
    &::before{
      content: 'problem';
    }
  }
  .content {
    background-color: #000537;
    border-radius: 12px;
    padding: 5% 4%;
    // margin: 0 20px;
     @media only screen and(max-width:960px) {
       margin: 0 5%;
  }
    .items-container {
      display: flex;
      margin: 10px 0;
       @media only screen and(max-width:500px) {
       flex-direction: column;
       align-items: start;
  }
      .caption {
        &-title {
          color: white;
          font-size: 22px;
          font-weight: 600;
          line-height: 28.6px;
          margin: 0px 0px 16px;
          text-align: left;
        }
        li {
          color: #d2d3ff;
          font-size: 15px;
          font-weight: 300;
          line-height: 24.3px;
          text-align: left;
          padding: 5px 0px 5px 22px;
        }
      }
    }
  }
}
ul {
  li::marker {
    color: #46bdf4;
  }
}
</style>
