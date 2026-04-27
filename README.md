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
background:#0a0a0a;
color:#fff;
scroll-behavior:smooth;
}

/* NAV */
nav{
display:flex;
justify-content:space-between;
padding:15px 30px;
position:fixed;
width:100%;
background:rgba(0,0,0,0.6);
backdrop-filter:blur(10px);
z-index:1000;
}

nav h1{color:#00f0ff;}
nav a{color:#fff;margin-left:15px;text-decoration:none;}

/* HERO */
.hero{
height:100vh;
display:flex;
justify-content:center;
align-items:center;
text-align:center;
background:linear-gradient(45deg,#000,#111);
animation:fadeIn 2s ease-in;
}

.hero h2{
font-size:40px;
animation:slideUp 1.5s ease;
}

.hero p{color:#aaa;margin-top:10px;}

.btn{
margin-top:20px;
padding:12px 25px;
border:none;
border-radius:30px;
cursor:pointer;
background:#00f0ff;
color:black;
box-shadow:0 0 20px #00f0ff;
transition:0.3s;
}

.btn:hover{transform:scale(1.1);}

/* SECTION */
section{padding:80px 20px;text-align:center;}

/* SERVICES */
.grid{
display:grid;
grid-template-columns:repeat(auto-fit,minmax(250px,1fr));
gap:20px;
margin-top:30px;
}

.card{
background:#1a1a1a;
padding:25px;
border-radius:15px;
transition:0.3s;
}

.card:hover{
background:#00f0ff;
color:black;
transform:translateY(-10px);
}

/* PRICING */
.price{
font-size:20px;
margin-top:10px;
color:#00f0ff;
}

/* CONTACT */
.contact a{display:block;margin-top:10px;color:#00f0ff;}

/* BOOKING */
input,textarea{
width:90%;
padding:10px;
margin:10px;
border:none;
border-radius:10px;
}

footer{
background:#111;
padding:15px;
}

/* ANIMATION */
@keyframes fadeIn{
from{opacity:0;}
to{opacity:1;}
}

@keyframes slideUp{
from{transform:translateY(50px);opacity:0;}
to{transform:translateY(0);opacity:1;}
}
</style>
</head>

<body>

<nav>
<h1>Plaban Edits</h1>
<div>
<a href="#">Home</a>
<a href="#services">Services</a>
<a href="#pricing">Pricing</a>
<a href="#contact">Contact</a>
</div>
</nav>

<!-- HERO -->
<section class="hero">
<div>
<h2>🎬 Cinematic Video Editing & Premium Content Creation</h2>
<p>Professional • Trusted • High Quality Editing</p>
<button class="btn" onclick="scrollToContact()">Hire Me</button>
</div>
</section>

<!-- SERVICES -->
<section id="services">
<h2>🔥 My Services</h2>

<div class="grid">

<div class="card">
<h3>Cinematic Shoot + Edit</h3>
<p>Full video shoot + cinematic editing</p>
</div>

<div class="card">
<h3>Cinematic Editing</h3>
<p>Film look color grading & transitions</p>
</div>

<div class="card">
<h3>Reels Editing</h3>
<p>Viral reels & shorts editing</p>
</div>

<div class="card">
<h3>Photo Editing</h3>
<p>Lightroom style professional edit</p>
</div>

<div class="card">
<h3>Premium Editing</h3>
<p>High-end effects & storytelling</p>
</div>

</div>
</section>

<!-- PRICING -->
<section id="pricing">
<h2>💰 Pricing Plans</h2>

<div class="grid">

<div class="card">
<h3>Basic</h3>
<p>Reels Editing</p>
<div class="price">₹300 - ₹800</div>
</div>

<div class="card">
<h3>Standard</h3>
<p>Cinematic Editing</p>
<div class="price">₹800 - ₹2000</div>
</div>

<div class="card">
<h3>Pro</h3>
<p>Shoot + Edit</p>
<div class="price">₹1500 - ₹3000</div>
</div>

<div class="card">
<h3>Premium</h3>
<p>High-End Editing</p>
<div class="price">₹2000 - ₹5000</div>
</div>

</div>
</section>

<!-- BOOKING -->
<section>
<h2>📩 Book Your Project</h2>

<input type="text" placeholder="Your Name">
<input type="text" placeholder="Mobile Number">
<textarea placeholder="Project Details"></textarea>

<br>
<button class="btn">Submit</button>

</section>

<!-- CONTACT -->
<section id="contact" class="contact">
<h2>📞 Contact Me</h2>

<p>✅ 100% Trusted Service</p>

<a href="https://wa.me/919332160383" target="_blank">📱 WhatsApp: 9332160383</a>
<a href="https://instagram.com/6x_alive" target="_blank">📷 Instagram: @6x_alive</a>

<p>💳 UPI: plaban4@ptyes</p>

<button class="btn" onclick="openUPI()">Pay Now</button>
</section>

<footer>
<p>© 2026 Plaban Edits | All Rights Reserved</p>
</footer>

<script>
function scrollToContact(){
document.getElementById("contact").scrollIntoView({behavior:"smooth"});
}

function openUPI(){
alert("Send payment to UPI: plaban4@ptyes");
}
</script>

</body>
</html>
