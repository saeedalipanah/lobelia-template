<template>
  <div class="container">
    <div class="title">
      <h1>CONTACT ICO CRYPTO</h1>
      <p>Any question? Reach out to us and we’ll get back to you shortly.</p>
    </div>
    <div class="content">
      <v-container>
        <v-row justify="center">
          <v-col cols="12" sm="4" v-for="(item,i) in items" :key="i">
            <div class=" red d-flex justify-center align-center">
              <span class="fas fa-phone"></span>
              <h4 class="mx-4">{{item.text}}</h4>
            </div>
          </v-col>
        </v-row>
      </v-container>
      <v-container>
        <v-row class="">
          <v-col cols="12" class=" red">
              <v-text-field class="input-text"
            label="Your Name"
          ></v-text-field>
          </v-col>
          <v-col cols="12">
              <v-text-field
              class="input-text"
            label="Your Email"
          ></v-text-field>
          </v-col>
          <v-col cols="12">
              <v-text-field class="input-text"
            label="Your Message"
          ></v-text-field>
          </v-col>
        </v-row>
      </v-container>
      <div class="d-flex justify-center">
      <v-btn rounded>submit</v-btn>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      items: [
        {
          icon: "",
          text: "+44 0123 4567",
        },
        {
          icon: "",
          text: "info@company.com",
        },
        {
          icon: "",
          text: "Join us on Telegram",
        },
      ],
    };
  },
};
</script>

<style lang="scss" scoped>
.container {
  .title {
    display: flex;
    flex-direction: column;
    align-items: center;
    text-align: center;
  }
  .content {
   .input-text {
     width: 60%;
     margin: 0 auto;
     ::v-deep .v-label{
       left: 45% !important;
     }
  }
}
}
span{
  font-size: 30px;
  position: relative;
  background: rgb(255, 253, 253);
  padding: 10px;
  border-radius: 50%;
  
}
</style>
