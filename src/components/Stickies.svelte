<script>
</script>

<ul>
  <li>
    <a href="#" contenteditable>
      <h2>ABOUT</h2>
    </a>
  </li>
  <li>
    <a href="#" contenteditable>
      <h2>EXPERIENCE</h2>
    </a>
  </li>
  <li>
    <a href="#" contenteditable>
      <h2>PROJECTS</h2>
    </a>
  </li>
  <li>
    <a href="#" contenteditable>
      <h2>CONTACT</h2>
    </a>
  </li>
  <li>
    <a href="#" contenteditable>
      <h2>RESUME</h2>
    </a>
  </li>
</ul>

<style>
  h2 {
    font-weight: bold;
    font-size: 32px;
    font-family: "Amatic SC", cursive;
  }
  ul,
  li {
    list-style: none;
  }
  ul {
    display: grid;
    grid-template-columns: 1fr 1fr 1fr;
    margin-top: 200px;
  }
  ul li a {
    text-decoration: none;
    color: #000;
    background: #ffc;
    display: block;
    height: 10em;
    width: 10em;
    padding: 1em;
    box-shadow: 5px 5px 7px rgba(33, 33, 33, 0.7);
    transform: rotate(-6deg);
    transition: transform 0.15s linear;
  }

  ul li:nth-child(even) a {
    transform: rotate(4deg);
    position: relative;
    background: #cfc;
  }
  ul li:nth-child(3n) a {
    transform: rotate(-3deg);
    position: relative;
    background: #ccf;
  }
  ul li:nth-child(5n) a {
    transform: rotate(5deg);
    position: relative;
  }

  ul li a:hover,
  ul li a:focus {
    box-shadow: 10px 10px 7px rgba(0, 0, 0, 0.7);
    transform: scale(1.15);
    position: relative;
    z-index: 5;
  }
</style>
