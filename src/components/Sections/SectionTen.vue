<template>
  <div class="contanier blue lighten-2">
    <v-container>
      <v-row>
        <v-col class="grey">
          <v-timeline>
            <v-timeline-item
              v-for="(year, i) in years"
              :key="i"
              :color="year.color"
              small
            >
              <template v-slot:opposite>
                <span
                class="red"
                  :class="`headline font-weight-bold ${year.color}--text`"
                  v-text="year.year"
                ></span>
              </template>


              <div class="title py-4 yellow">
                <h2
                class="white"
                  :class="`headline font-weight-light mb-4 ${year.color}--text`"
                >
                  Lorem ipsum
                </h2>
                <div class="content blue">
                  Lorem ipsum dolor sit amet, no nam oblique veritus. Commune
                  scaevola imperdiet nec ut, sed euismod convenire principes at.
                  Est et nobis iisque percipit, an vim zril disputando
                  voluptatibus, vix an salutandi sententiae.
                </div>
              </div>
            </v-timeline-item>
          </v-timeline>
        </v-col>
      </v-row>
    </v-container>
  </div>
</template>

<script>
export default {
  data() {
    
        return {
          years: [
            {
              color: "black",
              year: "1960",
            },
            {
              color: "green",
              year: "1970",
            },
            {
              color: "pink",
              year: "1980",
            },
            {
              color: "amber",
              year: "1990",
            },
            {
              color: "orange",
              year: "2000",
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
  .content {
    .actions {
      width: 80%;
      background: red;
    }
  }
}
</style>
