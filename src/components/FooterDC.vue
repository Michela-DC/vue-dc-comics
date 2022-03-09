<template>
    <footer>
        <section class="info-section">
            <div class="container">
                <div class="col">
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

                <div class="col dc">
                    <h4>dc</h4>
                    <ul>
                        <li v-for="(item, i) in dc" :key="i">
                            <a href="">{{item}}</a>
                        </li>
                    </ul>
                </div>

                <div class="col sites">
                    <h4>sites</h4>
                    <ul>
                        <li v-for="(item, i) in sites" :key="i">
                            <a href="">{{item}}</a>
                        </li>
                    </ul>
                </div>
            </div>
        </section>

        <section class="social-section">
            <div class="container">
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
        </section> 

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

@import '../assets/scss/MyMixins.scss';

footer{
    flex-grow: 1;
    background-image: url('../assets/img/footer-bg.jpg');
    background-position: center;
    background-repeat: no-repeat;
    background-size: cover;
    height: 100%;
    display: flex;
    flex-direction: column;
}


.info-section{
    
    .container{
        @include container;
        background-image: url('../assets/img/dc-logo-bg.png');
        background-position: right;
        background-size: 45%;
        background-repeat: no-repeat;
        display: flex;
        gap: 25px;
        padding: 55px 0;

        .col{
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
    }

}

.social-section{ 
    background-color: #303030;
    flex-grow: 1;
    display: flex;
    align-items: center;

    .container{
        width: 80%;
        margin: 0 auto;
        display: flex;
        align-items: center;
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