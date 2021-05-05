<template>
    <div class="bottom-footer">
        <div class="container">
            <div class="left">
                <button>sign-up now!</button>
            </div>
            <div class="right">
                <h4>follow us</h4>
                <nav>
                    <ul class="social-icons">
                        <li><a href="/"><img src="../assets/img/footer-facebook.png" alt="logo FB"></a></li>
                        <li><a href="/"><img src="../assets/img/footer-periscope.png" alt="logo FB"></a></li>
                        <li><a href="/"><img src="../assets/img/footer-pinterest.png" alt="logo FB"></a></li>
                        <li><a href="/"><img src="../assets/img/footer-twitter.png" alt="logo FB"></a></li>
                        <li><a href="/"><img src="../assets/img/footer-youtube.png" alt="logo FB"></a></li>
                    </ul>
                </nav>
                
                
            </div>

        </div>
    
    </div>
</template>

<script>
export default {
    name: 'BottomFooter'
}
</script>

<style scoped lang="scss">
@import '@/styles/vars.scss';
@import '@/styles/mixins.scss';


.bottom-footer{
    height: 100px;
    background-color:#303030;
}
.container{
    @include center('both');
    /* display: flex;
    justify-content: space-between;
    align-items: center; */
    justify-content: space-between;
    height: 100%;
}

.left button{
    min-width:150px;
    padding: 15px;
    text-transform: uppercase;
    background-color: transparent;
    outline: none;
    color: #fff;
    border: 1px solid $primary;
}

.right{

    @include center('vertical');
    /* display: flex;
    align-items: center; */

    h4{
        color: $primary;
        text-transform: uppercase;
        margin-right: 1rem;

    };

    ul.social-icons{
        display: flex;
        list-style: none;
        li{
            margin-right: 1rem;
            &:last-child{
                margin-right: 0;
            }

            img{
                cursor: pointer;
                
            }
        }

    }


}

</style>