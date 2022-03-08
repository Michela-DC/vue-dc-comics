<template>
  <header>
      <div class="header-container">
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

.header-container{
    display: flex;
    align-items: center;
    justify-content: space-between;
    height: 115px;
    width: 80%;
    margin: 0 auto;
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

    a{
        color: black;  
        font-weight: bold;  
    }
}
</style>