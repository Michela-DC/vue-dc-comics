<template>
  <header>
      <div class="container">
        <figure class="logo-wrapper">
            <img class="logo" src="../assets/img/dc-logo.png" alt="">
        </figure>

        <ul class="navbar">
            <li v-for="(option ,i) in options" :key="i">
                <a href="">{{option}}</a>
            </li>
        </ul>
      </div>
  </header>
</template>

<script>
export default {
  name: 'HeaderDC',
  data() {
      return {
          options: [
              'characters',
              'comics',
              'movies',
              'tv',
              'games',
              'collectibles',
              'videos',
              'fans',
              'news',
              'shop'
          ]
      }
  }
}
</script>

<style scoped lang="scss">

@import '../assets/scss/MyVariables.scss';
@import '../assets/scss/MyMixins.scss';

.container {
    @include container;
    @include flex-alignCenter;
    height: 115px;
    justify-content: space-between;
}

.logo-wrapper {
    .logo{
        height: 80px;
    }
}

.navbar {
    display: flex;
    flex-wrap: wrap;
    gap: 30px;
    text-transform: uppercase;
    height: 100%;

    li {

        a{
            color: black;  
            font-weight: bold; 
            height: 100%; 
            @include flex-alignCenter;
            position: relative;

        }

    }

    li:nth-child(2) a{
        color: $blue;

        &::after{
            content: '';
            display: block;
            position: absolute;
            height: 4px;
            width: 100%;
            bottom: 0;
            background-color: $blue;
        }
    }
}
</style>