<script>
import Card from './Card.vue';
import {products} from '../data/db.json';
export default {

components:{
  Card,

},
data(){
  return{
    products,
  }
}

}
</script>

<template>

<main>
  <div class="container">

   <Card
     v-for="product in this.products"
     :key="product.id"
     :finalProduct="product" />
   
   
  </div>
</main>
 
</template>

<style lang="scss" scoped>
main{
  padding-top: 120px;
  display: flex;
  justify-content: center;
  .container{
    display: flex;
    flex-wrap: wrap;
    
  }
}
</style>