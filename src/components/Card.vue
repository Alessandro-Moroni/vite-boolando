<script>
  export default {
   
  }
</script>

<template>

  <div class="card">
    <div class="photo">
      <img src="../assets/img/1.webp" alt="">
      <div class="heart">&#9829;</div>
      <div class="sold-1">-50</div>
      <div class="sold-2">sostenibilita</div>
    </div>
    <p>levis</p>
    <p>relaxed</p>
    <p>14</p>
  </div>
  
</template>


<style lang="scss" scoped>
.card{
  width: calc(100% / 3);
  padding: 5px;
  font-size: 1.2rem;
  .photo{
    position: relative;

    img{
      width: 100%;
      height: 100%;
    };
    .heart{
      position: absolute;
      right: 0;
      top: 10px;
      padding: 10px;
      background-color: white;
      font-size: 2rem;
    }
    .sold-1{
      position: absolute;
      bottom: 20px;
      left: 10px;
      background-color: red;
      padding: 7px;
    }
    .sold-2{
      position: absolute;
      bottom: 20px;
      left: 60px;
      background-color: green;
      padding: 7px;
    }
  }
}
</style>