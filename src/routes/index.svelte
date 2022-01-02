<script>
  import { fade, fly } from "svelte/transition";
  import DiCodeBadge from "svelte-icons/di/DiCodeBadge.svelte";
  import IoMdInformationCircle from "svelte-icons/io/IoMdInformationCircle.svelte";
  import IoLogoLinkedin from "svelte-icons/io/IoLogoLinkedin.svelte";
  let showLinks = false;
  const toggleShowLinks = () => {
    showLinks = !showLinks;
  };
</script>

<svelte:head>
  <title>Ross MacDonald</title>
</svelte:head>
<div in:fly={{ duration: 1000, y: 300, delay: 400 }} class="page-box">
  <div class="container">
    <div class="badge">
      <div class="hole">
        <div class="ring">
          <img class="string" src="ellipse.png" alt="ellipse" />
        </div>
      </div>
      <div class="image">
        <img width="180" src="headshot.png" alt="avatar" />
      </div>
      <div class="text">
        <h2>Ross MacDonald</h2>
        <div class="sub-header">
          <h4>Full Stack Software Engineer</h4>
        </div>
      </div>
      <div class="links">
        <div class="link">
          <a href="https://www.linkedin.com/in/rsmacdonald/">
            <IoLogoLinkedin />
          </a>
        </div>
        <div class="link">
          <a href="/">
            <IoMdInformationCircle />
          </a>
        </div>
        <div class="link">
          <a href="/">
            <DiCodeBadge />
          </a>
        </div>
      </div>
    </div>
  </div>
</div>

<style>
  * {
    font-family: "Roboto", sans-serif;
  }
  .links {
    display: flex;
    justify-content: space-evenly;
    margin-top: 20px;
    width: 50%;
    border-radius: 15px;
    color: white;
  }
  .link {
    width: 50px;
  }
  a {
    color: #000;
  }
  .string {
  }
  .badge {
    width: 350px;
    height: 550px;
    background-image: linear-gradient(#2e4052 60%, white 50%);
    border-radius: 10px;
    display: flex;
    flex-direction: column;
    align-items: center;
    transform: rotate(-7deg);
    box-shadow: 0 2.8px 2.2px rgba(0, 0, 0, 0.034),
      0 6.7px 5.3px rgba(0, 0, 0, 0.048), 0 12.5px 10px rgba(0, 0, 0, 0.06),
      0 22.3px 17.9px rgba(0, 0, 0, 0.072), 0 41.8px 33.4px rgba(0, 0, 0, 0.086),
      0 100px 80px rgba(0, 0, 0, 0.12);
    position: relative;
    border: 1px double rgba(0, 0, 0, 0.2);
  }

  .badge::after {
    position: absolute;
    bottom: 0;
    left: 0;
    width: 100%;
    content: "";
    border-bottom: 40px solid #2e4052;
    border-bottom-left-radius: 10px;
    border-bottom-right-radius: 10px;
  }

  .hole {
    background: white;
    height: 20px;
    width: 60px;
    margin-top: 15px;
    border-radius: 5px;
    box-shadow: inset 0 0 7px rgba(0, 0, 0, 0.75);
    position: relative;
  }
  .ring {
    position: absolute;
    top: -240px;
    left: 0;
  }
  .image {
    margin-top: 30px;
  }
  .text {
    color: white;
    border-radius: 5px;
    padding: 15px;
    margin-top: 10px;
    background: rgb(80, 42, 64);
  }
  .container {
    padding: 5%;
  }
  .page-box {
    transition: 0.75s all linear;
  }
  @media only screen and (min-width: 520px) {
  }
</style>
