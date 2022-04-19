<template>
   <div class="navbar">
       <ul v-for="(element, index) in navbarList" :key='index'>
           <li>{{element.name}}</li>
           <li class="active"></li>
       </ul>
   </div>
</template>

<script>


export default {
  name: 'NavbarMenu',
  data(){
      return {
           navbarList:[
          {
                name:'characters',
          },
          {
                name:'comics',
          },
          {
                name:'movies',
          },
          {
                name:'tv',
          },
          {
                name:'games',
          },
          {
                name:'videos',
          },
          {
                name:'fans',
          },
          {
                name:'news',
          },
          {
                name:'shop',
          }
      ]
      }
  }
}
</script>

<style scoped lang="scss">
    @import '../style/variable.scss';
    .navbar{
        widows: 70%;
        margin: 0 auto;
        display: flex;
        justify-content: space-between;
    }
    ul{
        list-style-type: none;
        display: flex; 
    };
     li{
        font-size: 0.8em;
        text-transform: uppercase;
        font-weight: bold;
    };
    .active{
        color:$bg-icon;
        padding-bottom: 20px;
        border-bottom: 4px solid $bg-icon;
    }
    
</style>