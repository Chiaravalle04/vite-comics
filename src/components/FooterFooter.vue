<script>
export default {
  name: 'FooterFooter',
  
  data() {
  
    return {
  
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
                    <li>
                        <a href="#">
                            <img src="../assets/img/footer-facebook.png" alt="">
                        </a>
                    </li>
                    <li>
                        <a href="#">
                            <img src="../assets/img/footer-twitter.png" alt="">
                        </a>
                    </li>
                    <li>
                        <a href="#">
                            <img src="../assets/img/footer-youtube.png" alt="">
                        </a>
                    </li>
                    <li>
                        <a href="#">
                            <img src="../assets/img/footer-pinterest.png" alt="">
                        </a>
                    </li>
                    <li>
                        <a href="#">
                            <img src="../assets/img/footer-periscope.png" alt="">
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