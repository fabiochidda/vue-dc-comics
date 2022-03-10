<template>
  <div id="app">
    <Header />

    <Main />
    
    <Footer />
  </div>
</template>

<script>
import Header from './components/Header.vue'
import Main from './components/Main.vue'
import Footer from './components/Footer.vue'

export default {
  name: 'App',
  components: {
    Header,
    Main,
    Footer,
  }
}
</script>

<style lang="scss">
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  color: #2c3e50;
}

* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}

.container {
  width: 100%;
}

.container-lg {
  width: 1320px;
  display: flex;
  margin: 0 auto;
}

.row {
  display: flex;
}

ul li {
  list-style: none;

  a {
    text-decoration: none;
  }
  
}
</style>
