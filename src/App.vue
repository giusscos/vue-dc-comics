<template>
  <div id="app">
    <MainHeader />
    <MainContent />
    <MainFooterB />
    <!-- <MainFooter /> -->
  </div>
</template>

<script>
import MainHeader from './components/MainHeader.vue';
import MainContent from './components/MainContent.vue';
// import MainFooter from './components/MainFooter.vue'; Tutte le nuove aggiunte riguardo al Footer sono state fatte nella cartella Bonus 
import MainFooterB from './bonus/components/MainFooterB.vue';


export default {
  name: 'App',
  components: {
    MainHeader,
    MainContent,
    // MainFooter,
    MainFooterB
  }
}
</script>

<style lang="scss">
@import '@/style/index.scss';

#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
}
</style>
