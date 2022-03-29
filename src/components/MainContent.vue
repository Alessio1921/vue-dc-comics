<template>
  <div class="content">
    <div class="main-top">
      <div class="my-container">
        <h2>--> Content goes here </h2>
      </div>
    </div>
    <div class="main-bottom">
      <div class="my-container">
        <div class="item" v-for="(item,index) in listItem" :key="index">
          <img :src="item.img" alt="">
          <p>{{item.name}}</p>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import digitalComics from "../assets/img/buy-comics-digital-comics.png"
import dcMerchiandise from "../assets/img/buy-comics-merchandise.png"
import subscription from "../assets/img/buy-comics-subscriptions.png"
import comicShop from "../assets/img/buy-comics-shop-locator.png"
import dcVisa from "../assets/img/buy-dc-power-visa.svg"

export default {
  name: 'MainContent',
  data: function(){
    return{
      listItem:[
        {
          name:"digital Comics",
          img:digitalComics,
          url:"#"
        },
        {
          name:"dc Merchiandise",
          img:dcMerchiandise,
          url:"#"
        },
        {
          name:"subscription",
          img:subscription,
          url:"#"
        },
        {
          name:"comic Shop Locator",
          img:comicShop,
          url:"#"
        },
        {
          name:"dc power Visa",
          img:dcVisa,
          url:"#"
        }
      ]
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
  .my-container{
    display: flex;
    align-items: center;
    height: 100%;
  }
  .content{
    height: 200px;
    color: white;
    .main-top{
      height: 100px;
      background-color: rgb(29,28,28);
      
    }
    .main-bottom{
      background-color: rgb(56,128,241);
      height: 100px;
      .my-container .item{
        height: 100%;
        display: flex;
        align-items: center;
        img{
          padding: 30px;
          height: 100%;
        }
        p{
          text-transform: uppercase;
          font-size: .8rem;
        }
      }
    }
  }
</style>
