<template>
<section class="TopFooter">
    <div class="container">
        <div class="list">
            <h3>dc comics</h3>
            
            <ul>
                <li v-for="(element,index) in dsComics" :key="index"><a href="#">{{ element.text}}</a></li>
            </ul>

            <h3>shop</h3>

            <ul>
                <li v-for="(element,index) in shop" :key="index"><a href="#">{{ element.text}}</a></li>
            </ul>

        </div>
        <div class="list">
            <h3>dc</h3>

            <ul>
                <li v-for="(element,index) in dc" :key="index"><a href="#">{{ element.text}}</a></li>
            </ul>


        </div>
        <div class="list">
            <h3>sites</h3>

            <ul>
                <li v-for="(element,index) in sites" :key="index"><a href="#">{{ element.text}}</a></li>
            </ul>


        </div>
    </div>

        <div class="logo-bg">
            <img src="../assets/img/dc-logo-bg.png" alt="logo-bg">
        </div>




</section>
  
</template>

<script>
export default {
    name: 'TopFooter',
    data(){
        return {
            dsComics: [
                {text: "characters"},
                {text: "comics"},
                {text: "movies"},
                {text: "tv"},
                {text: "games"},
                {text: "videos"},
                {text: "news"},
            ],
            shop: [
                {text: "Shop DC"},
                {text: "Shop DC Collectibles"},
            ],
            dc: [
                {text: "terms Of Use"},
                {text: "Privacy policy (New)"},
                {text: "Ad Choise"},
                {text: "Jobs"},
                {text: "subscriptions"},
                {text: "Talent Workshops"},
                {text: "CPSC Certificates"},
                {text: "Ratings"},
                {text: "Shop Help"},
                {text: "Contact Us"},
            ],
            sites: [
                 {text: "DC"},
                 {text: "MAD Magazine"},
                 {text: "DC Kids"},
                 {text: "DC Universe"},
                 {text: "DC Power Visa"},
            ],
        }
    }

}
</script>

<style scoped>
.TopFooter{
    position: relative;
    background-image: url(../assets/img/footer-bg.jpg); 
    background-size: cover;
    height: 300px;
    padding: 30px 0;
}
.container{
    display: flex;
    padding: 30px 0;
}

.list{
    margin-right: 20px;
}
h3{
    color: #fff;
    text-transform: uppercase;
    /* margin: 1rem 0; */
}

ul{
    list-style: none;
    margin-bottom: 1rem;
}

a{
  color: #ccc;
  text-decoration: none;
  text-transform: capitalize;
  font-size: 11px;
  transition: .3s;
}
a:hover{
    color:#fff;
}

/* LOGO BG */
.logo-bg{
    width: 530px;
    height: 400px;
    position: absolute;
    overflow: hidden;
    top: -15%;
    right: 5%;
}

.logo-bg img{
    width:320px;
}


</style>