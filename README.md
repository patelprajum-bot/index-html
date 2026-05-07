<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Pradyuman Patel | Portfolio</title>

<style>
  body{
    margin:0;
    font-family: Arial, sans-serif;
    transition:0.3s;
    background:#f4f4f4;
    color:#333;
  }

  .dark{
    background:#111;
    color:#fff;
  }

  header{
    text-align:center;
    padding:40px 20px;
    background:linear-gradient(135deg,#4a90e2,#7b2ff7);
    color:white;
  }

  header h1{
    margin:0;
    font-size:32px;
  }

  nav{
    display:flex;
    justify-content:center;
    gap:15px;
    padding:10px;
    background:#222;
  }

  nav a{
    color:white;
    text-decoration:none;
    font-weight:bold;
  }

  section{
    padding:20px;
    max-width:800px;
    margin:auto;
  }

  .card{
    background:white;
    padding:20px;
    margin:15px 0;
    border-radius:12px;
    box-shadow:0 0 10px rgba(0,0,0,0.2);
    transition:0.3s;
  }

  .dark .card{
    background:#222;
  }

  button{
    padding:10px 15px;
    border:none;
    border-radius:8px;
    cursor:pointer;
    background:#4a90e2;
    color:white;
    margin-top:10px;
  }

  .toggle{
    position:fixed;
    top:10px;
    right:10px;
    background:black;
    color:white;
    padding:8px 12px;
    border-radius:8px;
    cursor:pointer;
  }

  footer{
    text-align:center;
    padding:15px;
    background:#222;
    color:white;
    margin-top:20px;
  }

  .card:hover{
    transform:scale(1.03);
  }
</style>
</head>

<body>

<button class="toggle" onclick="mode()">Toggle Mode</button>

<header>
  <h1>Pradyuman Patel</h1>
  <p>Web Developer | Student | Learner</p>
</header>

<nav>
  <a href="#about">About</a>
  <a href="#skills">Skills</a>
  <a href="#projects">Projects</a>
  <a href="#contact">Contact</a>
</nav>

<section id="about">
  <div class="card">
    <h2>About Me</h2>
    <p>I am Pradyuman Patel. I am currently learning web development and building my career in freelancing and coding.</p>
  </div>
</section>

<section id="skills">
  <div class="card">
    <h2>Skills</h2>
    <ul>
      <li>HTML</li>
      <li>CSS</li>
      <li>JavaScript (Learning)</li>
    </ul>
  </div>
</section>

<section id="projects">
  <div class="card">
    <h2>Projects</h2>
    <ul>
      <li>Portfolio Website</li>
      <li>Workshop Website (Coming Soon)</li>
      <li>Mini Python Projects</li>
    </ul>
  </div>
</section>

<section id="contact">
  <div class="card">
    <h2>Contact</h2>
    <p>Email: patelprajum@gmail.com</p>
    <button onclick="msg()">Say Hello</button>
  </div>
</section>

<footer>
  © 2026 Pradyuman Patel | Built with HTML, CSS & JavaScript
</footer>

<script>
  function msg(){
    alert("Thanks for visiting my portfolio!");
  }

  function mode(){
    document.body.classList.toggle("dark");
  }
</script>

</body>
</html>
