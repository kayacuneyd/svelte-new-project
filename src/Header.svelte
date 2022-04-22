<script>
  import MyNavBar from './components/MyNavBar.svelte'
</script>

<MyNavBar />
<header>

  <!-- This div is  intentionally blank. It creates the transparent black overlay over the video which you can modify in the CSS -->
  <div class="overlay"></div>

  <!-- The HTML5 video element that will create the background video on the header -->
  <video playsinline="playsinline" autoplay="autoplay" muted="muted" loop="loop">
    <source src="./static/video/space-vd.mp4" type="video/mp4">
  </video>

  <!-- The header content -->
  <div class="container h-100">
    <div class="d-flex h-100 text-center align-items-center">
      <div class="w-100 text-white">
        <h1 class="display-3">Cüneyt Kaya</h1>
        <h4 class="lead mb-0">a Frontend & WordPress Developer</h4>
        <br>
        <a href="#footer" id="myButton">For more information</a>
      </div>
    </div>
  </div>
</header>

<style>
  #myButton{

    padding: 7.5px 15px;
    text-decoration: none;
    background-color: #208FCE;
    color: white;
    border-radius: 5px;
    border: 1px solid gray;
  }
  #myButton:hover{
    background-color: transparent;
  }
</style>
