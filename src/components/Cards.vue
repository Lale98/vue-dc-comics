<template>
  <div class="image">
      <img :src="item.thumb" :alt="item.series">
      <h4> {{ item.series }} </h4>
  </div>
</template>

<script>
export default {
    nome: "Cards",
    props: ["item"]
}
</script>

<style lang="scss" scoped>

    img {
        height: 170px;
        width: 170px;
        object-fit: cover;
        object-position: top;
        margin-bottom: 10px;
    }

    h4 {
        text-transform: uppercase;
        font-size: 14px;
    }
    

</style>