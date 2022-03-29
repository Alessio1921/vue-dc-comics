<template>
  <div class="footer">
    <div class="footer-top">
      <div class="my-container">
        <div class="list">
          <div class="list-left">
            <ul>
              <li>Dc comics</li>
              <li v-for="(item,index) in listDccomics" :key="index">
                <a :href="item.url">{{item.name}}</a>
              </li>
            </ul>
            <ul>
              <li>Shop</li>
              <li v-for="(item,index) in listShop" :key="index">
                <a :href="item.url">{{item.name}}</a>
              </li>
            </ul>
          </div>
          
          <ul>
            <li>dc</li>
            <li v-for="(item,index) in listDc" :key="index">
              <a :href="item.url">{{item.name}}</a>
            </li>
          </ul>

          <ul>
            <li>Sites</li>
            <li v-for="(item,index) in listSites" :key="index">
              <a :href="item.url">{{item.name}}</a>
            </li>
          </ul>
        </div>
        <div class="footer-logo">
        </div>
      </div>
    </div>
    <div class="footer-bottom">
      <div class="my-container">
        <button>sign-up-now!</button>
        <div class="social">
          <h3>follow us</h3>
          <img v-for="(item,index) in listSocial" :key="index" :src="item.img" alt="" >
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import facebookLogo from "../assets/img/footer-facebook.png"
import twitterLogo from "../assets/img/footer-twitter.png"
import youtubeLogo from "../assets/img/footer-youtube.png"
import pinterestLogo from "../assets/img/footer-pinterest.png"
import periscopeLogo from "../assets/img/footer-periscope.png"

export default {
  name: 'homeFooter',
  data: function(){
    return{
      listDccomics:[
        {
          name:"characters",
          url:"#"
        },
        {
          name:"comics",
          active:true,
          url:"#"
        },
        {
          name:"movies",
          url:"#"
        },
        {
          name:"games",
          url:"#"
        },
        {
          name:"collectibles",
          url:"#"
        },
        {
          name:"videos",
          url:"#"
        },
        {
          name:"fans",
          url:"#"
        },
        {
          name:"news",
          url:"#"
        },
        {
          name:"shop",
          url:"#"
        }
      ],
      listShop:[
        {
          name:"Shop Dc",
          url:"#"
        },
        {
          name:"Shop Dc Colletibles",
          url:"#"
        }  
      ],
      listDc:[
        {
          name: "Term Of Use",
          url: "#"
        },
        {
          name: "Privacy policy (New)",
          url: "#"
        },
        {
          name: "Ad Choise",
          url: "#"
        },
        {
          name: "Advertising",
          url: "#"
        },
        {
          name: "Jobs",
          url: "#"
        },
        {
          name: "Subscriptions",
          url: "#"
        },
        {
          name: "Talent Workshop",
          url: "#"
        },
        {
          name: "CPSC Certificates",
          url: "#"
        },
        {
          name: "Ratings",
          url: "#"
        },
        {
          name: "Shop Help",
          url: "#"
        },
        {
          name: "Contact Us",
          url: "#"
        }
      ],
      listSites:[
        {
          name: "DC",
          url: "#"
        },
        {
          name: "MAD Magazine",
          url: "#"
        },
        {
          name: "DC Kids",
          url: "#"
        },
        {
          name: "DC Universe",
          url: "#"
        },
        {
          name: "Dc Power Visa",
          url: "#"
        }
      ],
      listSocial:[
        {
        img:facebookLogo,
        },
        {
          img:twitterLogo,
        },
        {
          img:youtubeLogo,
        },
        {
          img:pinterestLogo,
        },
        {
          img:periscopeLogo,
        }
      ]
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
@import "../assets/scss/style.scss";
  .footer-top{
    background-image: url(../assets/img/footer-bg.jpg);
    height: 350px;
    .my-container{
      justify-content: space-between;
      .list{
        display: flex;
        ul{
          margin: 10px;
          li{
            list-style: none;
            color: white;
            text-transform: uppercase;
            a{
              text-decoration: none;
              color: rgb(116,119,115);
              font-size: .7rem;
            }
          }
        }
      }
      .footer-logo{
        background-image: url(../assets/img/dc-logo-bg.png);
        background-position: center;
        background-size: cover;
        height: 350px;
        width: 50%;
      }
    }
  }
  .footer-bottom {
    background-color: rgb(48,48,48);
    .my-container{
      justify-content: space-between;
      height: 80px;
      align-items: center;
      button{
        text-transform: uppercase;
        display: inline-block;
        font-weight: 400;
        line-height: 1.5;
        text-align: center;
        text-decoration: none;
        vertical-align: middle;
        cursor: pointer;
        background-color: transparent;
        border: 1px solid transparent;
        padding: 0.375rem 0.75rem;
        font-size: 1rem;
        color: white;
        border-color: $colorPrimary;
      }
      .social{
        color: $colorPrimary;
        display:flex;
        align-items: center;
        img{
          margin-left: 10px;
        }
      }
    }
  }
</style>
