<script>
export default {
  name: 'AppHeader',
  
  data() {
  
    return {
  
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
                    <li>
                        <a href="#">characters</a>
                    </li>
                    <li>
                        <a href="#">comics</a>
                    </li>
                    <li>
                        <a href="#">movies</a>
                    </li>
                    <li>
                        <a href="#">tv</a>
                    </li>
                    <li>
                        <a href="#">games</a>
                    </li>
                    <li>
                        <a href="#">collectibles</a>
                    </li>
                    <li>
                        <a href="#">videos</a>
                    </li>
                    <li>
                        <a href="#">fans</a>
                    </li>
                    <li>
                        <a href="#">news</a>
                    </li>
                    <li>
                        <a href="#">shop</a>
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