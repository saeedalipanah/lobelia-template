<template>
  <div class="page-container">
    <div class="page-title-container">
      <h1 class="page-title observe">CONTACT ICO CRYPTO</h1>
      <p class="page-title-text observe">
        Any question? Reach out to us and we’ll get back to you shortly.
      </p>
    </div>
    <div class="content">
      <v-container>
        <v-row>
          <v-col cols="12" sm="4" v-for="(item, i) in items" :key="i">
            <div
              class="content-us d-flex justify-center align-center observe"
              :class="`observe-${i}`"
            >
              <span class="content-us-icon" :class="`${item.icon}`"></span>
              <h4 class="mx-4 content-us-text">{{ item.text }}</h4>
            </div>
          </v-col>
        </v-row>
      </v-container>
      <v-container>
        <v-row class="">
          <v-col cols="12">
            <v-text-field
              class="input-text name mt-14"
              label="Your Name"
            ></v-text-field>
          </v-col>
          <v-col cols="12">
            <v-text-field
              class="input-text email"
              label="Your Email"
            ></v-text-field>
          </v-col>
          <v-col cols="12">
            <v-text-field
              class="input-text message pt-10 pb-2"
              label="Your Message"
            ></v-text-field>
          </v-col>
        </v-row>
      </v-container>
      <div class="d-flex justify-center">
        <v-btn rounded class="submit observe observe-3">submit</v-btn>
      </div>
    </div>
    <base-line class="line"></base-line>
  </div>
</template>

<script>
import BaseLine from "@/components/UI/BaseLine.vue";
export default {
  data() {
    return {
      items: [
        {
          icon: "fas fa-phone",
          text: "+44 0123 4567",
        },
        {
          icon: "fas fa-envelope",
          text: "info@company.com",
        },
        {
          icon: "fab fa-telegram-plane",
          text: "Join us on Telegram",
        },
      ],
    };
  },
  components: {
    BaseLine,
  },
};
</script>

<style lang="scss" scoped>
.page-container {
  background-color: #0a1992;
  position: relative;
  .page-title {
    position: relative;
    &::before {
      content: "contact";
    }
  }
  .content {
    max-width: 800px;
    .content-us {
      .content-us-icon {
        color: #0a1992;
        font-size: 18px;
        &.fa-telegram-plane {
          padding: 10px 12px;
        }
      }
      .content-us-text {
        color: #f5f7fe;
        display: inline;
        font-size: 15.04px;
        font-weight: 300;
        line-height: 25.2672px;
        text-align: center;
        white-space: nowrap;
      }
    }

    .input-text {
      width: 100%;
      max-width: 800px;
      margin: 0 auto;
      font-size: 50px;
      &:hover {
        color: transparent;
        border-color: transparent !important;
      }

      ::v-deep .v-input__slot:before {
        border-color: rgba(145, 145, 145, 0.719);
        width: 100%;
        ::v-deep .v-label--acitve {
          top: -30px;
        }
      }
      ::v-deep .v-label {
        // left: 45% !important;
        width: 100%;
        max-width: unset !important;
        transform-origin: center !important;
        text-align: center;
        font-size: 1rem;
        font-weight: 400;
        color: rgb(255, 255, 255);
      }
      ::v-deep .primary--text {
        color: rgb(255, 255, 255) !important;
        border-color: white;
      }
    }
    .submit {
      background-image: linear-gradient(to right, #2b56f5 0%, #46bdf4 100%);
      padding: 27px 65px;
      font-size: 14px;
      font-weight: 700;
      line-height: 24px;
      color: white;
    }
  }
  .line {
    bottom: -120px;
    @media only screen and(max-width: 960px) {
      bottom: -90px;
    }
    @media only screen and(max-width: 768px) {
      bottom: -60px;
    }
  }
}
span {
  font-size: 30px;
  position: relative;
  background: rgb(255, 253, 253);
  padding: 10px;
  border-radius: 50%;
}
</style>
