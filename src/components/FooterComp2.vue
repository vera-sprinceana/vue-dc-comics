<template>
  <footer>
    <div>
      <button>SING-UP NOW!</button> 
    </div>
    <div class="d-flex">
      <h3>follow us</h3>
      <img src="../assets/img/footer-facebook.png" alt="logo-facebook">
      <img src="../assets/img/footer-twitter.png" alt="logo-twitter">
      <img src="../assets/img/footer-youtube.png" alt="logo-youtube">
      <img src="../assets/img/footer-pinterest.png" alt="logo-pinterest">
      <img src="../assets/img/footer-periscope.png" alt="logo-periscope">
    </div>
  </footer>
</template>

<script>
export default {
  name: 'FooterComp2'
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
  }
  img{
    margin: 12px;
  }
</style>