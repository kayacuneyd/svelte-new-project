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
