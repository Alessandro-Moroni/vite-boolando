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

    <h1>header</h1>

    <nav>
      <ul>
        <li><a href=""></a>Donna</li>
        <li><a href=""></a>Uomo</li>
        <li><a href=""></a>Bambini</li>
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
    ul{
      display: flex;
      li{
        padding: 10px;
        list-style: none;
        color: white;
        a{
          text-decoration: none;
        }
      }
    }
  }
}
</style>