<script>
export default {
  data() {
    return {
      
    }
  }
}
</script>

<template>
<div>
  <div class="footer-bottom">
    <div class="container">
      <div class="left-side">
        <button>SIGN-UP NOW!</button>
      </div>
      <div class="right-side">
        <a href="#">FOLLOW US</a>
        <img src="../assets/img/footer-facebook.png" alt="facebook-logo">
        <img src="../assets/img/footer-twitter.png" alt="twitter-logo">
        <img src="../assets/img/footer-youtube.png" alt="youtube-logo">
        <img src="../assets/img/footer-pinterest.png" alt="pinterest-logo">
        <img src="../assets/img/footer-periscope.png" alt="periscope-logo">
      </div>
    </div>
  </div>
</div>
</template>

<style lang="scss" scoped>
  .footer-bottom {
    background-color: #303030;

  }

  .container {
    display: flex;
    justify-content: space-between;
    align-items: center;
  }

  button {
    border: 2px solid #0C7CEC;
    background-color: transparent;
    color: #fff;
    font-weight: 600;
    padding: 10px 15px;
    cursor: pointer;
  }
  .right-side {
    display: flex;
    justify-content: space-between;
    align-items: center;
    gap: 2rem;
  }

  a {
    color: #0C7CEC;
    font-weight: 600;
  
  }
</style>