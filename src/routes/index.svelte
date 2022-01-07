<script>
  import Badge from "../components/Badge.svelte";
  import { fade, fly } from "svelte/transition";
  import Pad from "../components/Pad.svelte";
</script>

<svelte:head>
  <title>Ross MacDonald</title>
</svelte:head>
<div in:fly={{ duration: 1000, y: 300, delay: 400 }} class="page-box">
  <div class="laptop"><img width="1000" src="laptop.png" alt="laptop" /></div>
  <div class="container">
    <Badge />
    <Pad />
  </div>
</div>

<style>
  * {
    font-family: "Roboto", sans-serif;
  }

  .container {
    padding: 5%;
    display: flex;
  }
  .laptop {
    position: absolute;
    top: -450px;
    left: 50%;
    width: 1000px;
    margin-left: -500px;
    transform: rotate(20deg);
  }
  .page-box {
    position: relative;
    height: 100vh;
    width: 100vw;
    background-image: linear-gradient(
      20deg,
      rgb(189, 217, 191, 0.8) 35%,
      rgb(248, 240, 226) 35%
    );
  }
  @media only screen and (min-width: 520px) {
  }
</style>
