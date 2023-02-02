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
              <li>
                <a href="#">Characters</a>
              </li>
              <li>
                <a href="#">Comics</a>
              </li>
              <li>
                <a href="#">Movie</a>
              </li>
              <li>
                <a href="#">Tv</a>
              </li>
              <li>
                <a href="#">Games</a>
              </li>
              <li>
                <a href="#">Videos</a>
              </li>
              <li>
                <a href="#">News</a>
              </li>
            </ul>

            <ul>
              <li>
                <h3>shop</h3>
              </li>
              <li>
                <a href="#">Shop DC</a>
              </li>
              <li>
                <a href="#">Shop DC Collectibles</a>
              </li>
            </ul>
          </div>

          <div class="links">
            <ul>
              <li>
                <h3>dc</h3>
              </li>
              <li>
                <a href="#">Terms Of Use</a>
              </li>
              <li>
                <a href="#">Privacy policy (New)</a>
              </li>
              <li>
                <a href="#">Ad Choice</a>
              </li>
              <li>
                <a href="#">Advertising</a>
              </li>
              <li>
                <a href="#">Jobs</a>
              </li>
              <li>
                <a href="#">Subscriptions</a>
              </li>
              <li>
                <a href="#">Talent Workshops</a>
              </li>
              <li>
                <a href="#">CPSC Certificates</a>
              </li>
              <li>
                <a href="#">Ratings</a>
              </li>
              <li>
                <a href="#">Shop Help</a>
              </li>
              <li>
                <a href="#">Contact Us</a>
              </li>
            </ul>
          </div>

          <div class="links">
            <ul>
              <li>
                <h3>sites</h3>
              </li>
              <li>
                <a href="#">DC</a>
              </li>
              <li>
                <a href="#">MAD Magazine</a>
              </li>
              <li>
                <a href="#">DC Kids</a>
              </li>
              <li>
                <a href="#">DC Universe</a>
              </li>
              <li>
                <a href="#">DC Power Visa</a>
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