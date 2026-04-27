# PlabanEditzz
<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">

<title>Plaban Edits | Cinematic Editor</title>

<link href="https://fonts.googleapis.com/css2?family=Poppins:wght@300;500;700&display=swap" rel="stylesheet">

<style>
*{margin:0;padding:0;box-sizing:border-box;font-family:'Poppins',sans-serif;}

body{
background:#0b0f1a;
color:#fff;
overflow-x:hidden;
padding-top:80px;
}

/* NAVBAR */
nav{
position:fixed;
top:0;
width:100%;
display:flex;
justify-content:space-between;
align-items:center;
padding:15px 25px;
background:rgba(10,15,30,0.8);
backdrop-filter:blur(12px);
z-index:1000;
border-bottom:1px solid rgba(255,255,255,0.1);
}

nav h1{
background:linear-gradient(45deg,#00f0ff,#ff00c8);
-webkit-background-clip:text;
color:transparent;
font-size:20px;
}

nav a{
color:#fff;
margin-left:15px;
text-decoration:none;
font-size:14px;
}

/* HERO */
.hero{
height:100vh;
display:flex;
justify-content:center;
align-items:center;
text-align:center;
flex-direction:column;
background:linear-gradient(120deg,#000,#0b0f1a,#000);
animation:bgMove 10s infinite linear;
}

.hero h2{
font-size:36px;
background:linear-gradient(45deg,#00f0ff,#ff00c8);
-webkit-background-clip:text;
color:transparent;
animation:fadeUp 1.5s ease;
}

.hero p{
margin-top:10px;
color:#aaa;
}

.btn{
margin-top:20px;
padding:12px 25px;
border:none;
border-radius:30px;
background:linear-gradient(45deg,#00f0ff,#ff00c8);
color:white;
cursor:pointer;
transition:0.3s;
box-shadow:0 0 15px #00f0ff;
}

.btn:hover{
transform:scale(1.1);
}

/* SECTION */
section{
padding:70px 20px;
text-align:center;
}

/* SERVICES */
.grid{
display:grid;
grid-template-columns:repeat(auto-fit,minmax(250px,1fr));
gap:20px;
margin-top:30px;
}

.card{
background:rgba(255,255,255,0.05);
padding:25px;
border-radius:15px;
transition:0.4s;
opacity:0;
transform:translateY(40px);
}

.card:hover{
transform:translateY(-10px);
background:rgba(255,255,255,0.08);
box-shadow:0 0 25px #00f0ff33;
}

.price{
color:#00f0ff;
margin-top:10px;
font-weight:bold;
}

/* PORTFOLIO */
.portfolio p{
margin-top:20px;
color:#aaa;
}

/* CONTACT */
.contact a{
display:block;
margin-top:10px;
color:#00f0ff;
}

/* FOOTER */
footer{
background:#111;
padding:15px;
font-size:14px;
}

/* ANIMATION */
@keyframes fadeUp{
from{opacity:0;transform:translateY(30px);}
to{opacity:1;transform:translateY(0);}
}

@keyframes bgMove{
0%{background-position:0%;}
100%{background-position:100%;}
}
</style>
</head>

<body>

<!-- NAV -->
<nav>
<h1>Plaban Edits</h1>
<div>
<a href="#">Home</a>
<a href="#services">Services</a>
<a href="#portfolio">Work</a>
<a href="#contact">Contact</a>
</div>
</nav>

<!-- HERO -->
<section class="hero">
<h2>🎬 Cinematic Editing That Feels Premium</h2>
<p>Creative • Professional • 100% Trusted</p>
<button class="btn" onclick="scrollToContact()">Hire Me</button>
</section>

<!-- SERVICES -->
<section id="services">
<h2>🔥 My Services</h2>

<div class="grid">

<div class="card">
<h3>🎬 Shoot + Edit</h3>
<p>Full cinematic production</p>
<div class="price">₹1500 – ₹3000</div>
</div>

<div class="card">
<h3>🎞️ Cinematic Edit</h3>
<p>Film look editing</p>
<div class="price">₹800 – ₹2000</div>
</div>

<div class="card">
<h3>📱 Reels Editing</h3>
<p>Viral short content</p>
<div class="price">₹300 – ₹800</div>
</div>

<div class="card">
<h3>📸 Photo Edit</h3>
<p>Lightroom style</p>
<div class="price">₹100 – ₹500</div>
</div>

<div class="card">
<h3>💎 Premium Edit</h3>
<p>High-end storytelling</p>
<div class="price">₹2000 – ₹5000</div>
</div>

<div class="card">
<h3>⚡ Custom Project</h3>
<p>Custom work</p>
<div class="price">DM for price</div>
</div>

</div>

<p style="margin-top:30px;">
✅ 100% Trusted • ⚡ Fast Delivery • 🎬 Pro Quality
</p>

</section>

<!-- PORTFOLIO -->
<section id="portfolio" class="portfolio">
<h2>🎥 My Work</h2>

<p>High-quality cinematic projects will be showcased here soon.</p>

<button class="btn" onclick="scrollToContact()">Work With Me</button>

</section>

<!-- CONTACT -->
<section id="contact" class="contact">
<h2>📞 Contact</h2>

<p>✅ 100% Trusted Service</p>

<a href="https://wa.me/919332160383" target="_blank">📱 WhatsApp: 9332160383</a>
<a href="https://instagram.com/6x_alive" target="_blank">📷 Instagram: @6x_alive</a>

</section>

<!-- FOOTER -->
<footer>
<p>© 2026 Plaban Edits</p>
</footer>

<script>
// scroll animation
const cards = document.querySelectorAll('.card');

window.addEventListener('scroll', ()=>{
cards.forEach(card=>{
if(card.getBoundingClientRect().top < window.innerHeight - 50){
card.style.opacity = "1";
card.style.transform = "translateY(0)";
}
});
});

function scrollToContact(){
document.getElementById("contact").scrollIntoView({behavior:"smooth"});
}
</script>

</body>
</html>
