{% raw %}
<link href="https://fonts.googleapis.com/css2?family=Inter:wght@100;300;400;500&display=swap" rel="stylesheet">

<style>
  :root {
    --scale: 1;
  }

  body {
    margin: 0;
    padding: 0;
    background: #000;
    display: flex;
    justify-content: center;
    align-items: center;
    height: 100vh;
    overflow: hidden;
    font-family: 'Inter', sans-serif;
  }

  .phone-wrapper {
    transform: scale(var(--scale));
    transform-origin: top center;
  }

  .a23-frame {
    width: 1080px;
    height: 2408px;
    background: url('./andrbackdropviacopilot.jpeg') no-repeat center center;
    background-size: cover;
    border-radius: 40px;
    overflow: hidden;
    position: relative;
    box-shadow: 0 0 40px rgba(0,0,0,0.4);
  }

  .clock {
    position: absolute;
    top: 260px;
    left: 60px;
    font-size: calc(180px * var(--scale));
    font-weight: 100;
    color: white;
  }

  .date {
    position: absolute;
    top: 500px;
    left: 65px;
    font-size: calc(42px * var(--scale));
    font-weight: 300;
    color: white;
  }

  .swipe {
    position: absolute;
    bottom: 180px;
    left: 50%;
    transform: translateX(-50%);
    font-size: calc(36px * var(--scale));
    font-weight: 400;
    color: white;
    opacity: 0.8;
  }
</style>

<script>
  function scalePhone() {
    const phoneHeight = 2408;
    const screenHeight = window.innerHeight;
    const scale = screenHeight / phoneHeight;
    document.documentElement.style.setProperty('--scale', scale);
  }
  window.onload = scalePhone;
  window.onresize = scalePhone;
</script>

<div class="phone-wrapper">
  <div class="a23-frame">
    <div class="clock">12:45</div>
    <div class="date">Tue, March 18</div>
    <div class="swipe">Swipe up to unlock</div>
  </div>
</div>
{% endraw %}
