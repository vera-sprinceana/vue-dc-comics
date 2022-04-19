<template>
   <div class="nav">
      <ul>
          <li v-for="(element, index) in icons" :key="index">
              <img :src="element.url" alt="">
             
              <h4>{{element.titolo}}</h4>
          </li>
      </ul>
   </div>
</template>

<script>
export default {
  name: 'IconComp',
 data() {
    return {
        icons: [
            {
                url: require('../assets/img/buy-comics-digital-comics.png'),
                titolo:'digital comics'
            },
            {
                url: require('../assets/img/buy-comics-merchandise.png'),
                titolo:'dc merchandise'
            },
            {
                url:require('../assets/img/buy-comics-subscriptions.png'),
                titolo:'subscription'
            },
            {
                url: require('../assets/img/buy-comics-shop-locator.png'),
                titolo:'dcomics shop locator'
            },
            {
                url: require('../assets/img/buy-dc-power-visa.svg'),
                titolo:'dc power visa'
            },
        ]
    }
} 
}

</script>

<style scoped lang="scss">
@import '../style/variable.scss';
ul{
    list-style-type: none;
    display: flex;
    justify-content: space-between;
    li{
        display: flex;
        align-items: center;
        text-transform: uppercase;
        padding-right: 25px ;
        h4{  
            color:$color-white;
            margin-left: 10px;  
            font-size: 0.7em;
        }
       img{
           width: 30px;
       }
    }
}
    .nav{
        display: flex;
       
    }
</style>