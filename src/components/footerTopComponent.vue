<template>
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
</template>

<script>
export default {
    name: 'footerTopComponent'
}
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
</style>