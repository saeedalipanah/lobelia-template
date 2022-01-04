<template>
  <div class="timeline-item">
    <div class="content">
      <div class="text-left block" v-if="!isRight">
        <h3 class="title">{{ title }}</h3>
        <p class="text text-end">
          {{body}}
        </p>
      </div>
    </div>
    <div class="line">
      <i
        class="circle-icon d-flex justify-center align-center"
        :class="`${isChecked ? 'checked' : ''}`"
        v-if="isChecked"
      >
        <i class="fas fa-check d-flex"></i>
      </i>
      <i class="circle-icon" v-else> </i>
    </div>
    <div class="content">
      <div class="text-right block" v-if="isRight">
        <h3 class="title">{{ title }}</h3>
        <p class="text text-start">
         {{body}}
        </p>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  props: ["isRight", "isChecked", "title","body"],
};
</script>

<style lang="scss" scoped>
.timeline-item {
  display: flex;
  justify-content: center;
  height: 120px;
  .content {
    width: 100%;
    max-width: 500px;
    position: relative;
    .block {
      display: flex;
      flex-direction: column;
      position: absolute;
      padding: 0 35px;
      top: 45px;

      &.text-left {
        align-items: end;
        right: 0;
      }

      &.text-right {
        align-items: start;
        left: 0;
      }

      .title {
        color: #ffffff;
        font-size: 14px !important;
        font-weight: 600;
        line-height: 23.52px;
        text-transform: capitalize;
        margin-bottom: 16px;
      }
      .text {
        color: #d2d3ff;
        font-size: 15px;
        font-weight: 300;
        line-height: 25.2px;
      }
    }
  }
  .line {
    height: 100%;
    width: 2px;
    background: #46bdf4;
    position: relative;
    display: flex;
    justify-content: center;
    align-items: center;
    .circle-icon {
      position: absolute;
      height: 25px;
      width: 25px;
      border-radius: 50%;
      background: #46bdf4;
      border: 1px solid #46bdf4;
      &.checked {
        background: #0a1992;
        border: 1px solid #46bdf4;
      }
      .fas {
        color: #46bdf4;
      }
    }
  }
}
</style>
