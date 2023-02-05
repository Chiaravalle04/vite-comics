<script>
import HeaderFooterBar from './HeaderFooterBar.vue';
import FooterFooter from './FooterFooter.vue'

export default {
  name: 'AppFooter',

  components: {
    HeaderFooterBar,
    FooterFooter,
  },
  
  data() {
  
    return {

      dcComics: [
        {
          url: '#',
          title: 'Characters'
        },
        {
          url: '#',
          title: 'Comics'
        },
        {
          url: '#',
          title: 'Movie'
        },
        {
          url: '#',
          title: 'Tv'
        },
        {
          url: '#',
          title: 'Games'
        },
        {
          url: '#',
          title: 'Videos'
        },
        {
          url: '#',
          title: 'News'
        },
      ],

      shop: [
        {
          url: '#',
          title: 'Shop DC'
        },
        {
          url: '#',
          title: 'Shop DC Collectibles'
        },
      ],

      dc: [
        {
          url: '#',
          title: 'Terms Of Use'
        },
        {
          url: '#',
          title: 'Privacy policy (New)'
        },
        {
          url: '#',
          title: 'Ad Choice'
        },
        {
          url: '#',
          title: 'Advertising'
        },
        {
          url: '#',
          title: 'Jobs'
        },
        {
          url: '#',
          title: 'Subscriptions'
        },
        {
          url: '#',
          title: 'Talent Workshops'
        },
        {
          url: '#',
          title: 'CPSC Certificates'
        },
        {
          url: '#',
          title: 'Ratings'
        },
        {
          url: '#',
          title: 'Shop Help'
        },
        {
          url: '#',
          title: 'Contact Us'
        },
      ],

      sites: [
        {
          url: '#',
          title: 'DC'
        },
        {
          url: '#',
          title: 'MAD Magazine'
        },
        {
          url: '#',
          title: 'DC Kids'
        },
        {
          url: '#',
          title: 'DC Universe'
        },
        {
          url: '#',
          title: 'DC Power Visa'
        },
      ]
  
    }
  }
}
</script>

<template>

  <footer>

    <HeaderFooterBar/>

    <main>

      <div class="general-container">

        <nav>

          <div class="links">
            <ul>
              <li>
                <h3>dc comics</h3>
              </li>
              <li v-for="item in dcComics">
                <a :href="item.url">{{ item.title }}</a>
              </li>
            </ul>

            <ul>
              <li>
                <h3>shop</h3>
              </li>
              <li v-for="item in shop">
                <a :href="item.url">{{ item.title }}</a>
              </li>
            </ul>
          </div>

          <div class="links">
            <ul>
              <li>
                <h3>dc</h3>
              </li>
              <li v-for="item in dc">
                <a :href="item.url">{{ item.title }}</a>
              </li>
            </ul>
          </div>

          <div class="links">
            <ul>
              <li>
                <h3>sites</h3>
              </li>
              <li v-for="item in sites">
                <a :href="item.url">{{ item.title }}</a>
              </li>
            </ul>
          </div>

        </nav>

        <div class="img-bg">

        </div>

      </div>

    </main>

    <FooterFooter/>

  </footer>

</template>

<style lang="scss" scoped>
main {
  height: 350px;
  background-image: url('../assets/img/footer-bg.jpg');
  background-size: cover;
  .general-container {
    display: flex;
    justify-content: space-between;
    nav {
      display: flex;
      ul {
        list-style: none;
      }
      .links {
        padding: 30px 30px 30px 0;
        h3 {
          text-transform: uppercase;
          color: #eef1fc;
          margin: 15px 0;
        }
        a {
          text-decoration: none;
          color: #808c8a;
          font-size: 13px;
          &:hover {
            text-decoration: underline;
          }
        }
      }
    }
    .img-bg {
      width: 50%;
      height: 100%;
      background-image: url('../assets/img/dc-logo-bg.png');
      background-position: center;
      background-repeat: no-repeat;
    }
  }
}
</style>