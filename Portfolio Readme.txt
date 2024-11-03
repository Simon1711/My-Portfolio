

<!DOCTYPE html>
<html lang="en">
<head>
  <title>My Portfolio</title>
  <link rel="stylesheet" href="styles.css">
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <link rel="preconnect" href="https://fonts.googleapis.com">
<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
<link href="https://fonts.googleapis.com/css2?family=Itim&family=Kanit:ital,wght@0,100;0,200;0,300;0,400;0,500;0,600;0,700;0,800;0,900;1,100;1,200;1,300;1,400;1,500;1,600;1,700;1,800;1,900&display=swap" rel="stylesheet">
<link href="https://fonts.googleapis.com/css2?family=Playfair+Display:ital@1&display=swap" rel="stylesheet">
<link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0-beta3/css/all.min.css">
</head>
<body>
 <nav id="navbar">
  <ul id="nav-list">
    <li><a href="#welcome-section">Welcome</a></li>
    <li><a href="#projects">Projects</a></li>
    <li><a href="#contact">Contact</a></li>
  </ul>
</nav>
<section id="welcome-section">
  <h1>Welcome to My Portfolio</h1>
  <p>This is a brief introduction about myself and my work.</p>
</section>
<section id="projects" class="projects">
<h2>My Projects</h2>
<div class="project-grid">
    <div class="project">
      <a href="https://github.com/Simon1711/My-Fitness-Survey-Form" class="project-link">
      <img src="https://github.com/Simon1711/My-Fitness-Survey-Form/blob/main/Fitness%20survey%20form%20image.jpg?raw=true" alt="My Fitness Survey Form" class="project-img">
      <p class="project-tile">Fitness Survey Form</p>
      </a>
    </div>
    <div class="project">
      <a href="https://github.com/Simon1711/Grumpy-cat-tribute-page" class="project-link">
      <img src="https://github.com/Simon1711/Grumpy-cat-tribute-page/blob/main/Grumpy%20Cat%20Image.jpg?raw=true" alt="My Fitness Survey Form" class="project-img">
      <p class="project-tile">Grumpy Cat Tribute Page</p>
      </a>
    </div>
    <div class="project">
      <a href="https://github.com/Simon1711/HTML-Technical-Documentation-Page" class="project-link">
      <img src="https://github.com/Simon1711/HTML-Technical-Documentation-Page/blob/main/HTML%20Documentation%20Image.jpg?raw=true" alt="My Fitness Survey Form" class="project-img">
      <p class="project-tile">HTML Documentation Page</p>
      </a>
    </div>
  <div class="project">
     <a href="https://github.com/Simon1711/Nintendo-Consoles-Landing-Page" class="project-link">
      <img src="https://github.com/Simon1711/Nintendo-Consoles-Landing-Page/blob/main/Nintendo%20Consoles%20Image.jpg?raw=true" alt="My Fitness Survey Form" class="project-img">
      <p class="project-tile">Nintendo Consoles Features</p>
      </a>
    </div>
  </div>
</section>
<section id="contact" class="contact">
<div id="contact-header">
<h2>I'd Love to Hear from You!</h2>
<p>Your feedback is important to me. How can I assist you today?</p>
  </div>
  <div id="contact-links">
<a href="https://github.com/Simon1711" id="profile-link" class="contact-link" target="_blank"><i class="fab fa-github"></i> GitHub</a>
<a href="https://www.facebook.com/simon.nasrallah/" target="_blank" class="contact-link">
      <i class="fab fa-facebook-square"></i> Facebook
    </a>
<a href="mailto:nasrallahsimon4@gmail.com" class="contact-link">
      <i class="fas fa-envelope"></i> Email Me
    </a>
<a href="https://wa.me/15147145655" target="_blank" class="contact-link">
  <i class="fab fa-whatsapp"></i> WhatsApp
</a>
    </div>
  </section>
</body>
  </html>




CSS:


* {
  box-sizing: border-box;
}


body {
  font-family: "Kanit", sans-serif;
  margin: 0;
  padding: 0;
}

#navbar {
  background-color: #243447; 
  position: fixed; 
  width: 100%;
  top: 0;
  left: 0; 
   z-index: 1000;
  display: flex;
  justify-content: center
}

#nav-list {
  display: flex;
  flex-direction: row;  
}

li {
  list-style: none;
   margin: 0;
}
a {
  color: yellow;
  text-decoration: none;
  font-size: 1.4em;
  padding: 1rem 1rem
}
#navbar a:hover {
  background-color: #3b5998; 
  color: white; 
}
#welcome-section {
  width: 100%;
  height: 70vh;
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
  background: linear-gradient(135deg, #1b1f3b, #282f58, #004d7a);
}

h1 {
  color: yellow;
  font-size: 2.5rem;
  font-weight: 800;
   margin-bottom: 0.5rem;
}

#welcome-section p {
  color: #b0c4de;
  font-family: 'Playfair Display', serif;
  font-style: italic;
  font-weight: 200;
  margin-top: 0;
}
.projects {
  text-align: center;
  background: linear-gradient(135deg, #3a4a6b, #466487, #527fa3);
  padding: 50px 20px;
}
.projects > h2 {
  color: yellow;
  font-size: 2.5rem;
  margin-top: 1px;
}
.project-img {
  height: calc(100% - 5.8rem);
  width: 100%;
  object-fit: cover; 
}
.project-tile {
  color: white;
  background-color: rgba(0, 0, 0, 0.6);
   font-weight: bold;
   width: 100%;
   margin: -0.55rem 1rem;
   padding: 1rem 0;
   font-size: 18px
}
.project-grid {
  display: grid;
grid-template-columns: repeat(auto-fit, minmax(220px, 1fr));
  grid-gap: 3rem;
  width: 100%;
  max-width: 1280px;
  margin: 0 auto;
  margin-bottom: 3rem;
}
.project:hover .project-tile {
  color: yellow; 
}
.project-tile {
  transition: color 0.3s ease; 
}
#contact {
  background: linear-gradient(135deg, #1b1f3b, #282f58, #004d7a);
  width: 100%;
  height: 70vh;
  padding: 1rem 2rem;
  display: flex;
  justify-content: center;
  flex-direction: column;
  align-items: center;
}
#contact h2 {
  color: yellow; 
  font-size: 2.5rem;
  margin-bottom: 0
}
#contact p {
  color: #b0c4de;
  font-style: italic;
  font-weight: 300;
  text-align: center;
  font-size: 1rem;
  margin-bottom: 1.5rem
}
@media (max-width: 800px) {
  h1 {font-size: 2rem
  }
}
#contact-links {
  display: flex;
  gap: 1rem; 
}
.contact-link:hover {
  background-color: #1d3b67; 
  transform: translateY(6px);
  border-radius: 5px 
}
.contact-link {
   transition: transform 0.5s ease, background-color 0.5s;
}



