# Travel-Website
A stylish travel adventure website created with HTML, CSS, and JavaScript.

<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">

<title>Travel Adventure</title>

<link rel="stylesheet" href="style.css">

<link
href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.5.1/css/all.min.css"
rel="stylesheet">

</head>

<body>

<header>

<div class="logo">
<i class="fa-solid fa-plane"></i>
Travel Adventure
</div>

<nav>

<a href="#">Home</a>
<a href="#">Destinations</a>
<a href="#">Hotels</a>
<a href="#">Weather</a>
<a href="#">Contact</a>

</nav>

<button class="login-btn">Login</button>

</header>

<section class="hero">

<div class="overlay"></div>

<div class="content">

<h1>Explore The World</h1>

<p>
Find beautiful places, hotels, weather,
travel time and plan your next trip.
</p>

<div class="search-box">

<input
type="text"
placeholder="Search Destination...">

<button>

<i class="fa-solid fa-magnifying-glass"></i>

Search

</button>

</div>

<div class="features">

<div class="card">

<i class="fa-solid fa-cloud-sun"></i>

<h3>Weather</h3>

<p>Live Forecast</p>

</div>

<div class="card">

<i class="fa-solid fa-hotel"></i>

<h3>Hotels</h3>

<p>Best Rooms</p>

</div>

<div class="card">

<i class="fa-solid fa-clock"></i>

<h3>Travel Time</h3>

<p>Distance</p>

</div>

<div class="card">

<i class="fa-solid fa-map-location-dot"></i>

<h3>Map</h3>

<p>Location</p>

</div>

</div>

</div>

</section>

<section class="places">

<h2>Popular Destinations</h2>

<div class="place-grid">

<div class="place">

<img src="images/place1.jpg">

<h3>Switzerland</h3>

<p>Beautiful Mountains</p>

</div>

<div class="place">

<img src="images/place2.jpg">

<h3>Bali</h3>

<p>Tropical Paradise</p>

</div>

<div class="place">

<img src="images/place3.jpg">

<h3>Manali</h3>

<p>Snow Hills</p>

</div>

</div>

</section>

<section class="hotel">

<h2>Recommended Hotels</h2>

<div class="hotel-card">

<img src="images/hotel1.jpg">

<div>

<h3>Mountain View Resort</h3>

<p>⭐⭐⭐⭐⭐</p>

<p>$120 / Night</p>

</div>

</div>

</section>

<section class="travel-time">

<h2>Travel Time Calculator</h2>

<input
type="text"
placeholder="From">

<input
type="text"
placeholder="To">

<button>Calculate</button>

</section>

<footer>

<p>

© 2026 Travel Adventure

</p>

</footer>

<script src="script.js"></script>

</body>
</html>
/* Google Font */
@import url('https://fonts.googleapis.com/css2?family=Poppins:wght@300;400;600;700&display=swap');

*{
    margin:0;
    padding:0;
    box-sizing:border-box;
    font-family:'Poppins',sans-serif;
}

body{
    background:#f5f7fa;
    color:#333;
}

/* Header */
header{
    position:fixed;
    top:0;
    width:100%;
    display:flex;
    justify-content:space-between;
    align-items:center;
    padding:20px 8%;
    background:rgba(0,0,0,.35);
    backdrop-filter:blur(10px);
    z-index:1000;
}

.logo{
    color:#fff;
    font-size:28px;
    font-weight:700;
}

nav a{
    color:#fff;
    text-decoration:none;
    margin:0 15px;
    transition:.3s;
}

nav a:hover{
    color:#00b4ff;
}

.login-btn{
    padding:10px 22px;
    border:none;
    border-radius:30px;
    background:#00b4ff;
    color:#fff;
    cursor:pointer;
}

/* Hero */
.hero{
    height:100vh;
    background:url("images/hero.jpg") center/cover no-repeat;
    position:relative;
    display:flex;
    justify-content:center;
    align-items:center;
}

.overlay{
    position:absolute;
    inset:0;
    background:rgba(0,0,0,.45);
}

.content{
    position:relative;
    z-index:2;
    text-align:center;
    color:white;
    width:90%;
}

.content h1{
    font-size:70px;
    margin-bottom:20px;
}

.content p{
    font-size:22px;
    margin-bottom:30px;
}

/* Search */
.search-box{
    display:flex;
    max-width:700px;
    margin:auto;
    background:#fff;
    border-radius:50px;
    overflow:hidden;
}

