<template>
    <header>
        <div id="header-container"  class="container">
            <img src="../assets/img/dc-logo.png" alt="Logo">
        </div>
        
    </header>
</template>

<script>
    export default {
        name: 'HeaderComponent',
        data(){
            return{

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