<template>
  <div class="page-container">
    <div class="page-title-container">
      <h1 class="page-title observe">FREQUENTLY ASKED QUESTION</h1>
      <p class="page-title-text observe">
        Below we’ve provided a bit of ICO, ICO Token, cryptocurrencies, and few
        others. If you have any other questions, please get in touch using the
        contact form below.
      </p>
    </div>
    <div class="content observe">
      <v-container fluid>
        <v-row justify="center">
          <v-col class="">
            <v-tabs
              class="tabs"
              v-model="tab"
              background-color="transparent"
              color=""
              grow
            >
              <v-tab v-for="(tab, i) in tabs" :key="i" class="tab">
                {{ tab.name }}
                <div class="line"></div>
              </v-tab>
            </v-tabs>
            <v-tabs-items v-model="tab">
              <v-tab-item v-for="(tab, i) in tabs" :key="i">
                <v-expansion-panels accordion class="panels my-5">
                  <v-expansion-panel
                    class="panel"
                    v-for="(quastion, i) in tabs[i].quastions"
                    :key="i"
                  >
                    <v-expansion-panel-header class="header">{{
                      quastion.title
                    }}</v-expansion-panel-header>
                    <v-expansion-panel-content class="text">
                      {{ quastion.content }}
                    </v-expansion-panel-content>
                  </v-expansion-panel>
                </v-expansion-panels>
              </v-tab-item>
            </v-tabs-items>
          </v-col>
        </v-row>
      </v-container>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      tab: null,
      tabs: [
        {
          name: "General",
          quastions: [
            {
              title: "What is ICO Crypto?",
              content:
                "Once ICO period is launched, You can purchased Token with Etherum, Bitcoin or Litecoin. You can also tempor incididunt ut labore et dolore magna aliqua sed do eiusmod eaque ipsa.",
            },
            {
              title: "What cryptocurrencies can I use to purchase?",
              content:
                "Once ICO period is launched, You can purchased Token with Etherum, Bitcoin or Litecoin. You can also tempor incididunt ut labore et dolore magna aliqua sed do eiusmod eaque ipsa.",
            },
            {
              title: "How can I participate in the ICO Token sale?",
              content:
                "Once ICO period is launched, You can purchased Token with Etherum, Bitcoin or Litecoin. You can also tempor incididunt ut labore et dolore magna aliqua sed do eiusmod eaque ipsa.",
            },
            {
              title: "How do I benefit from the ICO Token?",
              content:
                "Once ICO period is launched, You can purchased Token with Etherum, Bitcoin or Litecoin. You can also tempor incididunt ut labore et dolore magna aliqua sed do eiusmod eaque ipsa.",
            },
          ],
        },
        {
          name: "Pre-ICO & ICO",
          quastions: [
            {
              title: "Which of us ever undertakes laborious?",
              content:
                "Once ICO period is launched, You can purchased Token with Etherum, Bitcoin or Litecoin. You can also tempor incididunt ut labore et dolore magna aliqua sed do eiusmod eaque ipsa.",
            },
            {
              title: "Who do not know how to pursue rationally?",
              content:
                "Once ICO period is launched, You can purchased Token with Etherum, Bitcoin or Litecoin. You can also tempor incididunt ut labore et dolore magna aliqua sed do eiusmod eaque ipsa.",
            },
            {
              title: "Their separate existence is a myth?",
              content:
                "Once ICO period is launched, You can purchased Token with Etherum, Bitcoin or Litecoin. You can also tempor incididunt ut labore et dolore magna aliqua sed do eiusmod eaque ipsa.",
            },
            {
              title: "Pityful a rethoric question ran over her cheek?",
              content:
                "Once ICO period is launched, You can purchased Token with Etherum, Bitcoin or Litecoin. You can also tempor incididunt ut labore et dolore magna aliqua sed do eiusmod eaque ipsa.",
            },
          ],
        },
        {
          name: "Token",
          quastions: [
            {
              title: "When she reached the first hills?",
              content:
                "Once ICO period is launched, You can purchased Token with Etherum, Bitcoin or Litecoin. You can also tempor incididunt ut labore et dolore magna aliqua sed do eiusmod eaque ipsa.",
            },
            {
              title: "Big Oxmox advised her not to do?",
              content:
                "Once ICO period is launched, You can purchased Token with Etherum, Bitcoin or Litecoin. You can also tempor incididunt ut labore et dolore magna aliqua sed do eiusmod eaque ipsa.",
            },
            {
              title: "Which roasted parts of sentences fly into your mouth?",
              content:
                "Once ICO period is launched, You can purchased Token with Etherum, Bitcoin or Litecoin. You can also tempor incididunt ut labore et dolore magna aliqua sed do eiusmod eaque ipsa.",
            },
            {
              title: "Vokalia and Consonantia, there live?",
              content:
                "Once ICO period is launched, You can purchased Token with Etherum, Bitcoin or Litecoin. You can also tempor incididunt ut labore et dolore magna aliqua sed do eiusmod eaque ipsa.",
            },
          ],
        },
        {
          name: "Client",
          quastions: [
            {
              title: "When she reached the first hills?",
              content:
                "Once ICO period is launched, You can purchased Token with Etherum, Bitcoin or Litecoin. You can also tempor incididunt ut labore et dolore magna aliqua sed do eiusmod eaque ipsa.",
            },
            {
              title: "Big Oxmox advised her not to do?",
              content:
                "Once ICO period is launched, You can purchased Token with Etherum, Bitcoin or Litecoin. You can also tempor incididunt ut labore et dolore magna aliqua sed do eiusmod eaque ipsa.",
            },
            {
              title: "Which roasted parts of sentences fly into your mouth?",
              content:
                "Once ICO period is launched, You can purchased Token with Etherum, Bitcoin or Litecoin. You can also tempor incididunt ut labore et dolore magna aliqua sed do eiusmod eaque ipsa.",
            },
            {
              title: "Vokalia and Consonantia, there live?",
              content:
                "Once ICO period is launched, You can purchased Token with Etherum, Bitcoin or Litecoin. You can also tempor incididunt ut labore et dolore magna aliqua sed do eiusmod eaque ipsa.",
            },
          ],
        },
        {
          name: "Legal",
          quastions: [
            {
              title: "When she reached the first hills?",
              content:
                "Once ICO period is launched, You can purchased Token with Etherum, Bitcoin or Litecoin. You can also tempor incididunt ut labore et dolore magna aliqua sed do eiusmod eaque ipsa.",
            },
            {
              title: "Big Oxmox advised her not to do?",
              content:
                "Once ICO period is launched, You can purchased Token with Etherum, Bitcoin or Litecoin. You can also tempor incididunt ut labore et dolore magna aliqua sed do eiusmod eaque ipsa.",
            },
            {
              title: "Which roasted parts of sentences fly into your mouth?",
              content:
                "Once ICO period is launched, You can purchased Token with Etherum, Bitcoin or Litecoin. You can also tempor incididunt ut labore et dolore magna aliqua sed do eiusmod eaque ipsa.",
            },
            {
              title: "Vokalia and Consonantia, there live?",
              content:
                "Once ICO period is launched, You can purchased Token with Etherum, Bitcoin or Litecoin. You can also tempor incididunt ut labore et dolore magna aliqua sed do eiusmod eaque ipsa.",
            },
          ],
        },
      ],
    };
  },
};
</script>

