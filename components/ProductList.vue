<template>
  
    <div>
      <ProductCard  v-for="product in products" v-bind:key="product.productId" ProductList v-bind:products="products">
        
      </ProductCard>
    </div>

     
</template>

<script>

import ProductCard from './ProductCard.vue'

export default {
   
  props:['products'],
  components: {ProductCard}


}
</script>

<style>

</style>