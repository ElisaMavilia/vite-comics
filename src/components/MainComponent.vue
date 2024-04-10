<template>
    <main id="main-container">
        <div class="container">
        --> Content goes here <--
        
        </div>
    </main>
</template>

<script>
    export default {
        name: 'MainComponent',
        data(){
            return{

            }
        }
    }
</script>

<style lang="scss" scoped>
    @use '../assets/styles/partials/variables' as *;

    main{
        width: 100%;
        background-color: $black;
        color: $white;
        padding: 50px;
        font-size: 1.5em;
    
    #main-container{
        margin: 0 auto;
        border: 1px solid red;
       
    }
    }
</style>