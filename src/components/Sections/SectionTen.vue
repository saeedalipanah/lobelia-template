<template>
  <div class="page-container">
    <div class="page-title-container">
      <h1 class="page-title observe">OUR ROADMAP</h1>
    </div>
    <v-container>
      <v-row>
        <v-col class="">
          <timeline-item
            v-for="(item, i) in items"
            :key="i"
            :title="item.title"
            :body="item.body"
            :isRight="item.isRight"
            :isChecked="item.isChecked"
            class="observe"
          ></timeline-item>
        </v-col>
      </v-row>
    </v-container>
  </div>
</template>

<script>
import TimelineItem from "@/components/UI/TimelineItem.vue";
export default {
  data() {
    return {
      items: [
        {
          title: "March 2018",
          body: "Many desktop publishing packages and web page editors now use Lorem Ipsum as their default model text",
          isRight: true,
          isChecked: true,
        },

        {
          title: "May 2018",
          body: "Start of the ICO Crypto Platform Development. It is a long established fact that a reader will be distracted.",
          isRight: false,
          isChecked: true,
        },

        {
          title: "July 2018",
          body: "Nor again is there anyone who loves or pursues or desires to obtain pain of itself, because it is pain",
          isRight: true,
          isChecked: false,
        },

        {
          title: "September 2018",
          body: "Neque porro quisquam est, qui dolorem ipsum quia dolor sit amet, consectetur, adipisci velit, sed quia non",
          isRight: false,
          isChecked: false,
        },

        {
          title: "November 2018",
          body: "Nor again is there anyone who loves or pursues or desires to obtain pain of itself, because it is pain",
          isRight: true,
          isChecked: false,
        },
        {
          title: "January 2019",
          body: "Nam libero tempore, cum soluta nobis est eligendi optio cumque nihil impedit quo minus id quod maxime",
          isRight: false,
          isChecked: false,
        },
      ],
    };
  },
  components: {
    TimelineItem,
  },
};
</script>

<style lang="scss" scoped>
.page-container {
  background-color: #000537;
  .content {
    .actions {
    }
  }
}
</style>
