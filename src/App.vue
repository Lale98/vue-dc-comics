<template>
  <div id="app">
    <div id="header" class="container">
      <Header />
    </div>

    <div id="main">
      <Main />
    </div>

    <div id="footer">
      <Footer />
    </div>
  </div>
</template>

<script>
import Header from './components/Header';
import Main from './components/Main';
import Footer from './components/Footer';

export default {

  name : "app",
  components: {
    Header,
    Main,
    Footer,

  }
}
</script>

<style lang="scss">
  @import url('https://fonts.googleapis.com/css2?family=Roboto:wght@400;500;700&display=swap');

  * {
    box-sizing: border-box;
    margin: 0;
    padding: 0;
    font-family: 'Roboto', sans-serif;
  }
  .container {
    max-width: 1170px;
    margin: 0 auto ;
  }
  

</style>
