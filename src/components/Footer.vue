<template>
    <footer>
        <section class="container display-flex">
            <div class="info display-flex">
                <div class="links">
                    <h3>DC COMICS</h3>
                    <ul>
                        <li><a href="#">characters</a></li>
                        <li><a href="#">comics</a></li>
                        <li><a href="#">movies</a></li>
                        <li><a href="#">tv</a></li>
                        <li><a href="#">games</a></li>
                        <li><a href="#">videos</a></li>
                        <li><a href="#">news</a></li>
                    </ul>
                    <h3>SHOP</h3>
                    <ul>
                        <li><a href="#">shop DC</a></li>
                        <li><a href="#">shop DC collectibles</a></li>
                    </ul>
                </div>
                <div class="links">
                    <h3>DC</h3>
                    <ul>
                        <li><a href="#">terms of use</a></li>
                        <li><a href="#">privacy policy</a></li>
                        <li><a href="#">ad choice</a></li>
                        <li><a href="#">advertising</a></li>
                        <li><a href="#">jobs</a></li>
                        <li><a href="#">subscriptions</a></li>
                        <li><a href="#">talent</a></li>
                        <li><a href="#">subscriptions</a></li>
                        <li><a href="#">ad choice</a></li>
                        <li><a href="#">privacy policy</a></li>
                    </ul>
                </div>
                <div class="links">
                    <h3>SITE</h3>
                    <ul>
                        <li><a href="#">DC</a></li>
                        <li><a href="#">MAD  Magazine</a></li>
                        <li><a href="#">DC kids</a></li>
                        <li><a href="#">DC universe</a></li>
                        <li><a href="#">DC power visa</a></li>
                    </ul>
                </div>
            </div>
            <div>
                <img src="@/assets/dc-logo-bg.png" alt="logo">
            </div>
        </section>
        <section class="container display-flex">
            <button>SIGN-UP NOW!</button>
        </section>
    </footer>
</template>

<script>
export default {
    name: 'Footer'
}
</script>

<style lang='scss' scoped>
    @import '@/style/utilities';
    footer{
        flex-grow: 1;
        background-image: url('../assets/footer-bg.jpg');
        background-size: cover;
        padding: 25px 0;
        img{
            width: 90%;
        }
        section{
            .info{
                width: 50%;
                .links{
                    margin: 0px 20px;
                    h3{
                        color: white;
                        margin: 10px 0;
                    }
                }
            }
        }
        section:last-child{
            position: fixed;
            bottom: 0;
            justify-content: space-between;
            height: 50px;
            padding: 5px;
            button{
                border:1px solid dodgerblue;
                padding: 10px;
                color: white;
                background-color: transparent;
            }
        }
    }


</style>