<template>
  <h2>Available Items:</h2>
  <div v-for="product in products" :key="product.id">
    <router-link :to="`/products/${product.id}`">
      <h3>{{ product.name }}</h3>
    </router-link>
    <p>{{ product.price }}</p>
    <button>Add to Cart</button>
  </div>

</template>
<script>
import products from './products';
  export default{
    name:'ProductsListPage',
    data(){
      return{
        products,
      }
    }
  }
</script>