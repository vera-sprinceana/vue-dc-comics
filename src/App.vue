<template>
  <div id="app" >
      <header class="container text">
        <LogoDcNav/>
        <NavbarMenu/>
      </header>
      <main>
        <div class="hero">
         
        </div>
        <div class="bg-black">
          <div class="container">
             <ProductsComp/>
          </div>
         
        </div>
        <div class="bg-blue">
          <div class="container">
            <IconComp/>
          </div>
        </div> 
      </main>
      <footer>
        <div class="bg-footer">
          <div class="container">
            <div class="col">
              <FooterComp1/>
              
            </div>   
          </div>
        </div>
        <div class="bg-f-2">
          <div class="container">
            <FooterComp2/>
          </div>
        </div>
      </footer>
  </div>
</template>
<script>
import LogoDcNav from './components/LogoDcNav.vue';
import NavbarMenu from './components/NavbarMenu.vue';
import ProductsComp from './components/ProductsComp.vue';
import IconComp from './components/IconComp.vue';
import FooterComp1 from './components/FooterComp1.vue';
import FooterComp2 from './components/FooterComp2.vue';

export default {
  name: 'App',
  components: {
    LogoDcNav,
    NavbarMenu,
    ProductsComp,
    IconComp,
    FooterComp1,
    FooterComp2,
  }
}
</script>

<style scoped lang="scss">
@import './style/variable.scss';
*{
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}
#app{
  width: 100%;
}
.container{
  width: 70%;
  margin: 0 auto;
  display: flex;
};
.hero{
  background-image: url('./assets/img/jumbotron.jpg');
  background-size: cover;
  background-repeat: no-repeat;
  height: 45vh;
};
.bg-black{
  background-color: $bg-shop;
}
h3{
  color: $color-white;
}
.bg-blue{
  background: $bg-icon;
  padding: 20px;
}
.bg-footer{
  background: url('./assets/img/footer-bg.jpg');
  background-repeat: no-repeat;
  background-size: cover;
}
.text{
  display: flex;
  justify-content: space-between;
};
.col{
  width:100%;
  display: flex;
  justify-content: space-between;
};
.bg-f-2{
  background: #303030;
}
</style>
