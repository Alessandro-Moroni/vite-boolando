<script>
export default {

  data() {
    return{
     
    }
  },


}
</script>

<template>

<header>
  <div class="container">

    <nav>
      <ul>
        <li><a href=""></a>Donna</li>
        <li><a href=""></a>Uomo</li>
        <li><a href=""></a>Bambini</li>
      </ul>
    </nav>

    
    <img class="logo" src="/src/assets/img/boolean-logo.png" alt="">
  

    <nav>
      <ul>
        <li><a href=""></a><i class="fa-regular fa-user"></i></li>
        <li><a href=""></a><i class="fa-regular fa-heart"></i></li>
        <li><a href=""></a><i class="fa-solid fa-bag-shopping"></i></li>
      </ul>
    </nav>
  </div>
</header>
 
</template>

<style lang="scss" scoped>

header{
  height: 150px;
  display: flex;
  align-items: center;
  justify-content: center;
  div{
    display: flex;
    justify-content: space-between;
    align-items: center;
    ul{
      display: flex;
      li{
        padding: 10px;
        list-style: none;
        color: white;
        &:hover{
          cursor: pointer;
            text-decoration: underline;
          }
        a{
          text-decoration: none;
         
        }
      }
    }
  }
}

.logo{
  width: 30%;
  height: 30%;
 
}
</style>