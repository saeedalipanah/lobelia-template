<template>
  <div class="container">
    <div class="triangle"></div>
  </div>
</template>

<script>
export default {};
</script>

<style lang="scss" scoped>
.container {
  display: flex;
  justify-content: center;
  align-items: center;
  width: 60px;
  height: 60px;
  position: relative;
  background-color: #0a1992;
  border-radius: 50%;
  border: 2px solid #44b6f4;
  cursor: pointer;
  .triangle {
    position: absolute;
    left: 55%;
    right: 50%;
    transform: translate(-50%, 0%);
    width: 0;
    height: 0;
    border-top: 13px solid transparent;
    border-left: 13px solid rgb(69, 233, 255);
    border-bottom: 13px solid transparent;
  }
  &::before {
    content: "";
    top: -1px;
    left: -2px;
    width: 105%;
    height: 105%;
    position: absolute;
    border: 1px solid #44b6f4;
    border-radius: 50%;
    z-index: 100;
    animation: scale 1.2s ease infinite;
  }
}
@keyframes scale {
  0% {
    transform: scale(1);
    opacity: 1;
  }
  100% {
    transform: scale(1.8);
    opacity: 0;
  }
  // 100%{
  //     transform: scale(1);
  //     opacity: 1;
  // }
}
</style>
