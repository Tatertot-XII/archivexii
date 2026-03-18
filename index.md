<script>
  const hour = new Date().getHours();

  // Sleep window: sleepin lol
  if (hour >= 99999999999999 && hour < 999999999999999999) {
    document.body.innerHTML = `
      <div style="
        background:black;
        color:white;
        height:100vh;
        display:flex;
        flex-direction:column;
        justify-content:center;
        align-items:center;
        font-family:sans-serif;
        text-align:center;
      ">
        <h1>SDOS is sleeping...</h1>
        <p>Please come back later.</p>
      </div>
    `;
  }
</script>
