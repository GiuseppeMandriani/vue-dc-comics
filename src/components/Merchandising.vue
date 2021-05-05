<template>
<section class="merchandising">
    <div class="container">
        <ul class="menu">
            <li class="card" v-for="(logo,index) in loghi" :key="index" >
                <a href="#"><img :src="logo.url" :alt="`${logo.text}`"></a>
                <a class="text" href="#">{{ logo.text}}</a>
            </li>
        </ul>
    </div>
</section>
  
</template>

<script>
export default {
    name: 'Merchandising',
    data(){
        return {
            loghi:[
                {
                    text: 'digital comics',
                    url:require ('../assets/img/buy-comics-digital-comics.png'),
                },
                {
                    text: 'dc merchandise',
                    url:require( '../assets/img/buy-comics-merchandise.png'),
                },
                {
                    text: 'subscription',
                    url:require( '../assets/img/buy-comics-digital-comics.png'),
                },
                {
                    text: 'comic shop locator',
                    url:require( '../assets/img/buy-comics-shop-locator.png'),
                },
                {
                    text: 'dc power visa',
                    url:require( '../assets/img/buy-dc-power-visa.svg'),
                },
            ]
        }
    }
}
</script>

<style lang="scss">
@import '@/styles/vars.scss';
@import '@/styles/mixins.scss';



.merchandising{
    background-color: $primary;
    height: 120px;
}

.menu{
    display: flex;
    list-style: none;
}

.menu img{
    width: 50px;
}

.menu .card{
    flex-basis: calc(100% / 5);
    padding: 20px 30px;

    @include center('vertical')

    /* display: flex;
    align-items: center; */
}

.menu .card a{
    text-transform: uppercase;
    /* padding: 1rem .5rem; */
    color: #fff;
    text-decoration: none;
    font-size:12px;
}
.menu .card a.text{
    margin-left:.5rem;
}

</style>