<template>
  <div id="app">
    <div id="header" class="container">
      <Header />
    </div>

    <div id="main">
      <Main />
    </div>

    <div id="footer">

    </div>
  </div>
</template>

<script>
import Header from './components/Header';
import Main from './components/Main';

export default {

  name : "app",
  components: {
    Header,
    Main,

  }
}
</script>

<style lang="scss">
  * {
    box-sizing: border-box;
    margin: 0;
    padding: 0;
  }
  .container {
    max-width: 1170px;
    margin: 0 auto ;
  }
  

</style>
