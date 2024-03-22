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
      
      <div class="sold">

        <span v-for="discount in finalProduct.badges" :key="discount" :class="discount.type" class="badge discount">{{ discount.value }}</span>

        <span></span>
      </div>
     
    </div>
    <p>{{ finalProduct.brand }}</p>
    <h3>{{ finalProduct.name }}</h3>
    <p>{{ finalProduct.price }} €</p>
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
    .sold{
      position: absolute;
      bottom: 20px;
      color: white;
    }

  }
}
.discount{
  background-color: red;
  padding: 7px 18px;

}
.tag{
  background-color: green;
  margin-right: 5px;
}

.photo:hover .first-photo{
  display: none;
}
.photo:hover .second-photo{
  display: inline-block;
}
</style>