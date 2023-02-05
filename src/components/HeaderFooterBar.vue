<script>
import digital from "../assets/img/buy-comics-digital-comics.png";
import merchandise from "../assets/img/buy-comics-merchandise.png";
import subscriptions from "../assets/img/buy-comics-subscriptions.png";
import shop from "../assets/img/buy-comics-shop-locator.png";
import visa from "../assets/img/buy-dc-power-visa.svg";

export default {
  name: 'HeaderFooterBar',
  
  data() {
  
    return {
      itemHeaderBar: [
        {
          src: digital,
          url: '#',
          title: 'digital comics',
          smallImg: false
        },
        {
          src: merchandise,
          url: '#',
          title: 'dc merchandise',
          smallImg: false
        },
        {
          src: subscriptions,
          url: '#',
          title: 'subscription',
          smallImg: false
        },
        {
          src: shop,
          url: '#',
          title: 'comics shop locator',
          smallImg: true
        },
        {
          src: visa,
          url: '#',
          title: 'dc power visa',
          smallImg: false
        }
      ]
      
    }
  },
}
</script>

<template>

  <header>

    <div class="general-container">

      <nav>
        <ul class="d-flex">
          <li v-for="item in itemHeaderBar">
            <a class="d-flex jc-center ai-center" :href="item.url">
              <img :class="{'my-img': item.smallImg == false, 'img-min': item.smallImg == true}" :src="item.src" alt="">
              <span>{{ item.title }}</span>
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
  .general-container {
    nav {
      height: 100%;
      ul {
        height: 100%;
        li {
          width: calc(100% / 5);
          a {
            width: 100%;
            height: 100%;
            color: #ddeffe;
            .my-img {
              width: 15%;
              margin-right: 15px;
            }
            .img-min {
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