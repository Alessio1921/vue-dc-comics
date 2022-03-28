<template>
  <div class="footer">
    <div class="footer-top">
      <div class="my-container">
        <div class="list">
          <div class="list-left">
            <ul>
              <li>
                <a href="">title</a>
              </li>
              <li>
                <a href="">item</a>
              </li>
              <li>
                <a href="">item</a>
              </li>
              <li>
                <a href="">item</a>
              </li>
              <li>
                <a href="">item</a>
              </li>
              <li>
                <a href="">item</a>
              </li>
              <li>
                <a href="">item</a>
              </li>
              <li>
                <a href="">item</a>
              </li>
            </ul>
            <ul>
              <li>
                <a href="">title</a>
              </li>
              <li>
                <a href="">item</a>
              </li>
              <li>
                <a href="">item</a>
              </li>
            </ul>
          </div>
          
          <ul>
            <li>
              <a href="">title</a>
            </li>
            <li>
              <a href="">item</a>
            </li>
            <li>
              <a href="">item</a>
            </li>
            <li>
              <a href="">item</a>
            </li>
            <li>
              <a href="">item</a>
            </li>
            <li>
              <a href="">item</a>
            </li>
            <li>
              <a href="">item</a>
            </li>
            <li>
              <a href="">item</a>
            </li>
            <li>
              <a href="">item</a>
            </li>
            <li>
              <a href="">item</a>
            </li>
            <li>
              <a href="">item</a>
            </li>
            <li>
              <a href="">item</a>
            </li>
          </ul>

          <ul>
            <li>
              <a href="">title</a>
            </li>
            <li>
              <a href="">item</a>
            </li>
            <li>
              <a href="">item</a>
            </li><li>
              <a href="">item</a>
            </li>
            <li>
              <a href="">item</a>
            </li><li>
              <a href="">item</a>
            </li>
          </ul>
        </div>
        <div class="footer-logo">
        </div>
      </div>
    </div>
    <div class="footer-bottom">
      <div class="my-container">
        <button>sign up now</button>
        <div class="social">
          <h3>follow us</h3>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'homeFooter',
  
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
  .my-container{
    display: flex;
    justify-content: space-between;
  }
  .footer-top{
    background-image: url(../../img/footer-bg.jpg);
    height: 350px;
    .my-container{
      .list{
        display: flex;
        ul{
          margin: 10px;
        }
      }
      .footer-logo{
        background-image: url(../../img/dc-logo-bg.png);
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
      height: 80px;
      align-items: center;
      button{
        text-transform: uppercase;
        height: 20px;
      }
      .social{
        color: blue;
      }
    }
  }
</style>
