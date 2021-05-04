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
    
  </div>
</template>

<script>
import Header from '@/components/Header.vue';
import Slider from '@/components/Slider.vue';
import Merchandising from '@/components/Merchandising.vue';


export default {
  name: 'App',
  components: {
    Header,
    Slider,
    Merchandising,
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
}
.container{
  max-width: 1200px;
  margin: 0 auto;
}

</style>
