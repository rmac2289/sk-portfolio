<script>
    import { fade, fly } from "svelte/transition";
  </script>
  
  <svelte:head>
    <title>Ross MacDonald</title>
  </svelte:head>
  <div
    in:fly={{ duration: 1000, y: 300, delay: 400 }}
    class="page-box"
  >
    <div class="container">
      <div class="badge">
        <div class="hole">
          </div>
          <div class="image">
            <img width="200" src="avatar.png" alt="avatar">
          </div>
          <div class="text">
      <h2>Ross MacDonald</h2>
      <div class="sub-header">
        <h4>
          Full Stack Software Engineer
        </h4>
        <h4 style="color: blue;">
          <strong>Problem Solver</strong>
        </h4>
        <h4 style="color: purple;">
          Leader
        </h4>
        </div>
      </div>
    </div>
    </div>
  </div>
  
  <style>
    * {
      font-family: "Roboto", sans-serif;
    }
    .badge {
      width: 350px;
      height: 550px;
      background-image: linear-gradient(black 50%, transparent 50%);
      border-radius: 10px;
      display: flex;
      flex-direction: column;
      align-items: center;
      border: 5px solid black;
      border-bottom: 30px solid black
    }
    .hole {
      background: white;
      height: 20px;
      width: 60px;
      margin-top: 15px;
      border-radius: 5px
    }
    .image {
      margin-top: 30px;
    }
    .text {
      background: white;
      border-radius: 5px;
      padding: 15px;
      margin-top: 10px;
    }
    .container {
      max-width: 600px;
      display: flex;
      flex-direction: column;
      justify-content: center;
      padding: 1rem;
      min-height: 200px;
    }
    .page-box {
      
      transition: 0.75s all linear;
    }
    @media only screen and (min-width: 520px) {
     
    }
  </style>
  