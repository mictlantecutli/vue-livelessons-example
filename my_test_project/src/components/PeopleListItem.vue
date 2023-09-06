<template>
  <div>
    <h3>{{ name }}</h3>
    <p>Age: {{ age }} years</p>
    <p>Hair Color: {{ hairColor }}</p>
  </div>
</template>

<script>
export default{
  name:'PeopleListItem',
  data(){
    return{
      name: 'Moisés',
      age: 40,
      hairColor: 'black',
    }
  }
}
</script>