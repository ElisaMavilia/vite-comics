<template>
    <div>
        <img :src="image" :alt="info2">
        
        <h5 class="card-title">{{info2}}</h5>
        
</div>
  
</template>

<script>
    export default {
        name: 'CardComponent',
        props: ['image', 'info1', 'info2', 'info3' ]
    }
</script>

<style lang="scss" scoped>

</style>