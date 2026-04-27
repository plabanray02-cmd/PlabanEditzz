# PlabanEditzz
<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">

<title>Plaban Edits | Cinematic Editor</title>

<link href="https://fonts.googleapis.com/css2?family=Poppins:wght@300;500;600&display=swap" rel="stylesheet">

<style>
*{margin:0;padding:0;box-sizing:border-box;font-family:'Poppins',sans-serif;}

body{
background:#0b0f1a;
color:#fff;
padding-top:80px;
}

/* NAV */
nav{
position:fixed;
top:0;
width:100%;
display:flex;
justify-content:space-between;
align-items:center;
padding:12px 25px;
background:rgba(10,15,30,0.8);
backdrop-filter:blur(12px);
z-index:1000;
}

nav h1{
font-size:18px;
background:linear-gradient(45deg,#00f0ff,#ff00c8);
-webkit-background-clip:text;
color:transparent;
}

nav a{
font-size:13px;
margin-left:15px;
color:#fff;
text-decoration:none;
}

/* HERO */
.hero{
position:relative;
height:100vh;
display:flex;
justify-content:center;
align-items:center;
text-align:center;
overflow:hidden;
}

.bg-video{
position:absolute;
width:100%;
height:100%;
object-fit:cover;
z-index:-1;
filter:brightness(40%);
}

.hero h2{
font-size:28px;
line-height:1.4;
}

.hero p{
font-size:14px;
color:#ccc;
margin-top:10px;
}

.btn{
margin-top:15px;
padding:10px 20px;
border:none;
border-radius:30px;
background:linear-gradient(45deg,#00f0ff,#ff00c8);
color:white;
font-size:13px;
cursor:pointer;
}

/* SECTION */
section{
padding:60px 20px;
max-width:1100px;
margin:auto;
}

/* GRID */
.grid{
display:grid;
grid-template-columns:repeat(auto-fit,minmax(220px,1fr));
gap:15px;
margin-top:25px;
}

/* CARD */
.card{
background:rgba(255,255,255,0.05);
padding:18px;
border-radius:12px;
transition:0.3s;
opacity:0;
transform:translateY(30px);
}

.card:hover{
transform:translateY(-6px);
box-shadow:0 0 20px #00f0ff33;
}

.card h3{
font-size:15px;
}

.card p{
font-size:13px;
color:#aaa;
margin-top:5px;
}

.price{
font-size:13px;
color:#00f0ff;
margin-top:8px;
}

/* CONTACT */
.contact a{
display:block;
margin-top:8px;
font-size:14px;
color:#00f0ff;
}

/* FLOAT BUTTON */
.whatsapp{
position:fixed;
bottom:20px;
right:20px;
background:#25D366;
padding:12px;
border-radius:50%;
font-size:18px;
color:#fff;
}

/* FOOTER */
footer{
background:#111;
padding:12px;
text-align:center;
font-size:13px;
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
<a href="#reels">Reels</a>
<a href="#contact">Contact</a>
</div>
</nav>

<!-- HERO -->
<section class="hero">
<video autoplay muted loop playsinline class="bg-video">
<source src="your-video.mp4" type="video/mp4">
</video>

<div>
<h2>Cinematic Editing That Feels Premium</h2>
<p>Professional editing for reels, videos & photos</p>
<button class="btn" onclick="scrollToContact()">Hire Me</button>
</div>
</section>

<!-- SERVICES -->
<section id="services">
<h2>My Services</h2>

<div class="grid">

<div class="card"><h3>Shoot + Edit</h3><p>Full cinematic production</p><div class="price">₹1500–3000</div></div>

<div class="card"><h3>Cinematic Edit</h3><p>Film style editing</p><div class="price">₹800–2000</div></div>

<div class="card"><h3>Reels Editing</h3><p>Trending short videos</p><div class="price">₹300–800</div></div>

<div class="card"><h3>Photo Edit</h3><p>Lightroom style</p><div class="price">₹100–500</div></div>

<div class="card"><h3>Premium Edit</h3><p>High-end storytelling</p><div class="price">₹2000–5000</div></div>

</div>
</section>

<!-- WHY CHOOSE -->
<section>
<h2>Why Choose Me</h2>

<div class="grid">

<div class="card"><h3>Fast Delivery</h3><p>Quick turnaround</p></div>
<div class="card"><h3>Cinematic Quality</h3><p>Pro level editing</p></div>
<div class="card"><h3>Easy Contact</h3><p>WhatsApp & Instagram</p></div>
<div class="card"><h3>Trusted</h3><p>100% client focus</p></div>

</div>
</section>

<!-- REELS -->
<section id="reels">
<h2>Reels Preview</h2>

<div class="grid">

<div class="card">
<video controls width="100%">
<source src="reel1.mp4" type="video/mp4">
</video>
</div>

<div class="card">
<video controls width="100%">
<source src="reel2.mp4" type="video/mp4">
</video>
</div>

</div>
</section>

<!-- CONTACT -->
<section id="contact" class="contact">
<h2>Contact</h2>

<a href="https://wa.me/919332160383" target="_blank">WhatsApp: 9332160383</a>
<a href="https://instagram.com/6x_alive" target="_blank">Instagram: @6x_alive</a>

</section>

<!-- FLOAT BUTTON -->
<a href="https://wa.me/919332160383" class="whatsapp" target="_blank">💬</a>

<footer>
<p>© 2026 Plaban Edits</p>
</footer>

<script>
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
