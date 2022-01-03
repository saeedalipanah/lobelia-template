<template>
  <div class="container">
    <v-img src="@/assets/logo/gfx-c.png" class="blockchain-img"></v-img>
    <h1>Powering Data for the new equity blockchain</h1>
    <p>
      Global decentralize network to buy & sell shares. Solving the
      Cryptocurrency Trust problems.
    </p>
    <div class="buttons">
      <v-btn rounded>sign up to join</v-btn>
      <v-btn rounded>token distribution</v-btn>
    </div>
  </div>
</template>

<script>
export default {};
</script>

<style lang="scss" scoped>
.container {
  display: flex;
  flex-direction: column;
  align-items: center;
  // justify-content: center;
  .blockchain-img {
    width: 770px;
    height: 326px;
  }
}
</style>
