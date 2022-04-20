<template>
  <div class="product">
    <div class="box">
      <img :src="src" alt="">
      <h5>{{ titolo }}</h5>
    </div>
  </div>
</template>

<script>
  export default {
    name: 'ProductComp',
    // props: ['details']
    props: {
      src: String,
      titolo: String,
    }
  }
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
  .product {
    padding-top: 50px;
    display: flex;
    justify-content: space-between;
    flex-wrap: wrap;

    .box {
      margin-right: 10px;
      padding: 20px;
      flex-basis: calc(100% / 6) - 20px;
    }
  }
</style>