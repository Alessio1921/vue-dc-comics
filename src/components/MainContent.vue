<template>
  <div class="content">
    <div class="main-top">
      <div class="my-container">
        <h2>--> Content goes here </h2>
      </div>
    </div>
    <div class="main-bottom">
      <div class="my-container">
        <img src="../../img/buy-comics-digital-comics.png" alt="">
        <p>digital comics</p>
        <img src="../../img/buy-comics-digital-comics.png" alt="">
        <p>digital comics</p>
        <img src="../../img/buy-comics-digital-comics.png" alt="">
        <p>digital comics</p>
        <img src="../../img/buy-comics-digital-comics.png" alt="">
        <p>digital comics</p>
        <img src="../../img/buy-comics-digital-comics.png" alt="">
        <p>digital comics</p>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'MainContent',
  
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
      .my-container{
        img{
          padding: 25px;
          height: 100%;
        }
      }
    }
  }
</style>
