# ketantyagi
Ketan Tyagi- personal website
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>Ketan Tyagi - Personal Website</title>
    <style>
      /* General Reset */
      * {
        margin: 0;
        padding: 0;
        box-sizing: border-box;
      }
      @import url("https://fonts.googleapis.com/css2?family=Poppins:wght@300;400;500;600&display=swap");
      i body {
        font-family: "poppins", sans-serif;
        background-color: white;

        overflow-x: hidden;
        line-height: 1.6;
      }

      /* Header */
      header {
        background-color: white;
        color: white;
        padding: 20px;
        position: fixed;
        width: 100%;
        top: 0;
        left: 0;
        z-index: 999;
        display: flex;
        justify-content: space-between;
        align-items: center; /* or baseline */
      }

      header .logo {
        font-size: 2rem;
        font-weight: bold;
        color: black;
        background-color: white;
        padding: 1px 1px;
        border-radius: 10px;
      }

      header h1 {
        font-size: 3rem;
        text-align: center;
        margin: 0;
        color: black;
      }

      header h1 span {
        color: rgb(250, 152, 6); /* First letter of first name */
        font-weight: bold;
      }

      header h1 span:last-child {
        color: rgb(250, 152, 6); /* First letter of last name */
        font-weight: bold;
      }

      header nav {
        text-align: center;
        margin-top: 20px;
      }

      header nav a {
        color: rgb(4, 4, 4);
        text-decoration: none;
        padding: 9px 20px;
        font-size: 15px;
        margin: 0 5px;
        transition: background-color 0.7s ease-in-out;
      }

      header nav a:hover {
        background-color: rgb(250, 152, 6);
      }

      /* Hero Section */
      #hero {
        background: url("no") no-repeat center center/cover;
        height: 100vh;
        display: flex;
        justify-content: space-between;
        align-items: center;
        text-align: center;
        color: black;
        shape-margin: 30%;
        padding-left: 9%;
        color: rgb(19, 18, 18);
        text-shadow: 2px 2px 8px rgba(42, 42, 42, 0.7);
      }
      .hero-image {
        flex: 1;
        display: flex;
        justify-content: right;
        max-width: 60%;
        overflow: hidden;
        border-radius: 50px;
        padding: 80px;
        align-items: right;
      }

      .hero-image img {
        width: 100%;
        height: auto;
        max-width: 400px;
        border-radius: 20%;
        box-shadow: 0px 4px 10px rgba(0, 0, 0, 0.2);
        object-fit: cover;
        border-top-left-radius: 100px;
        border-bottom-left-radius: 50px;
        border: 8px solid rgb(250, 152, 6);
      }
      #hero h2 {
        font-size: 2rem;
      }

      /* About Section */
      #about {
        padding: 80px 20px;
        background: #fff;
        text-align: center;
      }

      #about img {
        width: 250px;
        border-radius: 50%;
        margin-bottom: 20px;
        border: 7px solid #4caf50;
        box-shadow: 0 4px 12px rgba(0, 0, 0, 0.1); /* Added shadow */
      }

      #about h2 {
        font-size: 2.5rem;
        margin-bottom: 20px;
      }

      #about p {
        font-size: 1.2rem;
        max-width: 900px;
        margin: 0 auto;
        line-height: 1.8;
      }

      #about a {
        display: inline-block;
        font-size: 18px;
        color: #4caf50;
        text-decoration: none;
        border: 2px solid #4caf50;
        padding: 10px 20px;
        border-radius: 5px;
        transition: background-color 0.3s ease-in-out;
      }

      #about a:hover {
        background-color: #4caf50;
        color: white;
      }

      /* Portfolio Section */
      #portfolio {
        padding: 80px 20px;
        background: #f9f9f9;
        text-align: center;
      }

      #portfolio h2 {
        font-size: 2.5rem;
        margin-bottom: 20px;
      }

      .portfolio-gallery {
        display: flex;
        flex-wrap: wrap;
        justify-content: center;
        gap: 20px;
      }

      .portfolio-gallery img {
        width: 300px;
        height: 200px;
        object-fit: cover;
        border-radius: 8px;
        transition: transform 0.3s ease;
      }

      .portfolio-gallery img:hover {
        transform: scale(1.05);
      }

      /* Contact Section */
      #contact {
        padding: 80px 20px;
        background: #fff;
        text-align: center;
      }

      #contact h2 {
        font-size: 2.5rem;
        margin-bottom: 20px;
      }

      #contact form input,
      #contact form textarea {
        width: 80%;
        padding: 15px;
        margin: 10px 0;
        border: 2px solid #ccc;
        border-radius: 5px;
      }

      #contact form button {
        padding: 15px 30px;
        background-color: #4caf50;
        color: white;
        border: none;
        border-radius: 5px;
        cursor: pointer;
        transition: background-color 0.3s ease-in-out;
      }

      #contact form button:hover {
        background-color: #45a049;
      }

      /* Footer Section */
      footer {
        padding: 20px 0;
        text-align: center;
        background: rgb(63, 63, 63);
        color: white;
      }

      footer p {
        margin-bottom: 10px;
      }

      footer a {
        color: #4caf50;
        text-decoration: none;
      }

      footer a:hover {
        text-decoration: underline;
      }

      /* Smooth Scroll */
      html {
        scroll-behavior: smooth;
      }

      /* Responsive Design */
      @media (max-width: 768px) {
        #hero h2 {
          font-size: 2rem;
        }

        #about img {
          width: 200px;
        }

        .portfolio-gallery {
          flex-direction: column;
        }
      }
      .hover-bar {
        position: fixed;
        top: 50%;
        right: -140px; /* Initially hidden */
        transform: translateY(-50%);
        display: flex;
        flex-direction: column;
        background: rgba(0, 0, 0, 0.8);
        padding: 10px;
        border-radius: 30px 0 0 30px;
        transition: right 0.8s ease-in-out;
        animation: movevertical 1.5s infinite alternate ease-in-out;
      }

      /* Diagonal Movement */
      @keyframes movevertical {
        from {
          transform: translateY(-90%) translateX(0);
        }
        to {
          transform: translateY(-150%) translateX(10px);
        }
      }

      /* Stop Animation on Hover */
      .hover-bar:hover {
        animation-play-state: paused; /* Stops movement when hovered */
        right: 0; /* Moves into view */
        transform: translateY(-50%) scale(1.05); /* Pops out slightly */
      }

      /* Social Links */
      .hover-bar a {
        color: white;
        text-decoration: none;
        padding: 10px 15px;
        font-size: 16px;
        font-weight: bold;
        display: flex;
        align-items: center;
        gap: 8px;
        transition: background-color 0.3s ease-in-out;
      }

      .hover-bar a:hover {
        background: rgb(250, 152, 6);
        border-radius: 2px;
      }

      .hover-bar img {
        width: 30px;
        height: 30px;
      }

      /* Social Links */
      .hover-bar a {
        color: white;
        text-decoration: none;
        padding: 10px 15px;
        font-size: 16px;
        font-weight: bold;
        display: flex;
        align-items: center;
        gap: 8px;
        transition: background-color 0.3s ease-in-out;
      }

      .hover-bar a:hover {
        background: rgb(250, 152, 6);
        border-radius: 2px;
      }

      .hover-bar img {
        width: 30px;
        height: 30px;
      }
    </style>
  </head>
  <body>
    <!-- Header -->
    <header>
      <!-- Logo on the left -->
      <div class="logo">KT</div>

      <h1><span>K</span>etan <span>T</span>yagi</h1>

      <!-- Navigation Menu -->
      <nav>
        <a href="#hero">Home</a>
        <a href="#about">About Me</a>
        <a href="#portfolio">Portfolio</a>
        <a href="#contact">Contact</a>
      </nav>
    </header>

    <!-- Hero Section -->
    <section
      id="hero"
      style="
        display: flex;
        align-items: center;
        justify-content: space-between;
        padding: 5% 9%;
      "
    >
      <!-- Left Content: Text -->
      <div style="max-width: 550px">
        <h2
          style="font-size: 2.2rem; color: rgb(22, 22, 22); margin-bottom: 20px"
        >
          Welcome to My Personal Website.
        </h2>

        <!-- Stylish Box for the Lower Text -->
        <div
          style="
            background-color: rgb(248, 234, 214);
            padding: 12px 22px;
            border-radius: 25px;
            border-left: 6px solid rgb(250, 152, 6);
            box-shadow: 3px 3px 10px rgb(148, 147, 147);
            display: inline-block;
            max-width: 520px;
          "
        >
          <p
            style="
              font-size: 1.3rem;
              line-height: 1.4;
              color: #1f1f1f;
              margin: 0;
            "
          >
            I craft innovative, high-performance web applications designed for
            impact, scalability, and a seamless user experience. Let's create
            something amazing together!
          </p>
        </div>
      </div>

      <!-- Right Content: Hero Image (Shifted More to Right) -->
      <div class="hero-image" style="margin-left: 50px">
        <img src="DSC_0002.jpg" alt="hero image" />
      </div>
    </section>

    <div class="hover-bar">
      <a
        href="https://www.linkedin.com/in/ketan-tyagi-3418b932b?utm_source=share&utm_campaign=share_via&utm_content=profile&utm_medium=ios_api"
        target="_blank"
      >
        <img src="linkedin.png" alt="LinkedIn" /> LinkedIn
      </a>
      <a
        href="https://www.instagram.com/ketantyagi_?igsh=MWY0c3Vrc3BwNWFtNg%3D%3D&utm_source=qr"
        target="_blank"
      >
        <img src="logo2.png" alt="Instagram" />Instagram
      </a>
    </div>

    <!-- About Section -->
    <section id="about">
      <img src="IMG_0632.jpg" alt="Ketan Tyagi" />
      <h2>About Me</h2>
      <p>
        Hi, I'm Ketan Tyagi, a Full-Stack Developer with deep expertise in
        front-end development and a passion for creating, visually stunning web
        solutions. With 40+ technical skills, Beyond coding, I have a strong
        grasp of business management, allowing me to develop solutions that are
        both innovative and strategically impactful. I also apply my analytical
        mindset in trading, making data-driven decisions. With exceptional
        speaking and listening skills, I communicate ideas effectively and
        thrive in dynamic environments. Let’s collaborate and turn ideas into
        reality!
      </p>

      <!-- "Let's Talk" Link -->
      <p style="margin-top: 20px">
        <a href="mailto:ketantyagi3495@gmail.com" target="_blank">Let's Talk</a>
      </p>
    </section>

    <!-- Portfolio Section -->
    <section id="portfolio">
      <h2>My Work</h2>
      <div class="portfolio-gallery">
        <img src="insert-project1-image.jpg" alt="Project 1" />
        <img src="insert-project2-image.jpg" alt="Project 2" />
        <img src="insert-project3-image.jpg" alt="Project 3" />
      </div>
    </section>

    <!-- Contact Section -->
    <section id="contact">
      <h2>Contact Me</h2>
      <form action="#">
        <input type="text" placeholder="Your Name" required />
        <input type="email" placeholder="Your Email" required />
        <textarea placeholder="Your Message" required></textarea>
        <button type="submit">Send Message</button>
      </form>
    </section>

    <!-- Footer Section -->
    <footer>
      <p>&copy; 2025 Ketan Tyagi | All Rights Reserved</p>
      <p>
        Connect with me on
        <a
          href="https://www.linkedin.com/in/ketan-tyagi-3418b932b?utm_source=share&utm_campaign=share_via&utm_content=profile&utm_medium=ios_api"
          target="_blank"
          >LinkedIn</a
        >,
      </p>
    </footer>
  </body>
</html>
