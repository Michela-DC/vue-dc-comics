<template>
  <div id="app">
    <HeaderDC/>
    <ContentDCComics/>
    <FooterDC/>
  </div>
</template>

<script>

import HeaderDC from './components/HeaderDC.vue'
import ContentDCComics from './components/ContentDCComics.vue'
import FooterDC from './components/FooterDC.vue'

export default {
  name: 'App',
  components: {
    HeaderDC,
    ContentDCComics,
    FooterDC
  }
}
</script>

<style lang="scss">
@import url('https://fonts.googleapis.com/css2?family=Roboto:wght@400;500&display=swap');

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
</style>
