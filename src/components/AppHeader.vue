<script>
export default {
  name: 'AppHeader',
  
  data() {
  
    return {

        navHeader: [
            'characters',
            'comics',
            'movies',
            'tv',
            'games',
            'collectibles',
            'videos',
            'fans',
            'news',
            'shop'
        ]
  
    }
  }
}
</script>

<template>

    <header>

        <div class="general-container d-flex jc-space-bet">

            <div class="header-logo">
                <a href="#">
                    <img src="../assets/img/dc-logo.png" alt="">
                </a>
            </div>

            <div class="nav-bar d-flex ai-center">
                <ul class="d-flex">
                    <li v-for="item in navHeader">
                        <a href="#">{{ item }}</a>
                    </li>
                </ul>
            </div>

        </div>

    </header>
    
</template>

<style lang="scss" scoped>
header {
    height: 100px;
    background-color: #fff;
    .general-container {
        .header-logo {
            width: 100px;
            padding: 10px;
            img {
                width: 100%;
            }
        }  
        .nav-bar {
            height: 100%;
            ul {
                li {
                    a {
                        text-transform: uppercase;
                        font-size: 10px;
                        padding: 38px 10px;
                        color: black;
                        font-weight: bold;
                        &:hover {
                            border-bottom: 4px solid #0383f9;
                            color: #0383f9;
                        }
                    }
                }
            }
        }
    }
}
</style>