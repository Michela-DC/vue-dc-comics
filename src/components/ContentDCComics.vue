<template>
    <main>
        <div class="main-container">
            <div class="content-container">
                <div class="content">
                    CONTENT
                </div>
            </div>

            <div class="menu-container">
                <ul class="menu">
                    <li class="options" v-for="(option, i) in options" :key="i">
                        <img :src="option.image" alt="">
                        <a href="">{{option.text}}</a>
                    </li>
                </ul>
            </div>
        </div>
    </main>
</template>

<script>
export default {
  name: 'ContentDCComics',
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

.main-container{
    color: white;
}

.content-container{
    background-color: black;

    .content{
        height: 115px;
        width: 80%;
        margin: 0 auto;
        display: flex;
        align-items: center;
    }
}

.menu-container {
    background-color: #0282F9;

    .menu{
        height: 115px;
        width: 80%;
        margin: 0 auto;
        display: flex;
        align-items: center;
        justify-content: space-evenly;
        text-transform: uppercase;

        .options{
            display: flex;
            align-items: center;
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