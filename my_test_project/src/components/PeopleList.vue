<template>
  <h1>People List</h1>
  <PeopleListItem v-for="person in people" :key="person.name" :person="person"/>


</template>
<script>
import PeopleListItem from './PeopleListItem.vue';
export default{
  name: 'PeopleList',
  components: {
    PeopleListItem,
  },
  data(){
      return{
        people: [
          {name: 'Monica', age: 34, hairColor: 'brown' },
          {name:'Carlos', age: 45, hairColor: 'blue'},
          {name: 'Yenny', age: 23, hairColor: 'Yellow'}
      
        ],
      }
    }
  
}
</script>