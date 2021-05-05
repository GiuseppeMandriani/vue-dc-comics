<template>
          <div class="box">
              <img :src="series.thumb" :alt="series.series">
              <span class="title">{{ series.series }}</span>

          </div>

</template>

<script>
export default {
    name: 'Card',
    // props: ['series'] // METODO 1
    props:{
        series: Object,     // METODO 2 Passo il tipo se oggetto array string number
    }
}
</script>

<style scoped lang="scss">
.box{
    flex-basis: calc(100% / 6 - 2rem);
    height: 190px;
    margin: 1.8rem 1rem;
    /* overflow: hidden; */
    position: relative;
    /* padding: 5px; */
    
    img{
        display: block;
        width: 100%;
        height: 100%;
        object-fit:center;

    }
    .title{
        color: #fff;
        position: absolute;
        top: 105%;
        text-transform: uppercase;

    }
}

</style>