<style lang="scss" scoped>
.page-container {
  background-color: #0a1992;
  .page-title {
    position: relative;
    &::before {
      content: "faqs";
      transform: translate(25%,-15%);
    }
  }
  .content {
    max-width: 900px;
    width: 100%;
    .tabs {
      position: relative;
      width: 100% !important;
      .v-tab {
        text-transform: none;
      }
      ::v-deep .v-slide-group__prev {
        display: none !important;
      }
      .tab {
        color: #3479f5 !important;
        line-height: 19px;
        font-size: 17px;
        letter-spacing: 0px;
        text-align: center;
        &:hover {
          color: #46bdf4 !important;
          background-color: transparent;
        }
      }
      .line {
        position: absolute;
        width: 100%;
        height: 2px;
        bottom: 0;
        background: #737ec5;
      }
    }
    .panels {
      background-color: #091682;
      .panel {
        background: transparent !important;
        border-bottom: 1px solid #45bbf25e !important;
        &:last-child {
          border: none !important;
        }
        &::before {
          box-shadow: none !important;
        }
        .header {
          color: #d2d3ff;
          font-size: 19.2px;
          line-height: 24.96px;
          padding: 16px 54px 16px 30px;
          text-align: left;
          ::v-deep .v-icon {
            color: white !important;
          }
          transition: all 0.3s ease;
          &:hover,
          &.v-expansion-panel-header--active {
            color: #46bdf4 !important;
          }
        }
        .text {
          color: #d2d3ff;
          font-size: 15px;
          font-weight: 300;
          line-height: 25.2px;
          text-align: left;
        }
      }
    }
  }
}
::v-deep .v-tabs-items {
  background: transparent !important;
}
</style>
