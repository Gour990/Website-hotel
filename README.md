<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Luxury Stay Hotel</title>

<style>
*{
    margin:0;
    padding:0;
    box-sizing:border-box;
    font-family: 'Segoe UI', sans-serif;
}

body{
    background:#f5f5f5;
    color:#333;
}

header{
    background:#111;
    color:#fff;
    padding:20px 10%;
    display:flex;
    justify-content:space-between;
    align-items:center;
}

header h1{
    font-size:24px;
}

nav a{
    color:#fff;
    text-decoration:none;
    margin-left:20px;
}

.hero{
    height:90vh;
    background:url('https://images.unsplash.com/photo-1501117716987-c8e1ecb2106b') center/cover;
    display:flex;
    justify-content:center;
    align-items:center;
    color:#fff;
    text-align:center;
}

.hero h2{
    font-size:50px;
    background:rgba(0,0,0,0.6);
    padding:20px;
}

.section{
    padding:60px 10%;
}

.rooms{
    display:grid;
    grid-template-columns:repeat(auto-fit, minmax(250px,1fr));
    gap:20px;
}

.room-card{
    background:#fff;
    padding:20px;
    border-radius:10px;
    box-shadow:0 5px 15px rgba(0,0,0,0.1);
    text-align:center;
}

.room-card img{
    width:100%;
    border-radius:10px;
}

button{
    background:#111;
    color:#fff;
    padding:10px 20px;
    border:none;
    margin-top:10px;
    cursor:pointer;
    border-radius:5px;
}

.booking-form{
    background:#fff;
    padding:30px;
    border-radius:10px;
    box-shadow:0 5px 15px rgba(0,0,0,0.1);
}

.booking-form input{
    width:100%;
    padding:10px;
    margin:10px 0;
}

footer{
    background:#111;
    color:#fff;
    text-align:center;
    padding:20px;
}

.unique-feature{
    background:#222;
    color:#fff;
    text-align:center;
    padding:40px;
    border-radius:10px;
}
</style>

</head>
<body>

<header>
    <h1>Luxury Stay</h1>
    <nav>
        <a href="#">Home</a>
        <a href="#rooms">Rooms</a>
        <a href="#booking">Booking</a>
        <a href="#contact">Contact</a>
    </nav>
</header>

<section class="hero">
    <h2>Experience Luxury & Comfort</h2>
</section>

<section class="section" id="rooms">
    <h2>Our Rooms</h2><br>
    <div class="rooms">
        <div class="room-card">
            <img src="https://images.unsplash.com/photo-1560184897-ae75f418493e">
            <h3>Deluxe Room</h3>
            <p>₹2500 / Night</p>
            <button>Book Now</button>
        </div>
        <div class="room-card">
            <img src="https://images.unsplash.com/photo-1582719478250-c89cae4dc85b">
            <h3>Executive Suite</h3>
            <p>₹4500 / Night</p>
            <button>Book Now</button>
        </div>
        <div class="room-card">
            <img src="https://images.unsplash.com/photo-1590490360182-c33d57733427">
            <h3>Family Room</h3>
            <p>₹3500 / Night</p>
            <button>Book Now</button>
        </div>
    </div>
</section>

<section class="section">
    <div class="unique-feature">
        <h2>🔥 Live Availability Checker</h2>
        <p id="availability">Checking availability...</p>
    </div>
</section>

<section class="section" id="booking">
    <h2>Book Your Stay</h2><br>
    <div class="booking-form">
        <input type="text" placeholder="Full Name">
        <input type="email" placeholder="Email">
        <input type="date">
        <input type="date">
        <button onclick="bookNow()">Confirm Booking</button>
    </div>
</section>

<section class="section" id="contact">
    <h2>Contact Us</h2><br>
    <p>Email: info@luxurystay.com</p>
    <p>Phone: +91 9876543210</p>
    <p>Location: Kolkata, India</p>
</section>

<footer>
    <p>© 2026 Luxury Stay Hotel | All Rights Reserved</p>
</footer>

<script>
setTimeout(() => {
    document.getElementById("availability").innerText = 
    "Rooms Available Today: " + Math.floor(Math.random()*5 + 1);
},2000);

function bookNow(){
    alert("Booking Request Submitted Successfully!");
}
</script>

</body>
</html>
