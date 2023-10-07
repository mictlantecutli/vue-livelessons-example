<template>
  <h1>Employee Of The Month</h1>
  <div v-if="personData">
    <h3>{{ personData.name.last }} {{ personData.name.first }}</h3>
  </div>
</template>

<script>
/*To install axios is into the project in the terminal type: npm install axios*/
/*Then this is to use instead fetch and it is more direct to make a call. Look in line 21 how to use that*/
import axios from 'axios'
  export default{
    name: 'EmployeeOfTheMonthPage',
    data(){
      return{
        personData: null,
      }

    },
    created(){
      axios.get('https://randomuser.me/api/')
      .then(response => this.personData=response.data.results[0])
    }


  }
</script>