.search-box input{
    flex:1;
    padding:18px;
    border:none;
    outline:none;
}

.search-box button{
    background:#00b4ff;
    color:white;
    border:none;
    padding:18px 35px;
    cursor:pointer;
}

/* Feature Cards */
.features{
    display:grid;
    grid-template-columns:repeat(4,1fr);
    gap:20px;
    margin-top:50px;
}

.card{
    background:rgba(255,255,255,.18);
    backdrop-filter:blur(12px);
    padding:30px;
    border-radius:20px;
    color:white;
}

.card i{
    font-size:40px;
    margin-bottom:15px;
}

/* Sections */
section{
    padding:80px 8%;
}

.place-grid{
    display:grid;
    grid-template-columns:repeat(3,1fr);
    gap:25px;
}

.place{
    background:white;
    border-radius:20px;
    overflow:hidden;
    box-shadow:0 10px 20px rgba(0,0,0,.15);
}

.place img{
    width:100%;
    height:230px;
    object-fit:cover;
}

.place h3{
    padding:15px;
}

.place p{
    padding:0 15px 20px;
}

.hotel-card{
    display:flex;
    gap:20px;
    background:white;
    padding:20px;
    border-radius:20px;
    box-shadow:0 8px 18px rgba(0,0,0,.1);
}

.hotel-card img{
    width:220px;
    border-radius:15px;
}

.travel-time input{
    width:250px;
    padding:15px;
    margin:10px;
}

.travel-time button{
    padding:15px 30px;
    background:#00b4ff;
    color:white;
    border:none;
}

footer{
    background:#111;
    color:white;
    text-align:center;
    padding:30px;
}

/* Mobile */
@media(max-width:900px){

.content h1{
    font-size:45px;
}

.features{
    grid-template-columns:1fr 1fr;
}

.place-grid{
    grid-template-columns:1fr;
}

.hotel-card{
    flex-direction:column;
}

.search-box{
    flex-direction:column;
    border-radius:20px;
}

.search-box button{
    width:100%;
}

}
// ===============================
// Travel Adventure Website
// script.js
// ===============================

// Welcome Message
window.addEventListener("load", () => {
    console.log("Welcome to Travel Adventure!");
});

// Search Destination
const searchBtn = document.querySelector(".search-box button");
const searchInput = document.querySelector(".search-box input");

if (searchBtn && searchInput) {
    searchBtn.addEventListener("click", () => {

        let destination = searchInput.value.trim();

        if (destination === "") {
            alert("Please enter a destination.");
        } else {
            alert("Searching for: " + destination);
        }

    });
}

// Dark Mode
const darkButton = document.createElement("button");

darkButton.innerHTML = "🌙";

darkButton.style.position = "fixed";
darkButton.style.right = "20px";
darkButton.style.bottom = "20px";
darkButton.style.width = "55px";
darkButton.style.height = "55px";
darkButton.style.borderRadius = "50%";
darkButton.style.border = "none";
darkButton.style.cursor = "pointer";
darkButton.style.fontSize = "22px";
darkButton.style.background = "#0099ff";
darkButton.style.color = "#fff";

document.body.appendChild(darkButton);

darkButton.addEventListener("click", () => {

    document.body.classList.toggle("dark-mode");

});

// Scroll Animation
const cards = document.querySelectorAll(".card, .place");

window.addEventListener("scroll", () => {

    cards.forEach(card => {

        const position = card.getBoundingClientRect().top;

        if (position < window.innerHeight - 100) {

            card.style.opacity = "1";
            card.style.transform = "translateY(0px)";

        }

    });

});

// Initial Animation Style
cards.forEach(card => {

    card.style.opacity = "0";
    card.style.transform = "translateY(40px)";
    card.style.transition = "0.6s";

});

// Travel Time Calculator
const travelButton = document.querySelector(".travel-time button");

if (travelButton) {

travelButton.addEventListener("click", () => {

const from = document.querySelectorAll(".travel-time input")[0].value;

const to = document.querySelectorAll(".travel-time input")[1].value;

if(from==="" || to===""){

alert("Please enter both locations.");

}else{

alert(
"Travel time calculation for:\n\n"
+ from + " ➜ " + to +
"\n\nFeature will connect with Google Maps API later."
);

}

});

}

// Wishlist
const hearts = document.querySelectorAll(".place");

hearts.forEach(place=>{

place.addEventListener("click",()=>{

place.style.border="3px solid #00bfff";

alert("Added to Wishlist ❤️");

});

});