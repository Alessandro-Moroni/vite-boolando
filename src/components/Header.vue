<script>
import {headerOb} from '../data/objects'

export default {

  computed: {
    mainMenu(){
      return headerOb.main
    },
    mainSocial(){
      return headerOb.social
    },
  }


}
</script>

<template>

<header>
  <div class="container">

    <nav>
      <ul>
        <li v-for="(item, index) in mainMenu" :key="`m-${index}`" ><a href="item.href">{{ item.text }}</a></li>
        
      </ul>
    </nav>

    
    <img class="logo" src="/src/assets/img/boolean-logo.png" alt="">
  

    <nav>
      <ul>
        <li v-for="(item, index) in mainSocial" :key="`s-${index}`"><a href="item.href" v-html="`${item.text}`"></a></li>
        
      </ul>
    </nav>
  </div>
</header>
 
</template>

<style lang="scss" scoped>

header{
  height: 120px;
  width: 100%;
  position: fixed;
  z-index: 1;
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
        &:hover{
          cursor: pointer;
          text-decoration: underline;
          color: white;
        }
        a{
          color: white;
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