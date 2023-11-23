<script>
  import Header from './components/AppHeader.vue';
  import Content from './components/AppContent.vue';
  import MainList from './components/AppMainList.vue';
  import Footer from './components/AppFooter.vue';

  export default {
    components: {
      Header,
      Content,
      MainList,
      Footer,
    }
  }
</script>

<template>
  <Header></Header>
  <Content></Content>
  <MainList></MainList>
  <Footer></Footer>
</template>

<style lang="scss">
@use "./style/general.scss";
</style>
