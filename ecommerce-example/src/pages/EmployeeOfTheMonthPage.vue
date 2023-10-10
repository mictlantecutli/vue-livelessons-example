<template>
  <h1 v-flash="1000">Employee Of The Month</h1>
  <div v-if="personData">
    <h3>{{ personData.name.last }} {{ personData.name.first }}</h3>
  </div>
</template>

<script>
/*To install axios is into the project in the terminal type: npm install axios*/
/*Then this is to use instead fetch and it is more direct to make a call. Look in line 21 how to use that*/
/*import axios from 'axios';*/
import randomPersonMixin from '../mixins/randomPersonMixin';
  export default{
    name: 'EmployeeOfTheMonthPage',
    mixins: [randomPersonMixin],
    


  }
</script>