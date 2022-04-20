<template>
  <div>
    <header class="container">
      <LogoComp/>
      <MenuComp/>
    </header>

    <main>
      <div class="jumbo">
        <!-- <JumboSection/> -->
        
      </div>
      <div class="series">
          CURRENT SERIES
        </div>
      <div class="content">
         <div class="container">
           <ProductSection/>
         </div>
      </div>

      <div class="icons">
        <iconsComp/>
      </div>

    </main>
    
    <footer>
      <FooterComp/>
    </footer>
  </div>
</template>

<script>

import LogoComp from './components/LogoComp.vue'
import MenuComp from './components/MenuComp.vue'
import iconsComp from './components/iconsComp.vue'
import ProductSection from './components/ProductSection.vue'
import FooterComp from './components/FooterComp.vue'
// import JumboSection from './components/JumboSection'

export default {
  name: 'App',
  components: {
    LogoComp,
    MenuComp,
    iconsComp,
    ProductSection,
    FooterComp,
    // JumboSection,
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

 .jumbo{
   background-image: url('./assets/img/jumbotron.jpg');
   height: 400px;
   background-size: cover;
   position: relative;
 }

 .series{
   color: white;
   border: 1px solid rgb(20, 135, 230);
   width: fit-content;
   background-color: rgb(20, 135, 230);
   padding: 10px;
   position: absolute;
   left: 10%;
   bottom: 45%;
 }

</style>
