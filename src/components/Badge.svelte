<script>
  import DiCodeBadge from "svelte-icons/di/DiCodeBadge.svelte";
  import IoMdInformationCircle from "svelte-icons/io/IoMdInformationCircle.svelte";
  import IoLogoLinkedin from "svelte-icons/io/IoLogoLinkedin.svelte";
</script>

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
  <div class="links" />
</div>

<style>
  .links {
    display: flex;
    justify-content: space-evenly;
    margin-top: 20px;
    width: 50%;
    border-radius: 15px;
    color: white;
  }
  .badge {
    width: 300px;
    height: 450px;
    background-image: linear-gradient(#2e4052 65%, white 50%);
    border-radius: 10px;
    display: flex;
    z-index: 4;
    flex-direction: column;
    align-items: center;
    transform: rotate(-7deg);
    box-shadow: 0 2.8px 2.2px rgba(0, 0, 0, 0.034),
      0 6.7px 5.3px rgba(0, 0, 0, 0.048), 0 12.5px 10px rgba(0, 0, 0, 0.06),
      0 22.3px 17.9px rgba(0, 0, 0, 0.072), 0 41.8px 33.4px rgba(0, 0, 0, 0.086);
    position: relative;
  }

  .badge::after {
    position: absolute;
    bottom: 0;
    left: 0;
    width: 100%;
    content: "";
    border-bottom: 30px solid #2e4052;
    border-bottom-left-radius: 10px;
    border-bottom-right-radius: 10px;
  }

  .hole {
    background: rgb(250, 239, 217);
    height: 20px;
    width: 60px;
    margin-top: 15px;
    border-radius: 5px;
    box-shadow: inset 0 0 5px rgb(88, 78, 56);
    position: relative;
  }
  .ring {
    position: absolute;
    top: -240px;
    left: 20px;
    transform: rotate(15deg);
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
    box-shadow: -5px 5px 0px rgba(255, 200, 87), -10px 10px 0 #bdd9bf;
  }
</style>
