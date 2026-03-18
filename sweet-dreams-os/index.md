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
    height: 100vh;
    width: 100vw;
    overflow: hidden;
    display: flex;
    justify-content: center;
    align-items: flex-start;
    font-family: 'Inter', sans-serif;
  }

  /* Move whole phone down slightly */
  .phone-wrapper {
    margin-top: 60px;
    transform: scale(var(--scale));
    transform-origin: top center;
    height: 2408px;
    width: 1080px;
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

  /* CENTERED CLOCK */
  .clock {
    position: absolute;
    top: calc(900px * var(--scale));
    left: 50%;
    transform: translateX(-50%);
    font-size: calc(180px * var(--scale));
    font-weight: 100;
    color: white;
  }

  /* DATE UNDER CLOCK */
  .date {
    position: absolute;
    top: calc(1100px * var(--scale));
    left: 50%;
    transform: translateX(-50%);
    font-size: calc(42px * var(--scale));
    font-weight: 300;
    color: white;
  }

  /* SWIPE TEXT MOVED UP */
  .swipe {
    position: absolute;
    top: calc(1500px * var(--scale));
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
