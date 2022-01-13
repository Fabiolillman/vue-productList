<template>
<div class="card-container">
  <div v-for="product in products" v-bind:key="product.productId" class="card-box">  
      <img v-bind:src="{{product.productImage}}">
      <h1>{{product.productName}}</h1>
      <p>{{product.productStock}}</p>
      <p>{{product.productPrice}}</p>
      <p>{{product.productSalePrice}}</p>
      <p>{{product.rating}}</p>
  </div>
  </div>
</template>

<script>
export default {
  data(){
    return{
      props:['products']
    }
  }

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

