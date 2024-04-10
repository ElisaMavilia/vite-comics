<template>
    <header>
        <div id="header-container"  class="container">
            <div id="left-navbar">
                <img src="../assets/img/dc-logo.png" alt="Logo">
            </div>
            <div id="rigth-navbar">
                <ul>
                    <li v-for="(item, index) in navbar" :key="index"><a href="item.url"></a>{{ item.name }}</li>
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

header{
    width: 100%;

    #header-container{
        margin: 0 auto;
        border: 1px solid red;
    }
  
}

</style>