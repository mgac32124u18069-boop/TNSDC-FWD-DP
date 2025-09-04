<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>My Portfolio</title>
  <style>
    body {
      margin: 0;
      font-family: Arial, sans-serif;
      scroll-behavior: smooth;
    }

    /* Navbar */
    nav {
      background: #222;
      padding: 15px 40px;
      display: flex;
      justify-content: space-between;
      align-items: center;
      position: fixed;
      top: 0;
      width: 100%;
      z-index: 1000;
    }
    nav h2 {
      color: #fff;
      margin: 0;
    }
    nav ul {
      list-style: none;
      margin: 0;
      padding: 0;
      display: flex;
    }
    nav ul li {
      margin-left: 20px;
    }
    nav ul li a {
      color: #fff;
      text-decoration: none;
      transition: 0.3s;
    }
    nav ul li a:hover {
      color: lightblue;
    }
    .tagline{
      font-style:italic;
      font size:22px;
      color:#8e44ad;
      margin-top:-px;
      margin-bottom:20px;
    }

    /* Hero Section */
    .hero {
      background: linear-gradient(to right, #00c6ff, #0072ff);
      color: white;
      text-align: center;
      padding: 100px 20px;
      margin-top: 60px;
    }
    .hero h1 {
      font-size: 2.5em;
    }
    .hero button {
      margin-top: 20px;
      padding: 10px 20px;
      border: none;
      background: white;
      color: #0072ff;
      border-radius: 5px;
      cursor: pointer;
      font-size: 1em;
      transition: 0.3s;
    }
    .hero button:hover {
      background: lightgray;
    }

    /* About Section */
    #about {
      padding: 60px 20px;
      text-align: center;
    }
    #about img {
      width: 150px;
      height: 150px;
      border-radius: 50%;
      object-fit: cover;
      margin-bottom: 20px;
    }
    

    /* Projects Section */
    #projects {
      padding: 60px 20px;
      text-align: center;
      background: #f9f9f9;
    }
    .project-list {
      display: flex;
      justify-content: center;
      flex-wrap: wrap;
      gap: 20px;
    }
    .project {
      background: #fff;
      padding: 20px;
      border-radius: 10px;
      box-shadow: 0 2px 6px rgba(0,0,0,0.1);
      width: 250px;
    }

    /* Contact Section */
    #contact {
      padding: 60px 20px;
      text-align: center;
    }
    form {
      max-width: 400px;
      margin: auto;
    }
    input, textarea {
      width: 100%;
      padding: 10px;
      margin: 8px 0;
      border: 1px solid #ccc;
      border-radius: 5px;
    }
    button[type="submit"] {
      background: #0072ff;
      color: white;
      border: none;
      padding: 10px;
      border-radius: 5px;
      cursor: pointer;
      width: 100%;
    }
    button[type="submit"]:hover {
      background: #0056cc;
    }
  </style>
</head>
<body>

  <!-- Navbar -->
  <nav>
    <h2>MyPortfolio</h2>
    <ul>
      <li><a href="#hero">Home</a></li>
      <li><a href="#about">About</a></li>
      <li><a href="#projects">Projects</a></li>
      <li><a href="#contact">Contact</a></li>
    </ul>
  </nav>

  <!-- Hero Section -->
  <section class="hero" id="hero">
    <h1>Hello, I'm <span style="color: yellow;">TAMIZHSELVI</span></h1> 
  <p class="tagline">"Beauticians add sparkle not just to faces, but to lives.”</P>
    
    <button onclick="document.querySelector('#projects').scrollIntoView({behavior:'smooth'})">
      View My Work
    </button>
  </section>

  <!-- About Section -->
  <section id="about">
    <h2>About Me</h2>
    <!-- Replace 'profile.jpg' with your image file -->
    <img src="profile.jpg" alt="My Profile Picture">
    <p>Hi, I'm Tamizhselvi, a passionate beautician.<br>
Beauty has always been my passion, and I use my skills in makeup, hairstyling, and skincare to enhance confidence and bring out natural beauty. I specialize in bridal looks, party makeovers, and personal grooming.</p> 
  </section>
  <!-- Projects Section -->
  <section id="projects">
    <h2>Projects</h2>
    <div class="project-list">
      <div class="project">
        <h3>Project 1</h3> 
      </div>
      <div class="project">
        <h3>Project 2</h3> 
      </div>
      <div class="project">
        <h3>Project 3</h3>
      </div>
<!-- Contact Section -->
<section id="contact">
  <h2>Contact Me</h2>
  <form action="https://formspree.io/f/your-form-id" method="POST">
    <input type="text" name="name" placeholder="Your Name" required>
    <input type="email" name="email" placeholder="Your Email" required>
    <textarea name="message" rows="5" placeholder="Your Message" required></textarea>
    <button type="submit">Send</button>
  </form>
</section>
