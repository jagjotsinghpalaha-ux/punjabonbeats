<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8" />
<meta name="viewport" content="width=device-width, initial-scale=1.0"/>
<title>PunjabOnBeats - Punjabi Music Platform</title>

<link href="https://fonts.googleapis.com/css2?family=Poppins:wght@300;400;500;600;700;800&display=swap" rel="stylesheet">

<style>
*{
    margin:0;
    padding:0;
    box-sizing:border-box;
    font-family:'Poppins',sans-serif;
}

body{
    background:#0d0d0d;
    color:white;
}

/* Navbar */
nav{
    display:flex;
    justify-content:space-between;
    align-items:center;
    padding:20px 8%;
    background:rgba(0,0,0,0.8);
    backdrop-filter:blur(12px);
    position:fixed;
    width:100%;
    top:0;
    z-index:999;
    border-bottom:1px solid rgba(255,255,255,0.1);
}

.logo{
    font-size:32px;
    font-weight:800;
    color:#ffcc00;
}

.logo span{
    color:#ff2c2c;
}

nav ul{
    display:flex;
    gap:30px;
    list-style:none;
}

nav ul li a{
    text-decoration:none;
    color:white;
    font-weight:500;
    transition:.3s;
}

nav ul li a:hover{
    color:#ffcc00;
}

.nav-buttons button{
    border:none;
    padding:12px 20px;
    border-radius:30px;
    margin-left:10px;
    cursor:pointer;
    font-weight:600;
}

.login{
    background:transparent;
    border:1px solid #ffcc00 !important;
    color:#ffcc00;
}

