<template>
  <div class="timer ">
    <div class="timer-body" v-if="!isEnd">
      <div class="">
        <span class="time" v-if="time.day < 10">0</span>
        <span class="time"> {{ time.day }}</span>
        <span class="time points">:</span>

        <p>Days</p>
      </div>
      <div class="">
        <span class="time" v-if="time.hour < 10">0</span>
        <span class="time">{{ time.hour }}</span>
        <span class="time points">:</span>

        <p>Hours</p>
      </div>
      <div class="">
        <span class="time" v-if="time.min < 10">0</span>
        <span class="time">{{ time.min }}</span>
        <span class="time points">:</span>

        <p>Min</p>
      </div>
      <div class="">
        <span class="time" v-if="time.sec < 10">0</span>
        <span class="time">{{ time.sec }}</span>

        <p>Sec</p>
      </div>
    </div>
    <div v-else>Time Over !</div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      time: {
        day: 66,
        hour: 23,
        min: 59,
        sec: 59,
      },
      isEnd: false,
    };
  },
  created() {
    this.timeDecrease();
  },
  methods: {
    timeDecrease() {
      setInterval(() => {
        this.time.sec--;
        if (this.time.sec == 0) {
          this.time.min--;
          this.time.sec = 59;
        } else if (this.time.min == 0) {
          this.time.hour--;
          this.time.min = 59;
        } else if (this.time.hour == 0) {
          this.time.day--;
          this.time.hour = 23;
        } else if (
          this.time.day == 0 &&
          this.time.hour == 0 &&
          this.time.min == 0
        ) {
          this.isEnd = true;
        }
      }, 100);
    },
  },
};
</script>

<style lang="scss" scoped>
.timer {
  width: 100%;
  min-width: 350px;
  @media only screen and (max-width: 450px) {
    min-width: 280px;
  }
  .timer-body {
    display: flex;
    .time {
      color: #ffffff;
      font-size: 46.4px;
      font-weight: 300;
      line-height: 50px;
      text-align: center;
      &.points {
        margin:0 16px;
        @media only screen and (max-width: 450px) {
          margin:0 5px
        }
      }
    }

    p {
      color: #aeafff;
      font-size: 12px;
      font-weight: 500;
      letter-spacing: 0.12px;
      line-height: 20.16px;
      text-transform: capitalize;
      padding-left: 12px;
    }
  }
}
</style>
