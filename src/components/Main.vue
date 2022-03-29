<template>
  <div class="content">
    <div class="main-top">
      <div class="my-container">
        <div class="info">current series</div>
        <div class="container-card">
          <MainContent v-for="(card,index) in mainContList" :key="index" :cardElement="card" />
        </div>
        <button>Load More</button>  
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
import MainContent from './main_parts/MainContent.vue'


export default {
  name: 'homeMain',
  components: {
    MainContent,
  },
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
      ],
      mainContList:[
        {
          "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2018/09/AC1000_DLX_162-001_HD_5ba13723281ab0.37845353.jpg?itok=ZsI-C5eX",
          "price": "$19.99",
          "series": "Action Comics",
          "type": "comic book"
        },
        {
          "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2020/09/AV1976_01_300-001_HD_5f738f6e39ddd7.18205602.jpg?itok=VgdYdJ01",
          "price": "$3.99",
          "series": "American Vampire 1976",
          "type": "comic book"
        },
        {
          "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/gn-covers/2018/08/AQMv4_UW_153-001_HD_5b7efa1745a9b8.08589135.jpg?itok=HPTtnrsb",
          "price": "$16.99",
          "series": "Aquaman",
          "type": "graphic novel"
        },
        {
          "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2018/06/batgirl_v5_1_5b23e1f1124941.50950783.jpg?itok=VnrJah76",
          "price": "$2.99",
          "series": "Batgirl",
          "type": "comic book"
        },
        {
          "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2018/09/BM_56_300-001_HD_5ba137a85c3bf3.33122291.jpg?itok=3FHJQYJZ",
          "price": "$3.99",
          "series": "Batman",
          "type": "comic book"
        },
        {
          "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2018/09/BM_56_300-001_HD_5ba137a85c3bf3.33122291.jpg?itok=3FHJQYJZ",
          "price": "$2.99",
          "series": "Batman Beyond",
          "type": "comic book"
        },
        {
          "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2019/08/BMSM_5d4361b7116261.74371456.jpg?itok=kEDR2OL8",
          "price": "$3.99",
          "series": "Batman/Superman",
          "type": "comic book"
        },
        {
          "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2020/09/BMSMANN_01_300-001_HD_5f5ff17fa1d665.74704970.jpg?itok=azz5sfGk",
          "price": "$4.99",
          "series": "Batman/Superman Annual",
          "type": "comic book"
        },
        {
          "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2020/09/BMTJWZ_01_300-001_HD_5f5ff2307dcb37.34652945.jpg?itok=VswVjLR8",
          "price": "$5.99",
          "series": "Batman: The Joker War Zone",
          "type": "comic book"
        },
        {
          "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2020/08/cover-v2_5f40314645a734.37285065.png?itok=ImNM2QBY",
          "price": "$6.99",
          "series": "Batman: Three Jokers",
          "type": "comic book"
        },
        {
          "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2020/10/BMWK_HQ_01_300-001_HD_5f7cb4945e13f6.89501032.jpg?itok=sVwALbUX",
          "price": "$4.99",
          "series": "Batman: White Knight Presents: Harley Quinn",
          "type": "comic book"
        },
        {
          "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/gn-covers/2019/04/CTWv1_CC_144-001_HD_5ca5299a751963.53054221.jpg?itok=ooPaoLDq",
          "price": "$16.99",
          "series": "Catwoman",
          "type": "graphic novel"
        }
      ]
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
@import "../assets/scss/style.scss";
  .content{
    color: white;
    .main-top{
      padding-top: 1.5rem;
      background-color: rgb(29,28,28);
      padding-bottom: 1rem;
      .my-container{
        position: relative;
        align-items: center;
        justify-content: center;
        flex-direction: column;
        .info{
          position: absolute;
          bottom: 101%;
          left: 0;
          background-color: $colorPrimary;
          padding: 7px;
          font-size: 1.2rem;
          font-weight: bold;
          text-transform: uppercase;
        }
        .container-card{
          display: flex;
          justify-content: center;
          flex-wrap: wrap;
        }
        button{
          margin: 2.5rem auto 0;
          border-color: $colorPrimary;
          background-color: $colorPrimary;
          display: inline-block;
          font-weight: 400;
          line-height: 1.5;
          color: white;
          text-align: center;
          text-decoration: none;
          vertical-align: middle;
          border: 1px solid transparent;
          padding: 0.375rem 2.5rem;
          font-size: 1rem;
        }
      }
    }
    .main-bottom{
      background-color: $colorPrimary;
      height: 100px;
      .my-container {
        height: 100%;
        .item{
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
  }

</style>
