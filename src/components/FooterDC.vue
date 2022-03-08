<template>
    <footer>
        <div class="footer-container">

            <div class="info-container">
                    <div class="col-1">
                        <div class="dc-comics">
                            <h4>dc comics</h4>
                            <ul>
                                <li v-for="(item, i) in dcComics" :key="i">
                                    <a href="">{{item}}</a>
                                </li>
                            </ul>
                        </div>

                        <div class="shop">
                            <h4>Shop</h4>
                            <ul>
                                <li v-for="(item, i) in shop" :key="i">
                                    <a href="">Shop DC</a>
                                </li>
                            </ul>
                        </div>
                    </div>

                    <div class="col-1 dc">
                        <h4>dc</h4>
                        <ul>
                            <li v-for="(item, i) in dc" :key="i">
                                <a href="">{{item}}</a>
                            </li>
                        </ul>
                    </div>

                    <div class="col-1 sites">
                        <h4>sites</h4>
                        <ul>
                            <li v-for="(item, i) in sites" :key="i">
                                <a href="">{{item}}</a>
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
                            <li v-for="(item, i) in icons" :key="i">
                                <a href="">
                                    <img :src="item" alt="">
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
  data () {
      return {
          dcComics: [
            'Charactres',
            'Comics',
            'Movies',
            'TV',
            'Games',
            'Videos',
            'News'
          ],

          shop: [
            'Shop DC',
            'Shop DC Collectibles'
          ],

          dc: [
            'Terms Of Use',
            'Provicy Ppolicy (New)',
            'Ad Choices',
            'Advertising',
            'Jobs',
            'Subscriptions',
            'Talent Workshops',
            'CPSC Certificates',
            'Ratings',
            'Shop Help',
            'Contact Us'
          ],
        
        sites: [
            'DC',
            'MAD Magazine',
            'DC Kids',
            'DC Universe',
            'DC Power Visa',
        ],

        icons: [
           require ('../assets/img/footer-facebook.png'),
            require ('../assets/img/footer-twitter.png'),
            require ('../assets/img/footer-youtube.png'),
            require ('../assets/img/footer-pinterest.png'),
            require ('../assets/img/footer-periscope.png'),
        ]
      }
  }
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
    gap: 25px;
    height: 388px;
    padding: 52px 0;
    position: relative;
    overflow: hidden;

    .col-1{
        position: relative;
        z-index: 10;

        h4{
            text-transform: uppercase;
            color: white;
            margin-bottom: 10px;
        }

        li{
            line-height: 20px;

            a{
                color: #acacac;
                font-size: 12px;
            }
        }

        .dc-comics{
            margin-bottom: 25px;
        }
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

                    img{
                        height: 30px;
                    }
                }
            }
        }
    }
}



</style>