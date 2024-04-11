<template>
  <HeaderComponent />
  <MainComponent />
  <CardComponent />
</template>

<script>
  import HeaderComponent from './components/HeaderComponent.vue';
  import MainComponent from './components/MainComponent.vue';
  import CardComponent from './components/CardComponent.vue';
  export default {
    name: 'App',
    components: {
      HeaderComponent,
      MainComponent,
      CardComponent

  }
}
</script>

<style lang="scss" scoped>

</style>