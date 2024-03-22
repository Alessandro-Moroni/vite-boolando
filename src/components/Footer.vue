<script>
import {footerOb} from '../data/objects'

export default {

  computed: {
    mainSocial(){
      return footerOb.social
    },
  }

}
</script>

<template>

<footer>
  <div class="container">
    <div class="footer-col">
      <h4>Boolando s.r.l</h4>
      <nav>
        <ul>
          <li><a href=""></a>Informazioni legali</li>
          <li><a href=""></a>Informativa sulla privacy</li>
          <li><a href=""></a>Diritto di recesso</li>
        </ul>
      </nav>
    </div>

    <div class="footer-col">
      <h5>Trovaci anche su</h5>
      
      <p>
        <nav>
          <ul>
            <li v-for="(item, index) in mainSocial" :key="`s-${index}`"><a href="item.href" v-html="`${item.text}`"></a></li>
          </ul>
        </nav>
      </p>
    </div>
  </div>
</footer>
 
</template>

<style lang="scss" scoped>
footer{
  height: 200px;
  padding: 30px 0;
  display: flex;
  justify-content: center;
  .container{
    color: white;
    display: flex;
    justify-content: space-between;
    ul{
      display: flex;
      margin-top: 10px;
      li{
        list-style: none;
        padding-right: 10px;
        &:hover{
            cursor: pointer;
            color: gray;
          }
        a{
          color: white;
          &:hover{
            cursor: pointer;
            color: gray;
          }
        }
      }
    }
  }
}

</style>