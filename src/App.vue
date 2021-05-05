<template>
  <div id="app">
    <!-- HEADER -->
    <Header />

    <!-- MAIN -->
    <main>
      <Jumbotron/>
      <Slider />
      <Merchandising />

    </main>

    <!-- FOOTER -->
    <footer>
      <!-- Top Footer -->
      <TopFooter />

      <!-- Bottom Footer -->
      <BottomFooter />
    </footer>
    
  </div>
</template>

<script>
import Header from '@/components/Header.vue';
import Slider from '@/components/Slider.vue';
import Merchandising from '@/components/Merchandising.vue';
import TopFooter from '@/components/TopFooter.vue';
import BottomFooter from '@/components/BottomFooter.vue';
import Jumbotron from '@/components/Jumbotron.vue';


export default {
  name: 'App',
  components: {
    Header,
    Jumbotron,
    Slider,
    Merchandising,
    TopFooter,
    BottomFooter,
  }
}
</script>

<style lang="scss">
@import '@/styles/general.scss';
@import '@/styles/utilities';





</style>
