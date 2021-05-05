<template>
<header>
    <div class="container">
        <!-- Logo -->
        <img class="logo" src="../assets/img/dc-logo.png" alt="Logo DC">

        <!-- Nav Bar -->
        <nav>
            <ul class="nav-menu">
                <li v-for="(link,index) in links" :key="index" :class="{active: index == indexLink}">
                    <a href="">{{ link.text }}</a>
                </li>
            </ul>
        </nav>

    </div>
</header>
  
</template>

<script>
import seriesData from '@/data/seriesData.js'

export default {
    // Componente
    name: 'Header',

    // Data come funzione
        data() {
       return {
           indexLink: 0,
           links: seriesData,
       }
    }
}


</script>

<style lang="scss" scoped>
@import '@/styles/vars.scss';
@import '@/styles/mixins.scss';

header{
    background-color: #fff;

}
.container{
    padding: 0 30px;

    @include center('both');

    /* display: flex;
    justify-content: space-between;
    align-items: center; */
    justify-content: space-between;
    height: 100px;
    background-color: #fff;
}

/* Logo */
.logo{
    max-width: 80px;
}

.nav-menu{
    display: flex;
    list-style: none;


}
.nav-menu li{
    height: 100%;
    border-bottom: 2px solid transparent;
    
}

.nav-menu li a{
    /* margin-right: 1rem; */
    padding: 1rem;
    line-height:100px;
    text-transform: uppercase;
    text-decoration: none;
    color: #1c1c1c;
    font-size:12px;
    transition: .3s;
}

.nav-menu li:hover,
.nav-menu li.active{
    border-bottom: 3px solid $primary;
}
</style>