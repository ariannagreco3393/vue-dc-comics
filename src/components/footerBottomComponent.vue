<template>
    <div class="footer_bottom">
      <div class="container">
        <div class="row">
          <div class="col-6 call-to-action">
            <button>SIGN-UP NOW!</button>
          </div>
          <div class="col-6 follow-us">
            <h3>FOLLOW US</h3>
            <div class="social">
              <img src="@/assets/img/footer-facebook.png" alt="" />
              <img src="@/assets/img/footer-twitter.png" alt="" />
              <img src="@/assets/img/footer-youtube.png" alt="" />
              <img src="@/assets/img/footer-pinterest.png" alt="" />
              <img src="@/assets/img/footer-periscope.png" alt="" />
            </div>
          </div>
        </div>
      </div>
    </div>
</template>


<script>
export default {
    name: 'footerBottomComponent'
}
</script>


<style lang="scss" scoped>
    .footer_bottom {
  padding: 2rem;
  background-color: $footer;

  .call-to-action{
    display: flex;
    align-items: center;
  }

  button {
    height: 100%;
    border: 2px solid $dc-primary;
    border-radius: 0;
    padding: 0.8rem;
    background-color: transparent;
    color: $white;
  }

  .follow-us {
      display: flex;
      justify-content: right;
      align-items: center;
  }

  h3 {
      margin-right: 1rem;
      color: $dc-primary;
  }

  img {
      margin-right: 1rem;
  }
}
</style>