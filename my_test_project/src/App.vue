<template>
  <Congratulations_user :numberOfClicks="numberOfClicks" />
  <CounterButton @increment="increment" :numberOfClicks="numberOfClicks" />
  
  <PeopleList />
</template>

<script>

import PeopleList from './components/PeopleList.vue';
import CounterButton from './components/CounterButton.vue';

import Congratulations_user from './components/Congratulations.vue';

export default {
  name: 'App',
  components: {
    PeopleList,
    CounterButton,
    Congratulations_user,
    
},
  data(){
    return{
      numberOfClicks: 0,
    }

  },
  methods:{
    increment(){
      this.numberOfClicks += 1
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
