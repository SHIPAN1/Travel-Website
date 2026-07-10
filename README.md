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