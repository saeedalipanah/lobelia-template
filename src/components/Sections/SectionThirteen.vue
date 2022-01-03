<template>
  <div class="contanier yellow lighten-2">
    <div class="title">
      <h1>FREQUENTLY ASKED QUESTION</h1>
      <p>
        Below we’ve provided a bit of ICO, ICO Token, cryptocurrencies, and few
        others. If you have any other questions, please get in touch using the
        contact form below.
      </p>
    </div>
    <v-container>
      <v-row justify="center">
        <v-col class="red">
          <v-tabs
            class="tabs"
            v-model="tab"
            background-color="transparent"
            color="blue"
            grow
          >
            <v-tab v-for="(tab, i) in tabs" :key="i" class="white--text">
              {{ tab.name }}
            </v-tab>
          </v-tabs>
          <v-tabs-items v-model="tab">
            <v-tab-item v-for="(tab, i) in tabs" :key="i">
              <v-expansion-panels accordion>
                
                <v-expansion-panel v-for="(quastion, i) in tabs[i].quastions" :key="i">
                  
                  <v-expansion-panel-header>{{
                    quastion.title
                  }}</v-expansion-panel-header>
                  <v-expansion-panel-content>
                    {{quastion.content}}
                  </v-expansion-panel-content>
                </v-expansion-panel>
              </v-expansion-panels>
            </v-tab-item>
          </v-tabs-items>
        </v-col>
      </v-row>
    </v-container>
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
.contanier {
  .title {
    display: flex;
    flex-direction: column;
    align-items: center;
    text-align: center;
  }
  .tabs {
    border-bottom: 3px solid black;
  }
}
</style>
