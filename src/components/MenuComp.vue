<template>
  <div>
    <ul>
        <li v-for="(element, index) in menuLink" :key="index"> 
            <a :href="element.url">{{element.Link}}</a> 
        </li>
    </ul>
  </div>
</template>

<script>
export default {
  name: 'MenuComp',
  data(){
      return {
          menuLink:[
              {
                  Link:'characters',
                  url:'#'
              },
               {
                  Link:'comics',
                  url:'#'
              },
               {
                  Link:'movies',
                  url:'#'
              },
               {
                  Link:'tv',
                  url:'#'
              },
              {
                  Link:'games',
                  url:'#'
              },
               {
                  Link:'collectibles',
                  url:'#'
              },
               {
                  Link:'videos',
                  url:'#'
              },
               {
                  Link:'fans',
                  url:'#'
              },
               {
                  Link:'news',
                  url:'#'
              },
               {
                  Link:'shop',
                  url:'#'
              }
          ]
      }
  }
  }

</script>

<style scoped lang="scss">
ul{
    list-style-type: none;
    display: flex;
    li{
        margin: 0 30px;
        a{
            text-decoration: none;
            text-transform: uppercase;
            color: black;
            font-weight: bold;
        }
    }
}
</style>
