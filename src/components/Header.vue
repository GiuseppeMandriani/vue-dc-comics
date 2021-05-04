<template>
<header>
    <div class="container">
        <!-- Logo -->
        <img class="logo" src="../assets/img/dc-logo.png" alt="Logo DC">

        <!-- Nav Bar -->
        <nav>
            <ul class="nav-menu">
                <li v-for="(link,index) in links" :key="index">
                    <a href="">{{ link.text }}</a>
                </li>
            </ul>
        </nav>

    </div>
</header>
  
</template>

<script>
export default {
    // Componente
    name: 'Header',

    // Data come funzione
        data() {
       return {
           links: [
               { 
                    text: "characters",
                    url: "/characters",
                    current: false
                },
               { 
                   text: "comics", 
                   url: "/comics", 
                   current: true
                },
               { 
                   text: "movies", 
                   url: "/movies", 
                   current: false
                },
               { 
                   text: "tv", 
                   url: "/tv", 
                   current: false
                },
               { 
                   text: "games", 
                   url: "/games", 
                   current: false
                },
               { 
                   text: "collectilbles", 
                   url: "/collectibles", 
                   current: false
                },
               { 
                   text: "videos", 
                   url: "/videos", 
                   current: false
                },
               { 
                   text: "fans", 
                   url: "/fans", 
                   current: false
                },
               { 
                   text: "news", 
                   url: "/news", 
                   current: false
               },
               { 
                   text: "shop", 
                   url: "/shop", 
                   current: false
                },
           ],
       }
    }
}


</script>

<style scoped>
.container{
    padding: 30px 0;
    display: flex;
    justify-content: space-between;
    align-items: center;
    height: 100px;
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
.nav-menu li:active{
    border-bottom: 2px solid dodgerblue;

}
</style>