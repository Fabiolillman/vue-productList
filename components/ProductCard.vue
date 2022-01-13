<template>
<div class="card-container">
  <div class="card-box"> 
    <p>{{productId}}</p>
    <img v-bind:src="{{productImage}}">
    <h1>{{productName}}</h1>
    <p>{{productStock}}</p>
    <p>{{productPrice}}</p>
    <p>{{productSalePrice}}</p>
    <p>{{rating}}</p>
  </div>
  </div>
</template>

<script>
export default {

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

