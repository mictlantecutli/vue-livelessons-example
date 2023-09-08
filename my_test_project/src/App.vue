<template>
  <CounterButton />
  
  <PeopleList />
</template>

<script>

import PeopleList from './components/PeopleList.vue';
import CounterButton from './components/CounterButton.vue';

export default {
  name: 'App',
  components: {
    PeopleList,
    CounterButton,

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
