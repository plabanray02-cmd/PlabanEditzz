# PlabanEditzz
<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Plaban Edits</title>

<link href="https://fonts.googleapis.com/css2?family=Poppins:wght@300;500;700&display=swap" rel="stylesheet">

<style>
*{
margin:0;
padding:0;
box-sizing:border-box;
font-family:'Poppins', sans-serif;
}

body{
background:#0f0f0f;
color:#fff;
overflow-x:hidden;
}

/* NAVBAR */
nav{
display:flex;
justify-content:space-between;
padding:20px 50px;
position:fixed;
width:100%;
background:rgba(0,0,0,0.6);
backdrop-filter:blur(10px);
}

nav h1{
color:#00f0ff;
}

nav a{
color:white;
margin-left:20px;
text-decoration:none;
}

/* HERO */
.hero{
height:100vh;
display:flex;
justify-content:center;
align-items:center;
text-align:center;
background:linear-gradient(to right,#000,#111);
}

.hero h2{
font-size:50px;
}

.hero p{
margin-top:10px;
color:#aaa;
}

.btn{
margin-top:20px;
padding:12px 25px;
background:#00f0ff;
color:black;
border:none;
cursor:pointer;
border-radius:30px;
}

/* SERVICES */
.services{
padding:80px 50px;
text-align:center;
}

.service-box{
display:grid;
grid-template-columns:repeat(auto-fit,minmax(250px,1fr));
gap:30px;
margin-top:40px;
}

.card{
background:#1a1a1a;
padding:30px;
border-radius:20px;
transition:0.3s;
}

.card:hover{
transform:translateY(-10px);
background:#00f0ff;
color:black;
}

/* PORTFOLIO */
.portfolio{
padding:80px 50px;
text-align:center;
}

.video-box{
margin-top:30px;
}

/* CONTACT */
.contact{
padding:80px 50px;
text-align:center;
}

footer{
text-align:center;
padding:20px;
background:#111;
}
</style>
</head>

<body>

<nav>
<h1>Plaban Edits</h1>
<div>
<a href="#">Home</a>
<a href="#services">Services</a>
<a href="#portfolio">Portfolio</a>
<a href="#contact">Contact</a>
</div>
</nav>

<section class="hero">
<div>
<h2>Professional Video & Photo Editing</h2>
<p>Cinematic • Reels • Premium Editing</p>
<button class="btn">Hire Me</button>
</div>
</section>

<section id="services" class="services">
<h2>My Services</h2>

<div class="service-box">
<div class="card">
<h3>Cinematic Video Editing</h3>
<p>Movie style color grading & transitions</p>
</div>

<div class="card">
<h3>Reels Editing</h3>
<p>Instagram viral reels & shorts</p>
</div>

<div class="card">
<h3>Photo Editing</h3>
<p>Lightroom style professional retouch</p>
</div>

<div class="card">
<h3>Video Shooting</h3>
<p>Camera setup, lighting & full production</p>
</div>
</div>
</section>

<section id="portfolio" class="portfolio">
<h2>My Work</h2>

<div class="video-box">
<iframe width="300" height="200" src="https://www.youtube.com/embed/YOUR_VIDEO"></iframe>
</div>
</section>

<section id="contact" class="contact">
<h2>Contact Me</h2>
<p>WhatsApp: 1234567890</p>
<p>Email: your@email.com</p>
<button class="btn">Book Now</button>
</section>

<footer>
<p>© 2026 Plaban Edits</p>
</footer>

</body>
</html>
