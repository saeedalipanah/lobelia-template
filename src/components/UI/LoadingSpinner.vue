<template>
  <div class="semipolar-spinner" >
  <div class="ring"></div>
  <div class="ring"></div>
  <div class="ring"></div>
  <div class="ring"></div>
  <div class="ring"></div>
</div>
</template>

<script>
export default {

}
</script>

<style lang="scss" scoped>
.semipolar-spinner, .semipolar-spinner * {
      box-sizing: border-box;
    }

    .semipolar-spinner {
      height: 80px;
      width: 80px;
      position: relative;
    }

    .semipolar-spinner .ring {
      border-radius: 50%;
      position: absolute;
      border: calc(80px * 0.05) solid transparent;
      border-left-color: #7216fe;
      border-bottom-color: #43b0f4;
      border-top: gray;
      animation: semipolar-spinner-animation 3s infinite;
    }

    .semipolar-spinner .ring:nth-child(1) {
      height: calc(80px - 80px * 0.2 * 0);
      width: calc(80px - 80px * 0.2 * 0);
      top: calc(80px * 0.1 * 0);
      left: calc(80px * 0.1 * 0);
      animation-delay: calc(1500ms * 0.1 * 4);
      z-index: 5;
    }

    .semipolar-spinner .ring:nth-child(2) {
      height: calc(80px - 80px * 0.2 * 1);
      width: calc(80px - 80px * 0.2 * 1);
      top: calc(80px * 0.1 * 1);
      left: calc(80px * 0.1 * 1);
      animation-delay: calc(1500ms * 0.1 * 3);
      z-index: 4;
    }

    .semipolar-spinner .ring:nth-child(3) {
      height: calc(80px - 80px * 0.2 * 2);
      width: calc(80px - 80px * 0.2 * 2);
      top: calc(80px * 0.1 * 2);
      left: calc(80px * 0.1 * 2);
      animation-delay: calc(1500ms * 0.1 * 2);
      z-index: 3;
    }

    .semipolar-spinner .ring:nth-child(4) {
      height: calc(80px - 80px * 0.2 * 3);
      width: calc(80px - 80px * 0.2 * 3);
      top: calc(80px * 0.1 * 3);
      left: calc(80px * 0.1 * 3);
      animation-delay: calc(1500ms * 0.1 * 1);
      z-index: 2;
    }

    .semipolar-spinner .ring:nth-child(5) {
      height: calc(80px - 80px * 0.2 * 4);
      width: calc(80px - 80px * 0.2 * 4);
      top: calc(80px * 0.1 * 4);
      left: calc(80px * 0.1 * 4);
      animation-delay: calc(1500ms * 0.1 * 0);
      z-index: 1;
    }

    @keyframes semipolar-spinner-animation {
      50% {
        transform: rotate(560deg) scale(.7);
      }
    }
</style>