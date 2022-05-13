<template>
  <product-list-one v-bind:products="products"></product-list-one>
  <product-list-two v-bind:products="products"></product-list-two>
</template>

<script>
import ProductListOne from './components/ProductListOne.vue';
import ProductListTwo from './components/ProductListTwo.vue';

export default {
  name: 'App',
  components:{
    'product-list-one': ProductListOne,
    'product-list-two': ProductListTwo
  },
 
  data(){
    return{
      products: [
        {
          name: 'Banana Skin',
          price: 40,
        },
        {
          name: 'Green Shells',
          price: 40,
        },
        {
          name: 'Green Shells',
          price: 40,
        },
        {
          name: 'Green Shells',
          price: 80,
        }
      ]
    }
  }
}
</script>

<style>
body{
    font-family: Ubuntu;
    color: #555;
}
</style>
