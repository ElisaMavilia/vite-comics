<template>
  <HeaderComponent />
  <MainComponent />
  <CardComponent />
  <FooterUpComponent />
</template>

<script>
  import HeaderComponent from './components/HeaderComponent.vue';
  import MainComponent from './components/MainComponent.vue';
  import CardComponent from './components/CardComponent.vue';
  import FooterUpComponent from './components/FooterUpComponent.vue';
  export default {
    name: 'App',
    components: {
      HeaderComponent,
      MainComponent,
      CardComponent,
      FooterUpComponent

  }
}
</script>

<style lang="scss" scoped>

</style>