<script>
export default {
  name: 'HeaderFooterBar',
  
  data() {
  
    return {
  
    }
  }
}
</script>

<template>

  <header>

    <div class="header-footer-container">

      <nav>
        <ul>
          <li>
            <a href="#">
              <img class="my-img" src="../assets/img/buy-comics-digital-comics.png" alt="">
              <span>digital comics</span>
            </a>
          </li>
          <li>
            <a href="#">
              <img class="my-img" src="../assets/img/buy-comics-merchandise.png" alt="">
              <span>dc merchandise</span>
            </a>
          </li>
          <li>
            <a href="#">
              <img class="my-img" src="../assets/img/buy-comics-subscriptions.png" alt="">
              <span>subscription</span>
            </a>
          </li>
          <li>
            <a href="#">
              <img id="img-min" src="../assets/img/buy-comics-shop-locator.png" alt="">
              <span>comics shop locator</span>
            </a>
          </li>
          <li>
            <a href="#">
              <img class="my-img" src="../assets/img/buy-dc-power-visa.svg" alt="">
              <span>dc power visa</span>
            </a>
          </li>
        </ul>
      </nav>

    </div>

  </header>
    
</template>

<style lang="scss" scoped>
header {
  height: 130px;
  background-color: #0383f9;
  .header-footer-container {
    width: 80%;
    height: 100%;
    margin: 0 auto;
    nav {
      height: 100%;
      ul {
        height: 100%;
        list-style: none;
        display: flex;
        li {
          width: calc(100% / 5);
          a {
            text-decoration: none;
            width: 100%;
            height: 100%;
            color: #ddeffe;
            display: flex;
            align-items: center;
            justify-content: center;
            .my-img {
              width: 15%;
              margin-right: 15px;
            }
            #img-min {
              width: 10%;
              margin-right: 15px;
            }
            span {
              text-transform: uppercase; 
              font-size: 12px;
            }
          }
        }
      }
    }
  }
}
</style>