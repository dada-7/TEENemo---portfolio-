# TEENemo---portfolio-
<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8" />
<meta name="viewport" content="width=device-width, initial-scale=1" />
<title>TEENemo Portfolio</title>
<link rel="stylesheet" href="style.css" />
</head>
<body>

<header>
  <h1>TEENemo</h1>
</header>

<nav>
  <a href="#about">About</a>
  <a href="#portfolio">Portfolio</a>
  <a href="#testimonials">Testimonials</a>
  <a href="#blog">Blog</a>
  <a href="#contact">Contact</a>
  <a href="https://www.instagram.com/_tee.nemo/profilecard/?igsh=b3BmaGJlYXVwemlm" target="_blank" class="social-link" aria-label="Instagram">Instagram</a>
</nav>

<section id="about" class="container">
  <h2 class="section-title">About Me</h2>
  <p>
    I am a passionate graphic designer specializing in creative digital and print media solutions.
    With a strong focus on branding, visual storytelling, and user-centric design, I strive to bring ideas to life.
  </p>
</section>

<section id="portfolio" class="container">
  <h2 class="section-title">My Works</h2>
  <div class="portfolio-grid">
    <div class="portfolio-item">
      <a href="#img1"><img src="images/project1.jpg" alt="Project 1"></a>
    </div>
    <div class="portfolio-item">
      <a href="#img2"><img src="images/project2.jpg" alt="Project 2"></a>
    </div>
    <div class="portfolio-item">
      <a href="#img3"><img src="images/project3.jpg" alt="Project 3"></a>
    </div>
    <div class="portfolio-item">
      <a href="#img4"><img src="images/project4.jpg" alt="Project 4"></a>
    </div>
  </div>

  <!-- Lightbox images -->
  <div id="img1" class="lightbox">
    <a href="#portfolio" title="Close">&times;</a>
    <img src="images/project1.jpg" alt="Project 1 large view" />
  </div>
  <div id="img2" class="lightbox">
    <a href="#portfolio" title="Close">&times;</a>
    <img src="images/project2.jpg" alt="Project 2 large view" />
  </div>
  <div id="img3" class="lightbox">
    <a href="#portfolio" title="Close">&times;</a>
    <img src="images/project3.jpg" alt="Project 3 large view" />
  </div>
  <div id="img4" class="lightbox">
    <a href="#portfolio" title="Close">&times;</a>
    <img src="images/project4.jpg" alt="Project 4 large view" />
  </div>
</section>

<section id="testimonials" class="container">
  <h2 class="section-title">Testimonials</h2>
  <div class="testimonial">
    “Amazing creativity and professionalism. Highly recommended!”
  </div>
  <div class="testimonial">
    “Delivered beyond expectations on every project.”
  </div>
</section>

<section id="blog" class="container">
  <h2 class="section-title">Blog</h2>
  <div class="blog-post">
    <h3>Design Trends 2025</h3>
    <p>Exploring the latest trends shaping the world of graphic design this year...</p>
  </div>
  <div class="blog-post">
    <h3>How to Build a Brand Identity</h3>
    <p>Key elements and best practices for creating a memorable brand...</p>
  </div>
</section>

<section id="contact" class="container">
  <h2 class="section-title">Contact Me</h2>
  <form>
    <label for="name">Name:</label><br />
    <input type="text" id="name" name="name" required style="width:100%; padding:10px;margin-bottom:10px;"/>

    <label for="email">Email:</label><br />
    <input type="email" id="email" name="email" required style="width:100%; padding:10px;margin-bottom:10px;"/>

    <label for="message">Message:</label><br />
    <textarea id="message" name="message" rows="6" required style="width:100%; padding:10px;resize:none;"></textarea><br />

    <button type="submit" style="background:white; color:black; font-weight:bold; cursor:pointer; padding:10px 20px; border:none; border-radius:4px;">
      Send Message
    </button>
  </form>
</section>

<footer>
  &copy; 2025 TEENemo – All rights reserved.
</footer>

<script src="script.js"></script>
</body>
</html>

body {
  background: #000;
  color: #fff;
  font-family: Arial, sans-serif;
  margin: 0; padding: 0;
}
header {
  padding: 20px;
  text-align: center;
  border-bottom: 2px solid #fff;
}
header h1 {
  margin: 0; font-size: 2.5rem;
  letter-spacing: 0.1em;
  font-weight: bold;
}
nav {
  display: flex;
  justify-content: center;
  gap: 30px;
  background: #111;
  padding: 15px 0;
}
nav a {
  color: white;
  text-decoration: none;
  font-weight: bold;
  font-size: 1.1rem;
  transition: color 0.3s;
}
nav a:hover {
  color: #999;
}
section.container {
  max-width: 900px;
  margin: 40px auto;
}
h2.section-title {
  font-weight: bold;
  border-bottom: 3px solid white;
  padding-bottom: 10px;
  letter-spacing: 0.1em;
  font-size: 2rem;
  margin-bottom: 25px;
}

/* Portfolio grid */
.portfolio-grid {
  display: grid;
  grid-template-columns: repeat(auto-fit,minmax(250px,1fr));
  gap: 15px;
}
.portfolio-item {
  cursor: pointer;
  border: 2px solid #fff;
  border-radius: 5px;
  overflow: hidden;
  transition: transform 0.3s;
}
.portfolio-item:hover {
  transform: scale(1.05);
}
.portfolio-item img {
  width: 100%;
  display: block;
  height: 180px;
  object-fit: cover;
}

/* Lightbox styles */
.lightbox {
  position: fixed;
  top: 0; left: 0;
  width: 100vw; height: 100vh;
  background: rgba(0,0,0,0.9);
  display: none;
  align-items: center;
  justify-content: center;
  z-index: 1000;
}
.lightbox img {
  max-width: 90%;
  max-height: 90%;
  border: 3px solid #fff;
  border-radius: 6px;
}
.lightbox:target {
  display: flex;
}

/* About section */
#about p {
  line-height: 1.5;
  font-size: 1.1rem;
}

/* Testimonials */
.testimonial {
  margin-bottom: 20px;
  border-left: 5px solid #fff;
  padding-left: 15px;
  font-style: italic;
}

/* Blog */
.blog-post {
  margin-bottom: 25px;
}
.blog-post h3 {
  margin: 0 0 5px 0;
}
.blog-post p {
  margin: 0;
}

/* Footer */
footer {
  background: #111;
  text-align: center;
  padding: 15px 0;
  color: #777;
  font-size: 0.9rem;
}

/* Instagram icon */
.social-link {
  margin-left: 10px;
  color: white;
  text-decoration: none;
}
.social-link:hover {
  color: #999;
}
