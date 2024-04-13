<template>
    <main>
        <div id="main-container">
            <section id="jumbotron">
                
            </section>
            <section class="centered-container">
              
                <div class=" d-flex justify-content-between align-content-center align-items-center flex-wrap">
                    <div class="single-card py-4 ps-4" v-for="(item, index) in comicCards" :key="index">
                    <CardComponent :image="item.thumb" :info2="item.series"/>
                    </div>
               </div>
            </section>
        </div>
        <section id="blue-content">
            <div class="centered-container d-flex justify-content-between align-items-center align-content-center">
                <div class="blue-wrapper">
                    <ul class="d-flex justify-content-between align-items-center align-content-center ps-3 flex-wrap">
                    <li v-for="(item, index) in menu" :key="index" class="py-5"><a class="text-uppercase" :href="item.url"> <img :class="{ myimg: isActive }" :src="item.img" :alt="item.title"> {{ item.title }}</a></li>
                </ul>
                </div>
                </div>
        </section>
    </main>
</template>

<script>
    import {comics} from '../data/store.js';
    import CardComponent from './CardComponent.vue';
    export default {
        name: 'MainComponent',
        components: {
            CardComponent
        },
        data(){
            return{
                menu: [
                    {
                        img: "/images/buy-comics-digital-comics.png",
                        title: 'digital comics',
                        url: '#'
                    },

                    {
                        img: "/images/buy-comics-merchandise.png",
                        title: 'dc merchandise',
                        url: '#'
                    },

                    {
                        img: "/images/buy-comics-subscriptions.png",
                        title: 'subscriptions',
                        url: '#'
                    },

                    {
                        img: "/images/buy-comics-shop-locator.png",
                        title: 'comic shop locator',
                        url: '#'
                    },

                    {
                        img: "/images/buy-dc-power-visa.svg",
                        title: 'dc power visa',
                        url: '#'
                    }
                ],
                isActive: true,
                comicCards: comics,
            }
        }
    }
</script>

<style lang="scss" scoped>
    @use '../assets/styles/partials/variables' as *;

    main{
        width: 100%;
        color: $white;
        font-size: 1.2em;
    
   #main-container{ 
        background-color: $black;
        
    }

    .centered-container{
        margin: 0 auto;
        max-width: 1200px;
    }

    #blue-content{
        background-color: $bluemain;
    }

    a{
        text-decoration: none;
        color: $white;
        font-size: 0.8em;
    }

    ul{
        list-style: none;

    li{
        width: calc(100% / 5);

       }
    }
    .myimg{
        width: 20%;
    } 

    #jumbotron{
        background-image: url("./src/assets/img/jumbotron.jpg");
        width: 100%;
        height: 450px;
        background-size: cover;
    }

    .single-card{
        width: calc(100% / 6);
        cursor: pointer;
    }
    }
</style>