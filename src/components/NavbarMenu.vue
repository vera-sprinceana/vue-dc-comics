<template>
   <div>
      <LogoCompon/> 
       <ul>
           <li>characters</li>
           <li class="active">comics</li>
           <li>movies</li>
           <li>tv</li>
           <li>games</li>
           <li>collectibles</li>
           <li>videos</li>
           <li>fans</li>
           <li>news</li>
           <li>shop</li>
       </ul>
   </div>
</template>

<script>


export default {
  name: 'NavbarMenu'
}
</script>

<style scoped lang="scss">
    @import '../style/variable.scss';
    ul{
        list-style-type: none;
        display: flex;
       
    };
    ul li{
        margin:0 10px;
        text-transform: uppercase;
        font-weight: bold;
    };
    .active{
        color:$bg-icon;
        padding-bottom: 20px;
        border-bottom: 4px solid $bg-icon;
    }
    
</style>