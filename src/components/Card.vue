<script>

  export default {
    props:{
      finalProduct: Object,
    }
  }
</script>

<template>

  <div class="card">
    <div class="photo">
      <img class="first-photo" :src="`/imgcard/${finalProduct.frontImage}`" alt="">
      <img class="second-photo" :src="`/imgcard/${finalProduct.backImage}`" alt="">

      <div class="heart">&#9829;</div>
      <div class="sold-1">-50</div>
      <div class="sold-2">sostenibilita</div>
    </div>
    <p>levis</p>
    <h3>relaxed</h3>
    <p>14€</p>
  </div>
  
</template>


<style lang="scss" scoped>
.card{
  width: calc(100% / 3);
  padding: 5px;
  font-size: 1.2rem;
  margin-bottom: 20px;
  .photo{
    position: relative;
    cursor: pointer;

    .first-photo{
      width: 100%;
      height: 100%;
      display: inline-block;
    
    }
    .second-photo{
      width: 100%;
      height: 100%;
      display: none;

    }
    .heart{
      position: absolute;
      right: 0;
      top: 10px;
      padding: 10px 17px;
      background-color: white;
      font-size: 2rem;
    }
    .sold-1{
      position: absolute;
      bottom: 20px;
      background-color: red;
      padding: 7px 10px;
      color: white;
    }
    .sold-2{
      position: absolute;
      bottom: 20px;
      left: 50px;
      background-color: green;
      padding: 7px 10px;
      color: white;
    }
  }
}

.photo:hover .first-photo{
  display: none;
}
.photo:hover .second-photo{
  display: inline-block;
}
</style>