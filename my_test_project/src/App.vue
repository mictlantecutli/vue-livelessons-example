<template>
  <FlashingMessage message="Hellow friends!!" :delay="500"/>
</template>

<script>

import FlashingMessage from './components/FlashingMessage.vue';

export default {
  name: 'App',
  components: {
    
    FlashingMessage
    
},
  data(){
    return{
      numberOfClicks: 0,
    }

  },
  methods:{
    increment(){
      this.numberOfClicks += 1
    },
    onTick(name){
      console.log(name + 'Tick!!')
    }
  }
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
