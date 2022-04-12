<template>
  <div id="app" >
      <header class="container">
        <LogoCompon/>
        <NavbarMenu/>
      </header>
      <main>
        <div class="b-shop">
          <div class="container">
            <h3>--> Content goes here </h3>
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
          <div class="container ">
            <FooterComp1/>
        </div>
        </div>
        
        <div class="container">
           <FooterComp2/>
        </div>
      </footer>
  </div>
</template>
<script>
import NavbarMenu from './components/NavbarMenu.vue';
import LogoCompon from './components/LogoCompon.vue';
import IconComp from './components/IconComp.vue';
import FooterComp1 from './components/FooterComp1.vue';
import FooterComp2 from './components/FooterComp2.vue';
export default {
  name: 'App',
  components: {
    NavbarMenu,
    LogoCompon,
    IconComp,
    FooterComp1,
    FooterComp2,
  }
}
</script>

<style lang="scss">
@import './style/variable.scss';
#app{
  width: 100%;
}
.container{
  width: 70%;
  margin: 0 auto;
  display: flex;
};
.b-shop{
  background: $bg-shop;
  padding: 10px;
};
h3{
  color: $color-white;
}
.bg-blue{
  background: $bg-icon;
  padding: 20px;
}
.bg-footer{
  background: url('./assets/img/footer-bg.jpg');
  padding: 80px;
}

</style>
