<template>
  <div class="header">
    <div id="logo-img">
      <img src="../../img/dc-logo.png" alt="">
    </div>
    <ul>
      <li><a href="">item</a></li>
      <li><a href="">item</a></li>
      <li><a href="">item</a></li>
      <li><a href="">item</a></li>
      <li><a href="">item</a></li>
      <li><a href="">item</a></li>
      <li><a href="">item</a></li>
      <li><a href="">item</a></li>
      <li><a href="">item</a></li>
      <li><a href="">item</a></li>
    </ul>
  </div>
</template>

<script>
export default {
  name: 'homeHeader',
  
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
  .header{
    display: flex;
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
        a{
          text-decoration: none;
          color: black;
        }
      }
    }
  }
</style>
