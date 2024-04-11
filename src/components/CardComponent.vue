<template>
   <!--  <div class="container-fluid">
        <div class="row">
            <div class="col-sm-12 col-md-3 col-lg-6 py-5"> -->
                    <img class="cardimage" :src="image" :alt="info2">
                    <h5 class="card-title text-uppercase ">{{info2}}</h5>   
          <!--   </div>
        </div>
    </div> -->
</template>

<script>
    export default {
        name: 'CardComponent',
        props: ['image', 'info1', 'info2', 'info3' ]
    }
</script>

<style lang="scss" scoped>

/* .single-card{
        width: calc(100% / 6);
    } */

    .cardimage{
        width: 150px;
        height: 150px;
        display: block;
        
    }

    h5{
        font-size: 10px;

    }
</style>