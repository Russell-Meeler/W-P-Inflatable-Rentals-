# W-P-Inflatable-Rentals-
Inflatable bounce house rental company 
wp-inflatables/
├── index.html
├── style.css
└── script.js
 <!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
  <title>W&P Inflatable Rentals</title>
  <link rel="stylesheet" href="style.css" />
</head>
<body>
  <header>
    <div class="logo">W&P Inflatables</div>
    <nav>
      <ul>
        <li><a href="#services">Services</a></li>
        <li><a href="#gallery">Gallery</a></li>
        <li><a href="#inventory">Inventory</a></li>
        <li><a href="#booking">Booking</a></li>
      </ul>
    </nav>
  </header>

  <section class="hero">
    <h1>Make Your Event Unforgettable</h1>
    <p>Safe, clean, and fun inflatable rentals in Morgan County, AL</p>
    <a href="#booking" class="cta-button">Book Now</a>
  </section>

  <section id="services">
    <h2>Our Services</h2>
    <div class="cards">
      <div class="card">
        <h3>Bounce Houses</h3>
        <p>Perfect for birthday parties and school events.</p>
      </div>
      <div class="card">
        <h3>Water Slides</h3>
        <p>Beat the heat with our thrilling water slides!</p>
      </div>
      <div class="card">
        <h3>Combo Units</h3>
        <p>Get a bounce house and slide combo for more fun!</p>
      </div>
    </div>
  </section>

  <section id="gallery">
    <h2>Gallery</h2>
    <div class="gallery">
      <img src="bounce1.jpg" alt="Bounce House" />
      <img src="slide1.jpg" alt="Water Slide" />
      <img src="combo1.jpg" alt="Combo Unit" />
    </div>
  </section>

  <section id="inventory">
    <h2>Our Rental Inventory</h2>
    <div class="inventory-grid">
      <div class="inventory-item">
        <img src="bounce1.jpg" alt="Blue Castle Bounce House">
        <h3>Blue Castle Bounce House</h3>
        <p>Spacious and colorful, great for kids 3-12 years old. 15x15 feet.</p>
        <a href="#booking" class="cta-button small">Book Now</a>
      </div>
      <div class="inventory-item">
        <img src="slide1.jpg" alt="Wild Splash Water Slide">
        <h3>Wild Splash Water Slide</h3>
        <p>Keep cool with this exciting water slide, perfect for summer parties.</p>
        <a href="#booking" class="cta-button small">Book Now</a>
      </div>
      <div class="inventory-item">
        <img src="combo1.jpg" alt="Combo Fun Zone">
        <h3>Combo Fun Zone</h3>
        <p>A bounce house with a slide attached — double the fun in one unit!</p>
        <a href="#booking" class="cta-button small">Book Now</a>
      </div>
    </div>
  </section>

  <section id="booking">
    <h2>Book a Rental</h2>
    <form action="https://formspree.io/f/yourformid" method="POST">
      <label>
        Your Name:
        <input type="text" name="name" required>
      </label>
      <label>
        Email:
        <input type="email" name="email" required>
      </label>
      <label>
        Phone Number:
        <input type="text" name="phone">
      </label>
      <label>
        Select Your Rental:
        <select name="rental" required>
          <option value="Bounce House">Bounce House</option>
          <option value="Water Slide">Water Slide</option>
          <option value="Combo Unit">Combo Unit</option>
        </select>
      </label>
      <label>
        Event Date:
        <input type="date" name="event_date" required>
      </label>
      <label>
        Address:
        <textarea name="address" required></textarea>
      </label>
      <label>
        Additional Info:
        <textarea name="message" placeholder="Tell us more..."></textarea>
      </label>
      <button type="submit">Send Booking Request</button>
    </form>
    <p id="formResponse"></p>
  </section>

  <footer>
    <p>&copy; 2025 W&P Inflatable Rentals. All rights reserved.</p>
  </footer>

  <script src="script.js"></script>
</body>
</html>
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}

body {
  font-family: Arial, sans-serif;
  line-height: 1.6;
  background: #f7f7f7;
  color: #333;
}

header {
  background: #0066cc;
  color: white;
  padding: 20px;
  display: flex;
  justify-content: space-between;
  align-items: center;
  flex-wrap: wrap;
}

.logo {
  font-size: 24px;
  font-weight: bold;
}

nav ul {
  list-style: none;
  display: flex;
  gap: 20px;
}

nav a {
  color: white;
  text-decoration: none;
}

.hero {
  background: url('https://via.placeholder.com/1200x400') center/cover no-repeat;
  color: white;
  text-align: center;
  padding: 100px 20px;
}

.cta-button {
  background: #ffcc00;
  color: #333;
  padding: 10px 20px;
  text-decoration: none;
  margin-top: 20px;
  display: inline-block;
  font-weight: bold;
  border-radius: 5px;
}

section {
  padding: 60px 20px;
  max-width: 1000px;
  margin: auto;
}

h2 {
  margin-bottom: 30px;
  text-align: center;
}

.cards {
  display: flex;
  flex-wrap: wrap;
  gap: 20px;
  justify-content: center;
}

.card {
  background: white;
  padding: 20px;
  flex: 1 1 250px;
  border-radius: 10px;
  box-shadow: 0 0 10px rgba(0,0,0,0.1);
  text-align: center;
}

.gallery {
  display: flex;
  flex-wrap: wrap;
  gap: 20px;
  justify-content: center;
}

.gallery img {
  width: 300px;
  height: auto;
  border-radius: 10px;
}

.inventory-grid {
  display: flex;
  flex-wrap: wrap;
  gap: 30px;
  justify-content: center;
}

.inventory-item {
  background: white;
  padding: 20px;
  border-radius: 10px;
  box-shadow: 0 0 10px rgba(0,0,0,0.1);
  width: 300px;
  text-align: center;
}

.inventory-item img {
  width: 100%;
  border-radius: 10px;
  margin-bottom: 15px;
}

.inventory-item h3 {
  margin-bottom: 10px;
}

.cta-button.small {
  font-size: 0.9rem;
  padding: 8px 16px;
  margin-top: 10px;
}

form {
  display: flex;
  flex-direction: column;
  gap: 15px;
}

form input,
form textarea,
form select {
  padding: 10px;
  border: 1px solid #ccc;
  border-radius: 5px;
  font-size: 1rem;
}

form button {
  background: #0066cc;
  color: white;
  padding: 12px;
  border: none;
  font-size: 1rem;
  border-radius: 5px;
  cursor: pointer;
}

footer {
  text-align: center;
  padding: 20px;
  background: #333;
  color: white;
  margin-top: 40px;
}

/* Responsive */
@media (max-width: 768px) {
  .cards, .gallery, .inventory-grid {
    flex-direction: column;
    align-items: center;
  }

  header {
    flex-direction: column;
    text-align: center;
  }

  nav ul {
    flex-direction: column;
    gap: 10px;
  }
}
document.querySelector("form").addEventListener("submit", function (e) {
  const response = document.getElementById("formResponse");
  response.textContent = "Thank you! We'll be in touch soon.";
});