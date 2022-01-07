<script>
</script>

<div id="paper">
  <div id="top" />
  <div id="pattern">
    <div id="content">
      <div class="link-div">
        <h2><a href="/experience">- Experience</a></h2>
      </div>
      <div class="link-div">
        <h2><a href="/contact">- Contact</a></h2>
      </div>
      <div class="link-div">
        <h2><a href="/resume">- Resume</a></h2>
      </div>
      <div class="link-div">
        <h2><a href="/mywork">- Projects</a></h2>
      </div>
    </div>
  </div>
</div>

<style>
  .link-div {
  }
  a {
    text-decoration: none;
    color: rgba(0, 0, 0, 0.85);
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
    left: 32px;
    background: rgb(244, 248, 1, 0.5);
    visibility: hidden;
    transform: scaleX(0);
    transform-origin: center;
    transition: 0.25s linear;
  }
  .link-div:nth-child(1) > h2 > a:before {
    width: 142px;
  }
  .link-div:nth-child(2) > h2 > a:before {
    width: 112px;
  }
  .link-div:nth-child(3) > h2 > a:before {
    width: 102px;
  }
  .link-div:nth-child(4) > h2 > a:before {
    width: 107px;
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

  #paper::before {
    content: "";
    width: 2px;
    height: 100%;
    position: absolute;
    top: 0;
    left: 40px;
    background-color: rgba(255, 0, 0, 0.6);
  }

  #pattern {
    height: 100%;
    background-image: repeating-linear-gradient(
      rgb(248, 248, 237) 0px,
      rgb(248, 248, 237) 24px,
      teal 25px
    );
  }
  #content {
    padding-top: 6px;
    padding-left: 56px;
    padding-right: 16px;
    line-height: 25px;
    font-family: "Amatic SC", cursive;
    font-size: 30px;
    letter-spacing: 1px;
    word-spacing: 5px;
    display: flex;
    flex-direction: column;
    justify-content: space-evenly;
  }
</style>
