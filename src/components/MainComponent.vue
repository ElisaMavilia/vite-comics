<template>
    <main>
        <section id="main-container">
            <div class="centered-container">
                --> Content goes here <--
            </div>
        </section>
        <section id="blue-content">
            <div class="centered-container">
                <ul class="d-flex justify-content-between align-items-center ">
                    <li v-for="(item, index) in menu" :key="index" class="pt-2"><a class="text-uppercase" href="item.url"><img :src="item.img" alt=""> {{ item.object }}</a></li>
                </ul></div>
        </section>
    </main>
</template>

<script>
    export default {
        name: 'MainComponent',
        data(){
            return{
                menu: [
                    {
                        img: "../src/assets/img/buy-comics-digital-comics.png",
                        object: 'digital comics',
                        url: '#'
                    },

                    {
                        img: "../src/assets/img/buy-comics-merchandise.png",
                        object: 'dc merchandise',
                        url: '#'
                    },

                    {
                        img: "../src/assets/img/buy-comics-subscriptions.png",
                        object: 'subscriptions',
                        url: '#'
                    },

                    {
                        img: "../src/assets/img/buy-comics-shop-locator.png",
                        object: 'comic shop ocator',
                        url: '#'
                    },

                    {
                        img: "../src/assets/img/buy-dc-power-visa.svg",
                        object: 'dc power visa',
                        url: '#'
                    }
                ]
            }
        }
    }
</script>

<style lang="scss" scoped>
    @use '../assets/styles/partials/variables' as *;

    main{
        width: 100%;
        color: $white;
        font-size: 1.5em;
    
   #main-container{ 
        background-color: $black;
    }

    .centered-container{
        margin: 0 auto;
        border: 1px solid red;
        max-width: 1300px;
        }

    #blue-content{
        width: 100%;
        background-color: $bluemain;
    }
    a{
        text-decoration: none;
        color: $white;
        font-size: 0.8em;
    }

    ul{
        list-style: none;
    }

    img{
        width: 12%;
    } 

    }
</style>