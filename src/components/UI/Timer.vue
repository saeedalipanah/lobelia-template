<template>
  <div class="timer-container ">
      <h2>Day{{time.day}}</h2>
      <h2>hour{{time.hour}}</h2>
      <h2>min{{time.min}}</h2>
      <h2>sec{{time.sec}}</h2>
  </div>
</template>

<script>
export default {
data(){
    return{
        time:{
            day:'66',
            hour:'23',
            min:'59',
            sec:'59'
        }
    }
},
created(){
    this.timeDecrease();
},
methods:{
    timeDecrease(){
        setInterval(() => {
            this.time.sec --;
        }, 1000);
    }
}
}
</script>

<style>

</style>
