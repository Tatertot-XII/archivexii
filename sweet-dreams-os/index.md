<style>
  body {
    margin: 0;
    padding: 0;
    height: 100vh;
    width: 100vw;

    /* PERFECTLY CENTERED WALLPAPER */
    background-image: url('sweet-dreams-os/andrbackdropviacopilot.jpeg');
    background-size: cover;
    background-position: center center;

    font-family: 'Inter', sans-serif;
    color: white;
    overflow: hidden;
    position: relative;
  }

  /* CLOCK + DATE BLOCK */
  .clock-container {
    position: absolute;
    top: 38%; /* moves clock higher for One UI spacing */
    left: 50%;
    transform: translateX(-50%);
    text-align: center;
  }

  .clock {
    font-size: 72px;
    font-weight: 600;
    letter-spacing: -2px;
  }

  .date {
    margin-top: 12px; /* spacing between time + date */
    font-size: 22px;
    opacity: 0.85;
  }

  /* SWIPE TEXT */
  .swipe {
    position: absolute;
    bottom: 55px; /* moves it lower */
    left: 50%;
    transform: translateX(-50%);
    font-size: 18px;
    opacity: 0.8;
  }
</style>

<!-- CLOCK + DATE -->
<div class="clock-container">
  <div class="clock">12:45</div>
  <div class="date">Tue, March 19</div>
</div>

<!-- SWIPE TEXT -->
<div class="swipe">Swipe up to unlock</div>
