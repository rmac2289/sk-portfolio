<script>
  import Badge from "../components/Badge.svelte";
  import { fade, fly } from "svelte/transition";
</script>

<svelte:head>
  <title>Ross MacDonald</title>
</svelte:head>
<div in:fly={{ duration: 1000, y: 300, delay: 400 }} class="page-box">
  <div class="container">
    <Badge />
  </div>
</div>

<style>
  * {
    font-family: "Roboto", sans-serif;
  }

  .container {
    padding: 10%;
  }

  .page-box {
    transition: 0.75s all linear;
    height: 100vh;
    width: 100vw;
    background-image: linear-gradient(
      70deg,
      rgb(250, 239, 217) 65%,
      rgb(189, 217, 191, 0.8) 50%
    );
  }
  @media only screen and (min-width: 520px) {
  }
</style>
