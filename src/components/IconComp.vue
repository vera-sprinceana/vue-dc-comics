<template>
   <div>
      <ul>
          <li>
              <img src="../assets/img/buy-comics-digital-comics.png" alt="logo-dc">
              digital comics
          </li>
          <li>
              <img src="../assets/img/buy-comics-merchandise.png" alt="logo-dc">
              dc merchandise
          </li>
          <li>
              <img src="../assets/img/buy-comics-subscriptions.png" alt="logo-dc">
              subscription
          </li>
          <li>
              <img src="../assets/img/buy-comics-shop-locator.png" alt="logo-dc">
              comics shop locator
          </li>
          <li>
              <img src="../assets/img/buy-dc-power-visa.svg" alt="logo-dc">
              dc power visa
          </li>

      </ul>
   </div>
</template>

<script>
export default {
  name: 'IconComp'
}
</script>

<style scoped lang="scss">
@import '../style/variable.scss';
ul{
    list-style-type: none;
    display: flex;
    
    li{
        display: flex;
        align-items: center;
        text-transform: uppercase;
        margin-right: 50px;
        font-size: 0.7em;
        color:$color-white;
        img{
            margin-right: 10px;
            
        }
    }
}
    
</style>