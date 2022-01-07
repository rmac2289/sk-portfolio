<script>
</script>

<div id="paper">
  <div id="pattern">
    <div id="content">
      <h2>- About</h2>
      <h2>- Experience</h2>
      <h2>- Contact</h2>
      <h2>- Resume</h2>
      <h2>- Contact</h2>
    </div>
  </div>
</div>

<style>
  #paper {
    width: 450px;
    height: 500px;
    position: relative;
    padding-top: 40px;
    transform: rotate(8deg);
    z-index: 3;
    padding-bottom: 40px;
    background-color: rgb(248, 248, 237);
    box-shadow: 0px 0px 5px 0px #888, 1px 1px 0px rgb(248, 248, 237),
      2px 2px 0px rgb(248, 248, 237), 3px 3px 0 rgb(248, 248, 237),
      4px 4px 0px rgb(248, 248, 237);
  }

  /* styling red vertical line */
  #paper::before {
    content: "";
    width: 2px;
    height: 100%;
    position: absolute;
    top: 0;
    left: 40px;
    background-color: rgba(255, 0, 0, 0.6);
  }

  /* styling blue horizontal lines */
  #pattern {
    height: 100%;
    background-image: repeating-linear-gradient(
      rgb(248, 248, 237) 0px,
      rgb(248, 248, 237) 24px,
      teal 25px
    );
  }

  /* styling text content */
  #content {
    padding-top: 6px;
    padding-left: 56px;
    padding-right: 16px;
    line-height: 25px;
    font-family: "Amatic SC", cursive;
    font-size: 28px;
    letter-spacing: 1px;
    word-spacing: 5px;
  }
</style>
