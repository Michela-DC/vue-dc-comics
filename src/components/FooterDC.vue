<template>
    <footer>
        <div class="footer-container">

            <div class="info-container">
                    <div class="col-1">
                        <div class="dc-comics">
                            <h3>dc comics</h3>
                            <ul>
                                <li>
                                    <a href="">Charactres</a>
                                </li>
                                <li>
                                    <a href="">Comics</a>
                                </li>
                                <li>
                                    <a href="">Movies</a>
                                </li>
                                <li>
                                    <a href="">TV</a>
                                </li>
                                <li>
                                    <a href="">Games</a>
                                </li>
                                <li>
                                    <a href="">Videos</a>
                                </li>
                                <li>
                                    <a href="">News</a>
                                </li>
                            </ul>
                        </div>
                        <div class="shop">
                            <h3>Shop</h3>
                            <ul>
                                <li>
                                    <a href="">Shop DC</a>
                                </li>
                                <li>
                                    <a href="">Shop DC Collectibles</a>
                                </li>
                            </ul>
                        </div>
                    </div>

                    <div class="col-1 dc">
                        <h3>dc</h3>
                        <ul>
                            <li>
                                <a href="">Terms Of Use</a>
                            </li>
                            <li>
                                <a href="">Provicy Ppolicy (New)</a>
                            </li>
                            <li>
                                <a href="">Ad Choices</a>
                            </li>
                            <li>
                                <a href="">Advertising</a>
                            </li>
                            <li>
                                <a href="">Jobs</a>
                            </li>
                            <li>
                                <a href="">Subscriptions</a>
                            </li>
                            <li>
                                <a href="">Talent Workshops</a>
                            </li>
                            <li>
                                <a href="">CPSC Certificates</a>
                            </li>
                            <li>
                                <a href="">Ratings</a>
                            </li>
                            <li>
                                <a href="">Shop Help</a>
                            </li>
                            <li>
                                <a href="">Contact Us</a>
                            </li>
                        </ul>
                    </div>

                    <div class="col-1 sites">
                        <h3>sites</h3>
                        <ul>
                            <li>
                                <a href="">DC</a>
                            </li>
                            <li>
                                <a href="">MAD Magazine</a>
                            </li>
                            <li>
                                <a href="">DC Kids</a>
                            </li>
                            <li>
                                <a href="">DC Universe</a>
                            </li>
                            <li>
                                <a href="">DC Power Visa</a>
                            </li>
                        </ul>
                    </div>

                <div class="logo-bg">
                    <img src="../assets/img/dc-logo-bg.png" alt="">
                </div>
            </div>

            <div class="signUp-container">
                <div class="signUp-wrapper">
                    <button>
                        sign-up now!
                    </button>

                    <div class="social-media">
                        <h3>Follow us</h3>
                        <ul class="social-wrapper">
                            <li>
                                <a href="">
                                    <img src="../assets/img/footer-facebook.png" alt="">
                                </a>
                            </li>
                            <li>
                                <a href="">
                                    <img src="../assets/img/footer-twitter.png" alt="">
                                </a>
                            </li>
                            <li>
                                <a href="">
                                    <img src="../assets/img/footer-youtube.png" alt="">
                                </a>
                            </li>
                            <li>
                                <a href="">
                                    <img src="../assets/img/footer-pinterest.png" alt="">
                                </a>
                            </li>
                            <li>
                                <a href="">
                                    <img src="../assets/img/footer-periscope.png" alt="">
                                </a>
                            </li>
                        </ul>
                    </div>
                </div>
            </div> <!-- fine signUp-container -->

        </div> <!-- fine footer container -->
    </footer>
</template>

<script>
export default {
  name: 'FooterDC',
}
</script>

<style scoped lang="scss">

footer{
    flex-grow: 1;
    background-image: url('../assets/img/footer-bg.jpg');
    background-position: center;
    background-repeat: no-repeat;
    background-size: cover;
}

.footer-container{ 
    height: 100%;
    display: flex;
    flex-direction: column;
}

.info-container{
    width: 80%;
    margin: 0 auto;
    display: flex;
    gap: 20px;
    height: 388px;
    padding: 50px 0;
    position: relative;
    overflow: hidden;

    .col-1{
        position: relative;
        z-index: 10;
    }

    h3{
        text-transform: uppercase;
        color: white;
    }

    li{
        line-height: 22px;

        a{
            color: #acacac;
            font-size: 13px;
        }
    }

    .dc-comics{
        margin-bottom: 25px;
    }
    
    .logo-bg{
        position: absolute;
        top: -95px;
        right: 0;
    }
}

.signUp-container{
    flex-grow: 1;
    width: 100%;
    background-color: #303030;
    display: flex;
    align-items: center;

    .signUp-wrapper{
        display: flex;
        align-items: center;
        width: 80%;
        margin: 0 auto;
        justify-content: space-between;
        
        button{
            background-color: transparent;
            border: 2px solid #0282F9;
            color: white;
            padding: 12px;
            text-transform: uppercase;
        }

        .social-media{
            display: flex;
            align-items: center;
            gap: 20px;
            color: #0282F9;

            .social-wrapper{
                display: flex;
                align-items: center;
                gap: 18px;

                a{
                    display: flex;
                    align-items: center;
                }

                img{
                    height: 30px;
                }

            }
        }
    }
}



</style>