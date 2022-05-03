<template>
  <footer id="site_footer">
    <div class="footer_top">
      <div class="container">
        <div class="row">
          <div class="col-6 menu">
            <div class="row">
              <div class="col-3">
                <div class="col">
                  <h3>DC COMICS</h3>
                  <ul>
                    <li>Characters</li>
                    <li>Comics</li>
                    <li>Characters</li>
                    <li>Characters</li>
                    <li>Characters</li>
                    <li>Characters</li>
                    <li>Characters</li>
                  </ul>
                </div>
                <div class="col">
                  <h3>SHOP</h3>
                  <ul>
                    <li>Characters</li>
                    <li>Comics</li>
                  </ul>
                </div>
              </div>
              <div class="col-3">
                <div class="col">
                  <h3>DC</h3>
                  <ul>
                    <li>Characters</li>
                    <li>Comics</li>
                    <li>Characters</li>
                    <li>Characters</li>
                    <li>Characters</li>
                    <li>Characters</li>
                    <li>Comics</li>
                    <li>Characters</li>
                    <li>Characters</li>
                    <li>Characters</li>
                    <li>Characters</li>
                  </ul>
                </div>
              </div>
              <div class="col-3">
                <div class="col">
                  <h3>SITES</h3>
                  <ul>
                    <li>Characters</li>
                    <li>Comics</li>
                    <li>Characters</li>
                    <li>Characters</li>
                    <li>Characters</li>
                  </ul>
                </div>
              </div>
            </div>
          </div>
          <div class="col-6 bg_logo"></div>
        </div>
      </div>
    </div>
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
  </footer>
</template>

<script>
export default {
  name: "footerComponent",
};
</script>

<style lang="scss" scoped>
.footer_top {
  height: 380px;
  background-image: url("@/assets/img/footer-bg.jpg");

  .bg_logo {
    height: 380px;
    background-image: url("@/assets/img/dc-logo-bg.png");
    background-repeat: no-repeat;
    background-position: center;
  }

  h3 {
    color: white;
    margin-top: 1.5rem;
  }

  ul {
    list-style: none;
    margin-top: 0.5rem;
  }

  li {
    color: gray;
    font-size: 12px;
    padding: 0.2rem;
  }
}

.footer_bottom {
  padding: 2rem;
  background-color: #303030;

  .call-to-action{
    display: flex;
    align-items: center;
  }

  button {
    height: 100%;
    border: 2px solid #0582f9;
    border-radius: 0;
    padding: 0.8rem;
    background-color: transparent;
    color: white;
  }

  .follow-us {
      display: flex;
      justify-content: right;
      align-items: center;
  }

  h3 {
      margin-right: 1rem;
      color: #0582f9;
  }

  img {
      margin-right: 1rem;
  }
}
</style>