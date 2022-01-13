<template>
 
    <div class="card-box">  
      <img v-bind:src="product.productImage">
      <h1>{{product.productName}}</h1>
      <p>{{product.productStock}}</p>
      <p>{{product.productPrice}}</p>
      <p>{{product.productSalePrice}}</p>
      <p>{{product.rating}}</p>
    
  </div>
</template>

<script>
export default {
 props:['product']
  }

</script>

<style scoped>
 .card-container{
   display: flex;
   justify-content: center;
   align-items: center;
 }
 .card-box{
   width: 400px;
   height: 400px;
   border: 1px solid black;
 }
</style>

