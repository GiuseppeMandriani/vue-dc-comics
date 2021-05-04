<template>
<section class="merchandising">
    <div class="container">
        <ul class="menu">
            <li class="card" v-for="(logo,index) in loghi" :key="index" >
                <a href="#"><img src="'../assets/img/buy- +' logo.url" :alt="`${logo.text}`"></a>
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
                    url: 'comics-digital-comics.png'
                },
                {
                    text: 'dc merchandise',
                    url: 'comics-merchandise.png'
                },
                {
                    text: 'subscription',
                    url: 'comics-digital-comics.png'
                },
                {
                    text: 'comic shop locator',
                    url: 'comics-shop-locator.png'
                },
                {
                    text: 'dc power visa',
                    url: 'dc-power-visa.png'
                },
            ]
        }
    }
}
</script>

<style scoped>

.merchandising{
    background-color: #0282f9;
    height: 120px;
}

.menu{
    display: flex;
    list-style: none;
}

.menu img{
    max-width: 50px;
}

.menu .card{
    flex-basis: calc(100% / 5);
    padding: 20px 30px;
    display: flex;
    align-items: center;
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