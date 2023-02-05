<script>
export default {
  name: 'AppHeader',
  
  data() {
  
    return {

        navHeader: [
            {
                label: 'characters',
                url: '#',
                active: false,
            },
            {
                label: 'comics',
                url: '#',
                active: true,
            },
            {
                label: 'movies',
                url: '#',
                active: false,
            },
            {
                label: 'tv',
                url: '#',
                active: false,
            },
            {
                label: 'games',
                url: '#',
                active: false,
            },
            {
                label: 'collectibles',
                url: '#',
                active: false,
            },
            {
                label: 'videos',
                url: '#',
                active: false,
            },
            {
                label: 'fans',
                url: '#',
                active: false,
            },
            {
                label: 'news',
                url: '#',
                active: false,
            },
            {
                label: 'shop',
                url: '#',
                active: false,
            },
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
                        <a :href="item.url" :class="{'active': item.active == true}">{{ item.label }}</a>
                    </li>
                </ul>
            </div>

        </div>

    </header>
    
</template>

<style lang="scss" scoped>
@use '../styles/partials/varcolor.scss' as *;

header {
    height: 100px;
    background-color: $secondColor;
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
                        color: $thirdColor;
                        font-weight: bold;
                        &.active {
                            border-bottom: 4px solid $mainColor;
                            color: $mainColor;
                        }
                    }
                }
            }
        }
    }
}
</style>