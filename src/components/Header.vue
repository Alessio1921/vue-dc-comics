<template>
  <div class="header">
    <div class="my-container">
      <div id="logo-img">
        <img src="../assets/img/dc-logo.png" alt="">
      </div>
      <nav>
        <ul>
          <li v-for="(item,index) in listNav" :key="index" :class="{active:item.active}"><a :class="{active:item.active}" :href="item.url">{{item.name}}</a></li>
        </ul>
      </nav>
    </div>
  </div>
</template>

<script>
export default {
  name: 'homeHeader',
  data: function(){
  return {
    listNav:[
      {
        name:"characters",
        active:false,
        url:"#"
      },
      {
        name:"comics",
        active:true,
        url:"#"
      },
      {
        name:"movies",
        active:false,
        url:"#"
      },
      {
        name:"games",
        active:false,
        url:"#"
      },
      {
        name:"collectibles",
        active:false,
        url:"#"
      },
      {
        name:"videos",
        active:false,
        url:"#"
      },
      {
        name:"fans",
        active:false,
        url:"#"
      },
      {
        name:"news",
        active:false,
        url:"#"
      },
      {
        name:"shop",
        active:false,
        url:"#"
      }
    ]
  }
}
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
@import "../assets/scss/style.scss";
  .header .my-container{
    justify-content:space-between;
    align-items: center;
    #logo-img{
      height: 70px;
      margin: .8rem 0;
      img{
        height: 100%;
      }
    }
    ul{
      display: flex;
      li{
        list-style: none;
        margin: 0 .7rem;
        .active{
          border-bottom: 4px solid $colorPrimary;
          color: $colorPrimary;
          padding-bottom:33px ;
        }
        a{
          text-decoration: none;
          color: black;
        }
      }
    }
  }

</style>
