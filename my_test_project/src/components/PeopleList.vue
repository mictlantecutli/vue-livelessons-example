<template>
  <h1>People List</h1>
  <PeopleListItem :person="person1" />
  <PeopleListItem :person="person2" />
  <PeopleListItem :person="person3" />

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
        person1: {name: 'Monica', age: 34, hairColor: 'brown' },
        person2: {name:'Carlos', age: 45, hairColor: 'blue'},
        person3: {name: 'Yenny', age: 23, hairColor: 'Yellow'}
      }
    }
  
}
</script>