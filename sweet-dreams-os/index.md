<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Sweet Dreams OS</title>

<style>
  body {
    margin: 0;
    padding: 0;
    height: 100vh;
    width: 100vw;
    display: flex;
    justify-content: center;
    align-items: center; /* centers the phone perfectly */
    background: #000; /* outside background */
    font-family: 'Inter', sans-serif;
  }

  /* PHONE FRAME */
  .phone {
    width: 390px; /* iPhone / Samsung width */
    height: 844px; /* tall phone aspect ratio */
    border-radius: 40px; /* rounded top + bottom */
    overflow: hidden;
    position: relative;
    background-image: url('andrbackdropviacopilot.jpeg');
    background-size: cover;
    background-position: center center;
  }

  /* CLOCK + DATE BLOCK */
  .clock-container {
    position: absolute;
    top: 38%;
    left: 50%;
    transform: translateX(-50%);
    text-align: center;
    color: white;
  }

  .clock {
    font-size: 72px;
    font-weight: 600;
    letter-spacing: -2px;
  }

  .date {
    margin-top: 12px;
    font-size: 22px;
    opacity: 0.85;
  }

  /* SWIPE TEXT */
  .swipe {
    position: absolute;
    bottom: 55px;
    left: 50%;
    transform: translateX(-50%);
    font-size: 18px;
    opacity: 0.8;
    color: white;
  }
</style>

</head>
<body>

<div class="phone">
  <div class="clock-container">
    <div class="clock">12:45</div>
    <div class="date">Tue, March 19</div>
  </div>

  <div class="swipe">Swipe up to unlock</div>
</div>

</body>
</html>
