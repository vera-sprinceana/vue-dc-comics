<template>
  <footer>
    <div>
      <button>SING-UP NOW!</button> 
    </div>
    <div class="d-flex">
      <h3>follow us</h3>
      <ul>
        <li  v-for="(element, index) in iconsFooter" :key="index">
          <img :src="element.url " alt="logo-facebook">
        </li>
      </ul>
    </div>
  </footer>
</template>

<script>
export default {
  name: 'FooterComp2',
   data(){
     return {
       iconsFooter:[
         {
           name:'logo-facebook',
           url: require('../assets/img/footer-facebook.png')
         },
          {
           name:'logo-twitter',
           url: require('../assets/img/footer-twitter.png')
         },
          {
           name:'logo-youtube',
           url: require('../assets/img/footer-youtube.png')
         },
          {
           name:'logo-pinterest',
           url: require('../assets/img/footer-pinterest.png')
         },
          {
           name:'logo-periscope',
           url: require('../assets/img/footer-periscope.png')
         },
       ]
     }
   }
}
</script>

<style scoped lang="scss">
@import '../style/variable.scss';
 
  footer {
    width: 100%;
    display: flex;
    justify-content: space-between;
    align-items: center;
    padding: 20px;
  }
  button {
    background: #303030;
    border: 2px solid  $color-blue;
    color: $color-white;
    padding: 10px;
  };
  h3{
    color: $color-blue;
    text-transform: uppercase;
  }
  .d-flex{
    display: flex;
    justify-content: flex-end;
    align-items: center;
  }
  img{
    margin: 12px;
  }
  ul{
    list-style-type: none; 
    display: flex;
  }
</style>