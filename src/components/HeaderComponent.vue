<template>
    <header>
        <div id="header-container"  class="container d-flex align-content-center align-items-center">
            <div id="left-navbar">
                <img src="../assets/img/dc-logo.png" alt="Logo">
            </div>
            <div id="rigth-navbar">
                <ul class="d-flex justify-content-between">
                    <li v-for="(item, index) in navbar" :key="index"><a class="text-uppercase" href="item.url">{{ item.name }}</a></li>
                </ul>

            </div>
            
        </div>
        
    </header>
</template>

<script>
    export default {
        name: 'HeaderComponent',
        data(){
            return{
                navbar: [
                    {
                        name: 'charachters',
                        url: '#'
                    },
                    {
                        name: 'comics',
                        url: '#'
                    },
                    {
                        name: 'movies',
                        url: '#'
                    },
                    {
                        name: 'tv',
                        url: '#'
                    },
                    {
                        name: 'games',
                        url: '#'
                    },
                    {
                        name: 'collectibles',
                        url: '#'
                    },
                    {
                        name: 'videos',
                        url: '#'
                    },
                    {
                        name: 'fans',
                        url: '#'
                    },
                    {
                        name: 'news',
                        url: '#'
                    },
                    {
                        name: 'shop',
                        url: '#'
                    },
                ]

            }
        }
    }
</script>

<style lang="scss" scoped>
@use '../assets/styles/partials/variables' as *;

header{
    width: 100%;
   

    #header-container{
        margin: 0 auto;
        border: 1px solid red;
        display: flex;
        height: 90px

    }

    #left-navbar{
        width: 30%;

    img{
        width: 25%;
    }
    }

    #rigth-navbar{
        width: 70%;
    }

    ul{
        list-style: none;
    }

    a{
        text-decoration: none;
        color: $black;
        font-size: 0.8em;

        &:hover{
            color: $bluemain;
            border-bottom: 4px solid $bluemain;
            padding-bottom: 45px;
        }
    }
}
</style>