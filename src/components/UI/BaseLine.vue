<template>
  <div class="parent">
    <div class="line"></div>
  </div>
</template>

<script>
export default {};
</script>

<style lang="scss" scoped>
.parent {
  position: relative;
  font-size: 15px; 
  @media only screen and(max-width: 960px) {
    font-size: 10px;
  }
  @media only screen and(max-width: 768px) {
    font-size: 8px;
  }
  .line {
    width: 0.1875em;
    height: 9.375em;
    background-color: #3479f5;
    position: absolute;
    right: 50%;
    left: 50%;
    transform: translate(-50%, -50%);
  }
}
</style>
