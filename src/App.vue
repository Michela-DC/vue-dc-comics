<template>
  <div id="app">
    <HeaderDC/>
    <MainContentDC/>
    <FooterDC/>
  </div>
</template>

<script>

import HeaderDC from './components/HeaderDC.vue'
import MainContentDC from './components/MainContentDC.vue'
import FooterDC from './components/FooterDC.vue'

export default {
  name: 'App',
  components: {
    HeaderDC,
    MainContentDC,
    FooterDC
  }
}
</script>

<style lang="scss">
@import url('https://fonts.googleapis.com/css2?family=Roboto:wght@400;500&display=swap');
// @import url('../assets/scss/MyMixins');

*{
  box-sizing: border-box;
  margin: 0;
  padding: 0;
  font-family: 'Roboto', sans-serif;
}

ul li{
  list-style: none;
}

a{
  text-decoration: none;
}

#app {
  height: 100vh;
  display: flex;
  flex-direction: column;
}

// .container {
//   @include container;
// }

</style>
