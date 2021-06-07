<template>
  <div>
      <div id="main">
        <div class="container">
            <h2> --> Content goes here  </h2>
        </div>
      </div>
      <div id="main-bar">
          <div class="container">

          </div>
      </div>
  </div>
</template>

<script>
export default {
    name : "Main",

}
</script>

<style lang="scss" scoped>
    $colorBlue : #0282F9;
    #main {
        background-color: #1C1C1C;
        color: white;
        padding: 50px 0;
    }
    #main-bar {
        height: 180px;
        background-color: $colorBlue;
    }
</style>