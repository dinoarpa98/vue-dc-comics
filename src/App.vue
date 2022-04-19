<template>
  <div>
    <header class="container">
      <LogoComp/>
      <MenuComp/>
    </header>

    <main>
      <div class="content">
         <div class="container">
           <ProductSection/>
         </div>
      </div>

      <div class="icons">
        <iconsComp/>
      </div>

    </main>

  </div>
</template>

<script>

import LogoComp from './components/LogoComp.vue'
import MenuComp from './components/MenuComp.vue'
import iconsComp from './components/iconsComp.vue'
import ProductSection from './components/ProductSection.vue'

export default {
  name: 'App',
  components: {
    LogoComp,
    MenuComp,
    iconsComp,
    ProductSection
  }
}
</script>

<style lang="scss">

@import './style/reset.scss';
@import './style/mixin.scss';
@import './style/global.scss';


 header{
   @include flexContent(space-between, center);
 }

 .content{
   background-color: black;
   color: #fff;
   padding: 20px;
   display: flex;
 }

 .icons{
   background-color: rgb(20, 135, 230);
 }

</style>
