<template>
  <header>
      <div class="header-container">
        <figure class="logo-wrapper">
            <img class="logo" src="../assets/img/dc-logo.png" alt="">
        </figure>

        <ul class="navbar">
            <li>
                <a href="">charactres</a>
            </li>
            <li>
                <a href="">comics</a>
            </li>
            <li>
                <a href="">movies</a>
            </li>
            <li>
                <a href="">tv</a>
            </li>
            <li>
                <a href="">games</a>
            </li>
            <li>
                <a href="">collectibles</a>
            </li>
            <li>
                <a href="">videos</a>
            </li>
            <li>
                <a href="">fans</a>
            </li>
            <li>
                <a href="">news</a>
            </li>
            <li>
                <a href="">shop</a>
            </li> 
        </ul>
      </div>
  </header>
</template>

<script>
export default {
  name: 'HeaderDC',
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
    gap: 30px;
    text-transform: uppercase;

    a{
        color: black;  
        font-weight: bold;  
    }
}
</style>