.signup{
    background:linear-gradient(45deg,#ffcc00,#ff2c2c);
    color:white;
}

/* Hero */
.hero{
    height:100vh;
    background:
    linear-gradient(rgba(0,0,0,.6),rgba(0,0,0,.8)),
    url('https://images.unsplash.com/photo-1493225457124-a3eb161ffa5f?auto=format&fit=crop&w=1600&q=80');
    background-size:cover;
    background-position:center;
    display:flex;
    align-items:center;
    justify-content:center;
    text-align:center;
    padding:0 10%;
}

.hero-content h1{
    font-size:70px;
    font-weight:800;
    margin-bottom:20px;
}

.hero-content span{
    color:#ffcc00;
}

.hero-content p{
    font-size:20px;
    max-width:700px;
    margin:auto;
    color:#ddd;
}

.hero-buttons{
    margin-top:30px;
}

.hero-buttons button{
    padding:16px 35px;
    border:none;
    border-radius:40px;
    font-size:17px;
    cursor:pointer;
    margin:10px;
    font-weight:600;
}

.explore{
    background:linear-gradient(45deg,#ffcc00,#ff2c2c);
    color:white;
}

.premium{
    background:transparent;
    border:2px solid #ffcc00;
    color:#ffcc00;
}

/* Search */
.search-box{
    text-align:center;
    margin:50px auto;
}

.search-box input{
    width:70%;
    padding:18px;
    border:none;
    border-radius:40px;
    background:#1c1c1c;
    color:white;
    font-size:16px;
}

/* Sections */
.section{
    padding:70px 8%;
}

.section-title{
    font-size:38px;
    margin-bottom:30px;
    color:#ffcc00;
}

.cards{
    display:grid;
    grid-template-columns:repeat(auto-fit,minmax(220px,1fr));
    gap:25px;
}

.card{
    background:#171717;
    border-radius:20px;
    overflow:hidden;
    transition:.4s;
    cursor:pointer;
}

.card:hover{
    transform:translateY(-10px);
}

.card img{
    width:100%;
    height:250px;
    object-fit:cover;
}

.card-content{
    padding:20px;
}

.card-content h3{
    margin-bottom:8px;
}

.play-btn{
    background:linear-gradient(45deg,#ffcc00,#ff2c2c);
    border:none;
    width:50px;
    height:50px;
    border-radius:50%;
    color:white;
    margin-top:10px;
    cursor:pointer;
    font-size:20px;
}

/* Categories */
.categories{
    display:flex;
    flex-wrap:wrap;
    gap:15px;
}

.category{
    padding:15px 25px;
    border-radius:40px;
    background:#171717;
    transition:.3s;
    cursor:pointer;
}

.category:hover{
    background:#ffcc00;
    color:black;
}

/* Newsletter */
.newsletter{
    margin:80px 8%;
    background:linear-gradient(45deg,#111,#2a0d0d);
    border-radius:30px;
    padding:60px;
    text-align:center;
}

.newsletter h2{
    font-size:40px;
}

.newsletter input{
    width:60%;
    padding:18px;
    border:none;
    border-radius:40px;
    margin-top:20px;
}

.newsletter button{
    padding:18px 35px;
    border:none;
    border-radius:40px;
    background:linear-gradient(45deg,#ffcc00,#ff2c2c);
    color:white;
    cursor:pointer;
    margin-left:10px;
}

/* Footer */
footer{
    background:#111;
    padding:50px 8%;
    text-align:center;
    border-top:1px solid rgba(255,255,255,0.1);
}

footer h2{
    color:#ffcc00;
    margin-bottom:10px;
}

footer p{
    color:#aaa;
}

@media(max-width:900px){

nav ul{
display:none;
}

.hero-content h1{
font-size:45px;
}

.search-box input{
width:90%;
}

.newsletter input{
width:100%;
margin-bottom:20px;
}

}
</style>
</head>
<body>

<nav>
<div class="logo">Punjab<span>OnBeats</span></div>

<ul>
<li><a href="#">Home</a></li>
<li><a href="#">Trending</a></li>
<li><a href="#">Artists</a></li>
<li><a href="#">Albums</a></li>
<li><a href="#">Premium</a></li>
</ul>

<div class="nav-buttons">
<button class="login">Login</button>
<button class="signup">Sign Up</button>
</div>
</nav>

<section class="hero">
<div class="hero-content">
<h1>Feel The Power Of <span>Punjabi Music</span></h1>
<p>Listen to trending Punjabi songs, top artists, latest albums and experience premium Punjabi vibes only on PunjabOnBeats.</p>

<div class="hero-buttons">
<button class="explore">Explore Songs</button>
<button class="premium">Go Premium</button>
</div>
</div>
</section>

<div class="search-box">
<input type="text" placeholder="Search Punjabi Songs, Artists, Albums...">
</div>

<section class="section">
<h2 class="section-title">🔥 Trending Punjabi Songs</h2>

<div class="cards">

<div class="card">
<img src="https://images.unsplash.com/photo-1516280440614-37939bbacd81" alt="">
<div class="card-content">
<h3>Winning Speech</h3>
<p>Karan Aujla</p>
<button class="play-btn">▶</button>
</div>
</div>

<div class="card">
<img src="https://images.unsplash.com/photo-1493225457124-a3eb161ffa5f" alt="">
<div class="card-content">
<h3>Softly</h3>
<p>Karan Aujla</p>
<button class="play-btn">▶</button>
</div>
</div>

<div class="card">
<img src="https://images.unsplash.com/photo-1501386761578-eac5c94b800a" alt="">
<div class="card-content">
<h3>295</h3>
<p>Sidhu Moosewala</p>
<button class="play-btn">▶</button>
</div>
</div>

<div class="card">
<img src="https://images.unsplash.com/photo-1511379938547-c1f69419868d" alt="">
<div class="card-content">
<h3>Born To Shine</h3>
<p>Diljit Dosanjh</p>
<button class="play-btn">▶</button>
</div>
</div>

</div>
</section>

<section class="section">
<h2 class="section-title">🎧 Music Categories</h2>

<div class="categories">
<div class="category">Romantic</div>
<div class="category">Sad</div>
<div class="category">Lo-Fi</div>
<div class="category">Bhangra</div>
<div class="category">Rap</div>
<div class="category">Workout</div>
<div class="category">Party</div>
</div>
</section>

<section class="section">
<h2 class="section-title">⭐ Top Punjabi Artists</h2>

<div class="cards">

<div class="card">
<img src="https://images.unsplash.com/photo-1500648767791-00dcc994a43" alt="">
<div class="card-content">
<h3>Diljit Dosanjh ✓</h3>
</div>
</div>

<div class="card">
<img src="https://images.unsplash.com/photo-1506794778202-cad84cf45f1d" alt="">
<div class="card-content">
<h3>Sidhu Moosewala ✓</h3>
</div>
</div>

<div class="card">
<img src="https://images.unsplash.com/photo-1504593811423-6dd665756598" alt="">
<div class="card-content">
<h3>Karan Aujla ✓</h3>
</div>
</div>

<div class="card">
<img src="https://images.unsplash.com/photo-1494790108377-be9c29b29330" alt="">
<div class="card-content">
<h3>AP Dhillon ✓</h3>
</div>
</div>

</div>
</section>

<section class="newsletter">
<h2>Get Weekly Punjabi Hits</h2>
<p>Subscribe for latest Punjabi releases & trending songs.</p>

<input type="email" placeholder="Enter Email">
<button>Subscribe</button>
</section>

<footer>
<h2>PunjabOnBeats</h2>
<p>© 2026 PunjabOnBeats. All Rights Reserved.</p>
</footer>

</body>
</html>
