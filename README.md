<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <meta name="description" content="A personal portfolio website with smooth animations and a contact form.">
    <title>My Portfolio Website</title>
    <link rel="stylesheet" href="style.css">
    <link rel="icon" href="assets/images/favicon.ico">
</head>
<body>

    <header>
        <nav>
            <div class="logo">My Portfolio</div>
            <ul>
                <li><a href="#home">Home</a></li>
                <li><a href="#about">About</a></li>
                <li><a href="#projects">Projects</a></li>
                <li><a href="#contact">Contact</a></li>
            </ul>
        </nav>
    </header>

    <section id="home" class="hero">
        <div class="hero-content">
            <h1>Welcome to My Personal Website</h1>
            <p>Building cool things with code.</p>
            <a href="#about" class="cta-btn">Learn More</a>
        </div>
    </section>

    <section id="about" class="about">
        <h2>About us</h2>
        <p> we are a passionate website who love to help families grow and produce a loving family while also making it a user-friendly website.</p>
        <p>Feel free to check out my work below and get in touch if you're interested in collaborating!</p>
    </section>

    <section id="projects" class="projects">
        <h2>My Projects</h2>
        <div class="project-list">
            <div class="project-item">
                <img src="assets/images/project1.jpg" alt="Project 1">
                <h3>Project 1</h3>
                <p>Description of Project 1</p>
            </div>
            <div class="project-item">
                <img src="assets/images/project2.jpg" alt="Project 2">
                <h3>Project 2</h3>
                <p>Description of Project 2</p>
            </div>
            <div class="project-item">
                <img src="assets/images/project3.jpg" alt="Project 3">
                <h3>Project 3</h3>
                <p>Description of Project 3</p>
            </div>
        </div>
    </section>

    <section id="contact" class="contact">
        <h2>Contact Me</h2>
        <form action="https://formspree.io/f/xjvjqvzo" method="POST">
            <input type="text" name="name" placeholder="Your Name" required>
            <input type="email" name="email" placeholder="Your Email" required>
            <textarea name="message" rows="4" placeholder="Your Message" required></textarea>
            <button type="submit">Send Message</button>
        </form>
    </section>

    <footer>
        <p>&copy; 2025 My Portfolio. All Rights Reserved.</p>
    </footer>

    <script src="script.js"></script>
</body>
</html>

/* General Reset */
* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
}

body {
    font-family: 'Arial', sans-serif;
    line-height: 1.6;
    background-color: #f9f9f9;
}

a {
    text-decoration: none;
    color: inherit;
}

/* Header */
header {
    background: #333;
    color: #fff;
    padding: 20px 0;
    position: fixed;
    width: 100%;
    top: 0;
    left: 0;
    z-index: 1000;
}

nav .logo {
    font-size: 24px;
    font-weight: bold;
    margin-left: 20px;
    float: left;
}

nav ul {
    list-style: none;
    float: right;
    margin-right: 20px;
}

nav ul li {
    display: inline-block;
    margin-left: 20px;
}

nav ul li a {
    color: white;
    font-size: 18px;
    padding: 5px 15px;
    transition: all 0.3s ease;
}

nav ul li a:hover {
    background: #007acc;
    border-radius: 5px;
}

/* Hero Section */
.hero {
    background: #007acc;
    color: white;
    height: 100vh;
    display: flex;
    align-items: center;
    justify-content: center;
    text-align: center;
}

.hero-content h1 {
    font-size: 48px;
    margin-bottom: 10px;
}

.hero-content p {
    font-size: 24px;
    margin-bottom: 20px;
}

.cta-btn {
    background: #fff;
    color: #007acc;
    padding: 15px 30px;
    border-radius: 5px;
    font-size: 18px;
    transition: all 0.3s ease;
}

.cta-btn:hover {
    background: #007acc;
    color: white;
}

/* About Section */
.about {
    padding: 50px;
    text-align: center;
    background-color: #fff;
    margin-top: -20px;
}

.about h2 {
    font-size: 36px;
    margin-bottom: 10px;
}

.about p {
    font-size: 20px;
    margin: 10px 0;
}

/* Projects Section */
.projects {
    background-color: #f4f4f4;
    padding: 50px 20px;
}

.projects h2 {
    text-align: center;
    font-size: 36px;
    margin-bottom: 20px;
}

.project-list {
    display: flex;
    justify-content: space-around;
    gap: 20px;
    flex-wrap: wrap;
}

.project-item {
    background: white;
    border-radius: 8px;
    box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
    width: 30%;
    text-align: center;
    padding: 20px;
}

.project-item img {
    width: 100%;
    border-radius: 8px;
    margin-bottom: 15px;
}

.project-item h3 {
    font-size: 24px;
    margin-bottom: 10px;
}

/* Contact Section */
.contact {
    background-color: #fff;
    padding: 50px 20px;
    text-align: center;
}

.contact h2 {
    font-size: 36px;
    margin-bottom: 20px;
}

.contact form {
    max-width: 600px;
    margin: 0 auto;
}

.contact input,
.contact textarea {
    width: 100%;
    padding: 12px;
    margin: 10px 0;
    border: 1px solid #ccc;
    border-radius: 5px;
    font-size: 16px;
}

.contact button {
    background: #007acc;
    color: white;
    padding: 15px 25px;
    border: none;
    border-radius: 5px;
    font-size: 18px;
    cursor: pointer;
}

.contact button:hover {
    background: #005f8a;
}

/* Footer */
footer {
    background-color: #333;
    color: white;
    text-align: center;
    padding: 20px;
}

// Smooth Scroll for anchor links
document.querySelectorAll('a[href^="#"]').forEach(anchor => {
    anchor.addEventListener('click', function (e) {
        e.preventDefault();

        document.querySelector(this.getAttribute('href')).scrollIntoView({
            behavior: 'smooth',
            block: 'start'
        });
    });
});
