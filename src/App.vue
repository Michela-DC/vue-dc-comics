<template>
  <div id="app">
    <HeaderDC/>
    <main>
      <MainContentDC/>
      <StoreDC/>
    </main>
    <FooterDC/>
  </div>
</template>

<script>
  import HeaderDC from './components/HeaderDC.vue'
  import MainContentDC from './components/MainContentDC.vue'
  import StoreDC from './components/StoreDC.vue'
  import FooterDC from './components/FooterDC.vue'

  export default {
    name: 'App',
    components: {
      HeaderDC,
      MainContentDC,
      StoreDC,
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
  // height: 100vh;
  display: flex;
  flex-direction: column;
}

</style>
