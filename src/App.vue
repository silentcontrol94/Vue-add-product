<template>
  <div class="container">
    <h1 class="text-center">Ürün Ekleme Uygulaması</h1>
    <hr>
    <app-new-product></app-new-product>
    <br><br>
    <app-progress></app-progress>
    <br><br>
    <h3 class="text-center">Eklenen Ürünlerin Listesi</h3>
    <hr>
    <app-products></app-products>

  </div>


</template>

<script>
import NewProduct from "./Components/NewProduct";
import Product from "./Components/Product";
import Products from "./Components/Products";
import Progress from "./Components/Progress";

  export default {
    components : {
      appNewProduct : NewProduct,
      appProduct : Product,
      appProducts : Products,
      appProgress : Progress
    },
    data() {
      return {
      }
    },
  }
</script>

<style>
  body {
    background-color: aliceblue;
    padding-top: 20px;
    padding-bottom: 20px;
  }

  .card{
    margin-right: 5px;
    margin-bottom: 5px;
  }

  .card:last-child{
    margin-right: 0px;
  }

  .col-md-2{
    max-width: 15.666667%!important;
  }

  .product-container{
    margin-left: 15px;
  }

</style>

