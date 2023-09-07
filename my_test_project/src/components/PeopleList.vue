<template>
  <h1>People List</h1>
  <PeopleListItem name="Monica" :age="34" hairColor="brown"/>
  <PeopleListItem name="Carlos" :age="45" hairColor="blue"/>
  <PeopleListItem name="Yenny" :age="23" hairColor="yellow"/>

</template>
<script>
import PeopleListItem from './PeopleListItem.vue';
export default{
  name: 'PeopleList',
  components: {
    PeopleListItem,

  }
}
</script>