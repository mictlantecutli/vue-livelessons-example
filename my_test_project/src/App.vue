<template>
  <h1>My Vue Component</h1>
  <PeopleList />
</template>

<script>

import PeopleList from './components/PeopleList.vue';
export default {
  name: 'App',
  components: {
    PeopleList,

  }
}
</script>

<style scoped>
h1 {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
