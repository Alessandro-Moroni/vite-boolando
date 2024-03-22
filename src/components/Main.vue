<script>
import Card from './Card.vue';
export default {

components:{
  Card,
}

}
</script>

<template>

<main>
  <div class="container">

    <Card />
    <Card />
    <Card />
    <Card />
    <Card />
    <Card />
   
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