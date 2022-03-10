<template>
    <section class="menu-section">
        <div class="container">
            <ul class="menu">
                <li class="options" v-for="(option, i) in options" :key="i">
                    <img :src="option.image" alt="">
                    <a href="">{{option.text}}</a>
                </li>
            </ul>
        </div>
    </section>
</template>

<script>
export default {
  name: 'StoreDC',
  data () {
      return {
          options: [ 
              {
                image: require('../assets/img/buy-comics-digital-comics.png'),
                text: 'digital comics', 
              },
              {
                image: require('../assets/img/buy-comics-merchandise.png'),
                text: 'dc merchandise',
              },
              {
                image: require('../assets/img/buy-comics-shop-locator.png'),
                text: 'subscription',
              },
              {
                image: require('../assets/img/buy-comics-subscriptions.png'),
                text: 'comic shop locator',
              },
              {
                image: require('../assets/img/buy-dc-power-visa.svg'),
                text: 'dc power visa',
              }
          ],
      }
  }
}
</script>

<style scoped lang="scss">

@import '../assets/scss/MyVariables.scss';
@import '../assets/scss/MyMixins.scss';

.container {
    @include container;
}

.menu-section {
    background-color: $blue;


    .menu{
        height: 115px;
        @include flex-alignCenter;
        justify-content: space-evenly;
        text-transform: uppercase;

        .options{
            @include flex-alignCenter;
            gap: 10px;

            img{
                height: 50px;
            }

            &:last-child > img{
                width: 53px;
                height: 36px;
            }

            a{
                color: white;
                font-size: 15px;
            }
        }

    }
}

</style>