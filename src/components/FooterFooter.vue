<script>
import facebook from '../assets/img/footer-facebook.png';
import twitter from '../assets/img/footer-twitter.png';
import youtube from '../assets/img/footer-youtube.png';
import pinterest from '../assets/img/footer-pinterest.png';
import periscope from '../assets/img/footer-periscope.png';

export default {
  name: 'FooterFooter',
  
  data() {
  
    return {

        images: [
            {
                url: '#', 
                src: facebook 
            },
            { 
                url: '#', 
                src: twitter 
            },
            {
                url: '#', 
                src: youtube 
            },
            { 
                url: '#', 
                src: pinterest 
            },
            { 
                url: '#', 
                src: periscope
            }
      ]
    }
  }
}
</script>

<template>

    <footer>

        <div class="general-container d-flex ai-center jc-space-bet">

            <div class="btn-sign">
                <button>sign-up now!</button>
            </div>

            <nav>
                <ul class="d-flex ai-center">
                    <li>
                        <h3>FOLLOW US</h3> 
                    </li>
                    <li v-for="item in images">
                        <a :href="item.url">
                            <img :src="item.src" alt="">
                        </a>
                    </li>
                </ul>
            </nav>

        </div>
    
    </footer>
    
</template>

<style lang="scss" scoped>
footer {
    height: 100px;
    background-color: #303131;
    .general-container{
        .btn-sign {
            button {
                display: inline-block;
                padding: 15px;
                border: 2px solid #0383f8;
                background: none;
                text-transform: uppercase;
                color: #fff;
                font-weight: bold;
                cursor: pointer;
            }
        }
        nav {
            height: 100%;
            ul {
                height: 100%;
                h3 {
                    color: #0383f8;
                    margin-right: 10px;
                }
                a {
                    margin-left: 10px;
                }
            }
        }
    }
}
</style>