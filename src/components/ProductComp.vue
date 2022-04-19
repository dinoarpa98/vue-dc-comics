<template>
    <div class="product">
      <div class="box">
        <!-- <img :src="details.src" alt="">
        <h3>{{ details.titolo }}</h3> -->
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
    display: flex;
    justify-content: center;
    .box {
      margin-right: 10px;
      padding: 20px;
      height: 50%;
    }

    .box img{
      width: 70%;
    }
    
  }
</style>