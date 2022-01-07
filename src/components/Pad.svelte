<script>
</script>

<div id="paper">
  <div id="top" />
  <div id="pattern">
    <div id="content">
      <h2><a href="/">- About</a></h2>
      <h2><a href="/">- Experience</a></h2>
      <h2><a href="/">- Contact</a></h2>
      <h2><a href="/">- Resume</a></h2>
      <h2><a href="/">- Projects</a></h2>
    </div>
  </div>
</div>

<style>
  a {
    text-decoration: none;
    color: inherit;
  }
  h2 {
    position: relative;
  }
  h2 > a:before {
    content: "";
    position: absolute;
    width: 36%;
    height: 20px;
    bottom: -20px;
    left: 25px;
    background: rgb(244, 248, 1, 0.5);
    visibility: hidden;
    transform: scaleX(0);
    transform-origin: center;
    transition: 0.25s linear;
  }
  h2:nth-child(1) > a:before {
    width: 80px;
  }
  h2:nth-child(2) > a:before {
    width: 140px;
  }
  h2:nth-child(3) > a:before {
    width: 110px;
  }
  h2:nth-child(4) > a:before {
    width: 100px;
  }
  h2:nth-child(5) > a:before {
    width: 105px;
  }
  h2 > a:hover:before,
  h2 > a:focus:before {
    visibility: visible;
    transform: scaleX(1) rotate(-5deg);
  }
  #top {
    position: absolute;
    top: 0;
    left: 0;
    right: 0;
    height: 30px;
    background-color: rgb(250, 207, 120);
    z-index: 4;
    box-shadow: 0px 2px 0px 0px rgb(248, 248, 237);
  }
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
