<link href="https://fonts.googleapis.com/css2?family=Inter:wght@100;300;400;500&display=swap" rel="stylesheet">

<style>
  body {
    margin: 0;
    padding: 0;
    background: #000;
    display: flex;
    justify-content: center;
    align-items: center;
    height: 100vh;
    font-family: 'Inter', sans-serif;
  }

  .a23-frame {
    width: 1080px;
    height: 2408px;
    background: url('./andrbackdropviacopilot.jpeg') no-repeat center center;
    background-size: cover;
    border-radius: 40px;
    overflow: hidden;
    position: relative; /* THIS LINE IS THE FIX */
    box-shadow: 0 0 40px rgba(0,0,0,0.4);
  }

  .clock {
    position: absolute;
    top: 260px;
    left: 60px;
    font-size: 180px;
    font-weight: 100;
    color: white;
  }

  .date {
    position: absolute;
    top: 500px;
    left: 65px;
    font-size: 42px;
    font-weight: 300;
    color: white;
  }

  .swipe {
    position: absolute;
    bottom: 180px;
    left: 50%;
    transform: translateX(-50%);
    font-size: 36px;
    font-weight: 400;
    color: white;
    opacity: 0.8;
  }
</style>

<div class="a23-frame">
  <div class="clock">12:45</div>
  <div class="date">Tue, March 18</div>
  <div class="swipe">Swipe up to unlock</div>
</div>
