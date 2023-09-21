<template>
  <LifecycleTest v-if="numberOfClicks < 10" :numberOfClicks="numberOfClicks" />
  <Congratulations_user :numberOfClicks="numberOfClicks" />
  <CounterButton @increment="increment" :numberOfClicks="numberOfClicks" />
  <TimerComponent @tick="onTick" name="Timer 1" :delay="2000" />
  <TimerComponent @tick="onTick" name="Time 2" :delay="5000" />
  <PeopleList />
</template>

<script>

import PeopleList from './components/PeopleList.vue';
import CounterButton from './components/CounterButton.vue';

import Congratulations_user from './components/Congratulations.vue';
import LifecycleTest from './components/LifecycleTest.vue';
import TimerComponent from './components/Timer.vue';

export default {
  name: 'App',
  components: {
    PeopleList,
    CounterButton,
    Congratulations_user,
    LifecycleTest,
    TimerComponent
    
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
