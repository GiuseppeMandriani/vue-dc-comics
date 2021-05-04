<template>
  <div id="app">
    <!-- HEADER -->
    <Header />

    <!-- MAIN -->
    <main>
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


export default {
  name: 'App',
  components: {
    Header,
    Slider,
    Merchandising,
    TopFooter,
    BottomFooter,
  }
}
</script>

<style lang="scss">
/* GENERAL */
*{
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}

body{
  font-family: sans-serif;
  font-size:14px;
  color: #000;
}
.container{
  max-width: 1200px;
  margin: 0 auto;
}

</style>
