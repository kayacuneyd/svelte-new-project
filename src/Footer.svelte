<script>
  import { Styles } from "sveltestrap";
</script>

<Styles />
<footer class="bg-dark">
  <div class="my-copyright-area">
    <div class="bd-custom-container">
      <div class="row align-items-center">
        <div class="col-lg-4 order-1 order-lg-1">
          <div class="footer-social-media pb-10 text-center">
            <a href="#" target="_blank"><i class="bi-facebook" /></a>
            <a href="#" target="_blank"><i class="bi-twitter" /></a>
            <a href="#" target="_blank"><i class="bi-instagram" /></a>
            <a href="#" target="_blank"><i class="bi-google" /></a>
          </div>
        </div>

        <div class="col-lg-4 order-2 order-lg-2">
          <div class="my-copyright pb-10 text-center">
            <p class="m-0">
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
  #logo {
    width: 8rem;
    height: 8rem;
  }
  :root {
    --clr-common-white: #fff;
    --clr-common-black: #000;
    --clr-body-heading: #161616;
    --clr-body-heading2: #232323;
    --clr-theme-1: #2161d6;
    --clr-bg-gray: #f9f9f9;
    --clr-bg-gray2: #efefef;
    --clr-border-1: #474747;
    --clr-border-2: #757575;
    --clr-border-3: #303030;
    --clr-border-4: #e5e5e5;
    --clr-border-5: #d4d4d4;
    --clr-border-6: #dfdfdf;
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

  .my-copyright p {
    font-size: 16px;
    color: #e5e5e5;
    display: inline-block;
    margin-bottom: 0px;
  }
  .my-copyright p a:hover {
    color: #e5e5e5;
  }
  /*   a,
  button {
    color: inherit;
    outline: medium none;
    text-decoration: none !important;
    transition: all 0.3s ease-out 0s;
  } */
  .my-copyright p a {
    font-weight: 600;
    color: #228fce;
  }
  .footer-social-media a {
    height: 40px;
    width: 40px;
    line-height: 40px;
    text-align: center;
    border: 1px solid var(--clr-border-6);
    font-size: 16px;
    color: #e5e5e5;
    display: inline-block;
    margin-right: 15px;
    border-radius: 50%;
    overflow: hidden;
    z-index: 1;
    position: relative;
  }
  .footer-social-media a:hover {
    border-color: var(--clr-theme-1);
    color: var(--clr-common-white);
  }
  .footer-social-media a:after {
    position: absolute;
    content: "";
    height: 100%;
    width: 100%;
    top: 0px;
    left: 0px;
    transform: scale(0);
    background: var(--clr-theme-1);
    z-index: -1;
    -webkit-transition: all 0.3s ease-out 0s;
    -moz-transition: all 0.3s ease-out 0s;
    -ms-transition: all 0.3s ease-out 0s;
    -o-transition: all 0.3s ease-out 0s;
    transition: all 0.3s ease-out 0s;
    border-radius: 50%;
  }

  .footer-social-media a:hover:after {
    transform: scale(1);
  }
  .footer-social-media a:last-child {
    margin-right: 0px;
  }
  ul {
    margin: 0px !important;
    padding: 0px !important;
  }
  .my-copyright ul li {
    list-style: none;
    display: inline-block;
    padding-right: 20px;
    margin-right: 18px;
    border-right: 1px solid var(--clr-border-6);
  }
  .my-copyright ul li a {
    font-size: 16px;
    color: var(--clr-body-heading);
    line-height: 1;
  }
  .my-copyright ul li a:hover {
    color: var(--clr-theme-1);
  }
  .my-copyright ul li:last-child {
    padding-right: 0px;
    margin-right: 0px;
    border-right: 0px;
  }
</style>
