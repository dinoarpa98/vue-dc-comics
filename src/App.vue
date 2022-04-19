<template>
  <div>
    <header class="container">
      <LogoComp/>
      <MenuComp/>
    </header>

    <main>
      <div class="content">
         <div class="container">
           <h3>il contenuto va qui</h3>
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

export default {
  name: 'App',
  components: {
    LogoComp,
    MenuComp,
    iconsComp
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
   padding: 30px 0;
 }

 .icons{
   background-color: rgb(20, 135, 230);
 }

</style>
