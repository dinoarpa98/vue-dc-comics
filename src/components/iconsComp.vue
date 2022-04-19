<template>
  <div>
    <ul class="container">
      <li v-for="(element, index) in iconsList" :key="index">
        <img :src="element.url" alt="">
        <h3>{{element.nomeIcona}}</h3>
      </li>
    </ul>
  </div>
</template>

<script>
export default {
  name: 'iconsComp',

  data(){
    return{
      iconsList: [
        {
          nomeIcona:'DIGITAL COMICS',
          url: require('../assets/img/buy-comics-digital-comics.png')
        },
         {
          nomeIcona:'DC MERCHANDISE',
          url: require('../assets/img/buy-comics-merchandise.png')
        },
         {
          nomeIcona:'SUBSCRIPTION',
          url: require('../assets/img/buy-comics-shop-locator.png')
        },
         {
          nomeIcona:'COMIC SHOP LOCATOR',
          url: require('../assets/img/buy-comics-subscriptions.png')
        },
         {
          nomeIcona:'DC POWER VISA',
          url: require('../assets/img/buy-dc-power-visa.svg')
        },
      ]
    }
  }
  }

</script>

<style scoped lang="scss">


ul{
    list-style-type: none;
    display: flex;
    justify-content: space-between;
    padding: 20px;
    li{
        display: flex;
        align-items: center;
        color: white;
       h3{
         margin-left: 20px;
       }
    }
}
</style>
