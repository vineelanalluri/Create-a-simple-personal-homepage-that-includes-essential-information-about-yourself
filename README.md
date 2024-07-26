# Create-a-simple-personal-homepage-that-includes-essential-information-about-yourself
<!DOCTYPE html>
<html lang="en">
<head>
<title>Vineela Nalluri</title>
<link rel="stylesheet" href="styles.css">
</head>
<body>
<header>
<div class="container">
<h1>Vineela Nalluri</h1>
<nav>
<ul>
<li><a href="#about" onclick="showSection('about')">About Me</a></li>
<li><a href="#portfolio" onclick="showSection('portfolio')">Portfolio</a></li>
<li><a href="#skills" onclick="showSection('skills')">Skills</a></li>
<li><a href="#contact" onclick="showSection('contact')">Contact</a></li>
</ul>
</nav>
</div>
</header>
<h2>This is my personal homepage.</h2>
<img src="https://d1csarkz8obe9u.cloudfront.net/posterpreviews/welcome-home-design-template-942174bf76bf88a08f54bee7d76c6504_screen.jpg?ts=1683765314" alt="Default Image" id="default-image">
<main>
<div class="section" id="about">
<div class="container">
<h1>About Me</h1>
<p>My name is Vineela Nalluri</p>
<p>My father name is VenkataSubbaiah Nalluri</p>
<p>My mother name is Anuradha Nalluri</p>
<p>I am from Ongole</p>
<p>I am a STUDENT</p>
<p>I am pursuing graduation at Qis college of Engineering and Technology|| Cyber Security</p>

</div>
</div>
<div class="section" id="portfolio">
<div class="container">
<h1>Portfolio</h1>
<p>I have done a internship of Python .</p>
</div>
</div>
<div class="section" id="skills">
<div class="container">
<h1>Skills</h1>
<h3>Qualifications:</h3>
<p>I am studying III B.Tech in QIS College of Engineering and Technology, Ongole.</p>
<p>I have completed my Intermediate in Sri Chaitanya Junior College,Ongole.</p>
<p>I have completed my schooling in Sivani High School, Ongole.</p>
<p>I have some basic knowledge of coding languages like HTML, CSS, JAVA, JS, PYTHON, C</p>
<p>I learnt the coding languages and certified by known platforms like GreatLearning, LinkedIn Learning, Sololearn, etc.</p>
</div>
</div>
<div class="section" id="contact">
<div class="container">
<h1>Contact</h1>
<h2>Via</h2>
<a href="https://www.linkedin.com/in/vinni-nalluri-725923290?utm_source=share&utm_campaign=share_via&utm_content=profile&utm_medium=android_app" target="_blank"><i class="fab fa-linkedin"></i>LinkedIn</a>
<a href="https://www.instagram.com/" target="_blank"><i class="fab fa-instagram"></i>Instagram</a>
<a href="https://wa.me/qr/K2AC6U2WEL33B1" target="_blank"><i class="fab fa-whatsapp"></i>WhatsApp</a>
<a href="vinninalluri@gmail.com"><i class="fas fa-envelope"></i>Email</a>
</div>
</div>
</main>
<footer>
<div class="container">
<p>Follow me on social media:</p>
<a href="https://www.linkedin.com/in/vinni-nalluri-725923290?utm_source=share&utm_campaign=share_via&utm_content=profile&utm_medium=android_app" target="_blank"><i class="fab fa-linkedin"></i>LinkedIn</a>
<a href="https://www.instagram.com/" target="_blank"><i class="fab fa-instagram"></i>Instagram</a>
<a href="https://wa.me/qr/K2AC6U2WEL33B1" target="_blank"><i class="fab fa-whatsapp"></i>WhatsApp</a>
<a href="vinninalluri@gmail.com"><i class="fas fa-envelope"></i>Email</a>
</div>
</footer>
<script>
    function showSection(sectionId) {
        const sections = document.querySelectorAll('.section');
        sections.forEach(section => {
            section.style.display = 'none';
        });

        const activeSection = document.getElementById(sectionId);
        activeSection.style.display = 'block';

        // Hide default image when a section is shown
        document.getElementById('default-image').style.display = 'none';
    }

    document.addEventListener('DOMContentLoaded', () => {
        // No section is shown by default
        document.querySelectorAll('.section').forEach(section => {
            section.style.display = 'none';
        });
    });
</script>
</body>
</html>

#css

body {
    font-family:sans-serif;
    margin: 5px;
    padding: 5px;
    background-color: rgb(30, 210, 108);
    color: #d31473;
    display: flex;
    flex-direction: column;
    align-items: center;
    min-height: 100vh;
}
.container {
    width: 80%;
    margin: auto;
    overflow: hidden;
}
header {
    background: #d60c85;
    color: #010f13;
    padding-top: 30px;
    min-height: 70px;
    border-bottom: #c3d1d1 15px solid;
    width: 100%;
}
header h1 {
    text-align: center;
    margin: 5px;
}
header nav {
    text-align: center;
    margin-top: 10px;
}
header nav ul {
    padding: 0;
    list-style: none;
}
header nav ul li {
    display: inline;
    margin: 15px;
}
header nav ul li a {
    color: #fff;
    text-decoration: none;
    text-transform: uppercase;
    font-size: 16px;
    padding: 10px 20px;
    border-radius: 25px;
    background: rgba(108, 5, 43, 0.1);
    border: 2px solid transparent;
    transition: background 0.3s, transform 0.3s, color 0.3s, border-color 0.3s;
}
header nav ul li a:hover {
    background: rgb(222, 11, 148);
    color: red;
    border-color: rgb(7, 70, 70);
    transform: scale(1.1);
}
h2 {
    background: #fff;
    font-style: italic;
    font-family:   'Lucida Grande', 'Lucida Sans Unicode', Geneva, Verdana, sans-serif;
    width: 500px;
    height: 50px;
    border-radius: 10px;
    text-align: center;
    margin: 20px ;
}
#default-image {
    display: block;
    width: 500px;
    height: auto;
    margin: 20px ;
}
main {
    flex-grow: 1;
    width: 100%;
    display: flex;
    flex-direction: column;
    align-items: center;
    margin-bottom: 20px; 
}
.section {
    display: none;
    padding: 20px 0;
    background: #fff;
    margin: 20px 0;
    border-radius: 25px;
    width: 700px;
    text-align: center;
    transition: background-color 0.5s, color 0.5s;
}
.section h1, .section h2 {
    text-align: center;
    margin: 0 0 10px 0;
}
.section p {
    text-align: center;
    line-height: 1.6;
}
.section a {
    color: #0f63a8;
    text-align: center;
}
.social {
    text-align: center;
    padding: 20px;
}
.social a {
    margin: 0 10px;
    text-decoration: none;
    color: #333;
    font-size: 20px;
}
.social i {
    margin-right: 8px;
}
footer {
    text-align: center;
    padding: 20px 0;
    background: #333;
    color: #fff;
    width: 100%;
    position: relative;
}
footer a {
    color: aliceblue;
}
