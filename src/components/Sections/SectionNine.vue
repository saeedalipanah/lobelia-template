<template>
  <div class="page-container">
    <v-container>
      <v-row>
        <v-col md="6" class="grey">
          <h1>Distribution of tokens</h1>
          <v-img src="@/assets/logo/chart-1.png"></v-img>
        </v-col>
        <v-col md="6" class="yellow d-flex flex-column align-center">
          <h1>Use of proceeds</h1>
          <v-img src="@/assets/logo/chart-2.png"></v-img>
        </v-col>
      </v-row>
    </v-container>
  </div>
</template>

<script>
export default {
  data() {
    return {};
  },
};
</script>

<style lang="scss" scoped>
.page-container {
 
  .content {
    .actions {
      width: 80%;
      background: red;
    }
  }
}
</style>
