# PlabanEditzz
<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Plaban Edits | Ultra Pro</title>

<link href="https://fonts.googleapis.com/css2?family=Poppins:wght@300;500;700&display=swap" rel="stylesheet">

<style>
*{margin:0;padding:0;box-sizing:border-box;font-family:'Poppins',sans-serif;}

body{
background:#0b0f1a;
color:#fff;
overflow-x:hidden;
}

/* NAV */
nav{
display:flex;
justify-content:space-between;
padding:15px 30px;
position:fixed;
width:100%;
background:rgba(0,0,0,0.4);
backdrop-filter:blur(10px);
z-index:1000;
}

nav h1{
background:linear-gradient(45deg,#00f0ff,#ff00c8);
-webkit-background-clip:text;
color:transparent;
}

nav a{color:#fff;margin-left:15px;text-decoration:none;}

/* HERO VIDEO */
.hero{
position:relative;
height:100vh;
display:flex;
justify-content:center;
align-items:center;
text-align:center;
overflow:hidden;
}

.hero video{
position:absolute;
width:100%;
height:100%;
object-fit:cover;
z-index:-1;
filter:brightness(40%);
}

.hero h2{
font-size:45px;
background:linear-gradient(45deg,#00f0ff,#ff00c8);
-webkit-background-clip:text;
color:transparent;
animation:fadeUp 1.5s ease;
}

.btn{
margin-top:20px;
padding:12px 25px;
border:none;
border-radius:30px;
cursor:pointer;
background:linear-gradient(45deg,#00f0ff,#ff00c8);
color:white;
box-shadow:0 0 20px #00f0ff;
transition:0.3s;
}

.btn:hover{transform:scale(1.1);}

/* SECTION */
section{padding:80px 20px;text-align:center;}

/* GRID */
.grid{
display:grid;
grid-template-columns:repeat(auto-fit,minmax(250px,1fr));
gap:20px;
margin-top:30px;
}

/* CARD */
.card{
background:rgba(255,255,255,0.05);
backdrop-filter:blur(10px);
padding:25px;
border-radius:20px;
transition:0.3s;
opacity:0;
transform:translateY(40px);
}

.card.show{
opacity:1;
transform:translateY(0);
}

.card:hover{
transform:translateY(-10px);
background:linear-gradient(45deg,#00f0ff33,#ff00c833);
}

/* SLIDER */
.slider{
overflow:hidden;
margin-top:30px;
}

.slide-track{
display:flex;
width:calc(300px * 6);
animation:scroll 15s linear infinite;
}

.slide img{
width:300px;
height:200px;
border-radius:15px;
margin:10px;
}

@keyframes scroll{
0%{transform:translateX(0);}
100%{transform:translateX(-50%);}
}

/* CONTACT */
.contact a{
display:block;
margin-top:10px;
color:#00f0ff;
}

footer{
background:#111;
padding:15px;
}

@keyframes fadeUp{
from{opacity:0;transform:translateY(40px);}
to{opacity:1;transform:translateY(0);}
}
</style>
</head>

<body>

<nav>
<h1>Plaban Edits</h1>
<div>
<a href="#">Home</a>
<a href="#services">Services</a>
<a href="#portfolio">Work</a>
<a href="#contact">Contact</a>
</div>
</nav>

<!-- HERO VIDEO -->
<section class="hero">
<video autoplay muted loop>
<source src="https://www.w3schools.com/howto/rain.mp4" type="video/mp4">
</video>

<div>
<h2>🎬 Cinematic Editing That Feels Like Movie</h2>
<p>Premium • Creative • 100% Trusted</p>
<button class="btn" onclick="scrollToContact()">Hire Me</button>
</div>
</section>

<!-- SERVICES -->
<section id="services">
<h2>🔥 Services</h2>

<div class="grid">
<div class="card">Cinematic Shoot + Edit</div>
<div class="card">Cinematic Editing</div>
<div class="card">Reels Editing</div>
<div class="card">Photo Editing</div>
<div class="card">Premium Editing</div>
</div>

</section>

<!-- PORTFOLIO SLIDER -->
<section id="portfolio">
<h2>🎥 My Work</h2>

<div class="slider">
<div class="slide-track">

<div class="slide"><img src="https://images.unsplash.com/photo-1492724441997-5dc865305da7"></div>
<div class="slide"><img src="https://images.unsplash.com/photo-1500530855697-b586d89ba3ee"></div>
<div class="slide"><img src="https://images.unsplash.com/photo-1526178613658-3f1622045557"></div>

<div class="slide"><img src="https://images.unsplash.com/photo-1492724441997-5dc865305da7"></div>
<div class="slide"><img src="https://images.unsplash.com/photo-1500530855697-b586d89ba3ee"></div>
<div class="slide"><img src="https://images.unsplash.com/photo-1526178613658-3f1622045557"></div>

</div>
</div>

</section>

<!-- CONTACT -->
<section id="contact" class="contact">
<h2>📞 Contact</h2>

<p>✅ 100% Trusted Service</p>

<a href="https://wa.me/919332160383" target="_blank">WhatsApp: 9332160383</a>
<a href="https://instagram.com/6x_alive" target="_blank">Instagram: @6x_alive</a>

</section>

<footer>
<p>© 2026 Plaban Edits</p>
</footer>

<script>
// SCROLL ANIMATION
const cards = document.querySelectorAll('.card');

window.addEventListener('scroll', ()=>{
cards.forEach(card=>{
const top = card.getBoundingClientRect().top;
if(top < window.innerHeight - 50){
card.classList.add('show');
}
});
});

function scrollToContact(){
document.getElementById("contact").scrollIntoView({behavior:"smooth"});
}
</script>

</body>
</html>
