<script>
  export const socialData = [
    {
      "name": "facebook",
      "url": "https://www.facebook.com/kayacueneytt/"
    },
    {
      "name": "twitter",
      "url": "https://twitter.com/cueneytkaya"
    },
    {
      "name": "instagram",
      "url": "https://www.instagram.com/kayacueneyt/"
    },
    {
      "name": "envelope",
      "url": "mailto:kayacuneyd@gmail.com"
    }
  ]
export let name;
export let url;
</script>
<div class="footer-social-media pb-10 text-center">
  {#each socialData as data}
    <a href="{data.url}" target="_blank"><i class="bi-{data.name}" /></a>
  {/each}
</div>

  <style>

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
    border-color: grey;
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
    background: #208FCE;
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

  </style>