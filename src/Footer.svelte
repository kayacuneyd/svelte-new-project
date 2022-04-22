<script>
  import { Styles } from "sveltestrap";
  import SocialMedia from "./components/SocialMedia.svelte";
</script>

<Styles />
<footer id="footer">
  <div class="my-copyright-area">
    <div class="bd-custom-container">
      <div class="row align-items-center">
        <div class="col-lg-4 order-1 order-lg-1">
          <SocialMedia />
        </div>

        <div class="col-lg-4 order-2 order-lg-2">
          <div class="my-copyright pb-10 text-center">
            <p class="m-0 text-white">
              © 2022 All rights reserved | Design &amp; Develop by <a
                href="https://kayacuneyt.com"
                target="_blank">Cüneyt Kaya</a
              >
            </p>
          </div>
        </div>

        <div class="col-lg-4 order-3 order-lg-3">
          <div
            class="my-copyright pb-10 text-lg-end text-center d-flex justify-content-center"
          >
            <img src="static/images/logo.png" id="logo" alt="logo" />
          </div>
        </div>
      </div>
    </div>
  </div>
</footer>

<style>
  #footer{
    background-color: black;
  }
  #logo {
    width: 8rem;
    height: 8rem;
  }

  .my-copyright-area {
    padding-top: 32px;
    padding-bottom: 20px;
  }

  .bd-custom-container {
    max-width: 1730px;
    padding-left: 15px;
    padding-right: 15px;
    margin: 0 auto;
  }
  .pb-10 {
    padding-bottom: 10px;
  }

  .my-copyright p a {
    font-weight: 600;
    color: #228fce;
  }
</style>