<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>ZBC Detailing</title>
  <style>
    body {
      background-color: #0d0d0d;
      color: #f5f5f5;
      line-height: 1.6;
      overflow-x: hidden;
      scroll-behavior: smooth;
      font-family: Arial, sans-serif;
    }

    h1, h2, h3 {
      color: #ffd700; /* Gold */
      letter-spacing: 1px;
    }

    a, button {
      text-decoration: none;
      color: inherit;
    }

    /* Navbar */
    nav {
      position: fixed;
      top: 0;
      left: 0;
      width: 100%;
      background: rgba(20,20,20,0.9);
      display: flex;
      justify-content: space-between;
      align-items: center;
      padding: 15px 10%;
      z-index: 1000;
      backdrop-filter: blur(10px);
    }

    nav h1 {
      color: #ffd700;
      font-size: 1.5rem;
    }

    nav ul {
      display: flex;
      list-style: none;
      gap: 25px;
    }

    nav ul li a {
      color: #f5f5f5;
      transition: color 0.3s;
    }

    nav ul li a:hover {
      color: #ffd700;
    }

    /* Hero Section */
    .hero {
      height: 100vh;
      display: flex;
      flex-direction: column;
      justify-content: center;
      align-items: center;
      background: linear-gradient(rgba(0,0,0,0.6), rgba(0,0,0,0.6)),
                  url('https://images.unsplash.com/photo-1552519507-da3b142c6e3d') center/cover no-repeat;
      text-align: center;
      animation: fadeIn 1.5s ease-in-out;
    }

    .hero h1 {
      font-size: 3rem;
      margin-bottom: 1rem;
    }

    .hero p {
      font-size: 1.2rem;
      margin-bottom: 2rem;
      color: #ccc;
    }

    .btn {
      background: #ffd700;
      color: #000;
      padding: 12px 30px;
      border-radius: 30px;
      font-weight: bold;
      transition: all 0.3s ease;
    }

    .btn:hover {
      background: #fff;
      transform: scale(1.05);
    }

    /* Sections */
    section {
      padding: 100px 10%;
      opacity: 0;
      transform: translateY(40px);
      transition: all 0.8s ease;
    }

    section.show {
      opacity: 1;
      transform: translateY(0);
    }

    .service {
      background: #1a1a1a;
      padding: 30px;
      border-radius: 15px;
      margin-bottom: 40px;
      box-shadow: 0 8px 20px rgba(0,0,0,0.6);
      transition: transform 0.4s ease, background 0.4s ease;
      opacity: 0;
      transform: translateY(40px);
    }

    .service.show {
      opacity: 1;
      transform: translateY(0);
    }

    .service:hover {
      transform: translateY(-10px);
      background: #222;
    }

    .service h3 {
      margin-bottom: 10px;
      font-size: 1.5rem;
      cursor: pointer;
    }

    .service p {
      color: #bbb;
    }

    .price-time {
      margin-top: 10px;
      font-weight: bold;
      color: #ffd700;
    }

    /* Dropdown styles */
    .dropdown {
      max-height: 0;
      overflow: hidden;
      transition: max-height 0.5s ease;
      margin-top: 10px;
    }

    .service.open .dropdown {
      max-height: 500px;
    }

    /* Arrow rotation */
    .arrow {
      display: inline-block;
      margin-left: 8px;
      transition: transform 0.3s ease;
    }

    .service.open .arrow {
      transform: rotate(180deg);
    }

    /* Add-Ons Section */
    .addons {
      background: #1a1a1a;
      padding: 30px;
      border-radius: 15px;
      margin-bottom: 40px;
      box-shadow: 0 8px 20px rgba(0,0,0,0.6);
      transition: transform 0.4s ease, background 0.4s ease;
      opacity: 0;
      transform: translateY(40px);
    }

    .addons.show {
      opacity: 1;
      transform: translateY(0);
    }

    .addons:hover {
      transform: translateY(-10px);
      background: #222;
    }

    .addons h3 {
      margin-bottom: 10px;
      font-size: 1.5rem;
      cursor: pointer;
    }

    .addons .dropdown {
      max-height: 0;
      overflow: hidden;
      transition: max-height 0.5s ease;
      margin-top: 10px;
    }

    .addons.open .dropdown {
      max-height: 500px;
    }

    .addons .arrow {
      display: inline-block;
      margin-left: 8px;
      transition: transform 0.3s ease;
    }

    .addons.open .arrow {
      transform: rotate(180deg);
    }

    .addons p {
      color: #bbb;
      margin: 8px 0;
    }

    /* Booking Form */
    form {
      background: #1a1a1a;
      padding: 40px;
      border-radius: 15px;
      box-shadow: 0 8px 20px rgba(0,0,0,0.7);
    }

    form input, form select, form textarea {
      width: 100%;
      padding: 12px;
      margin-bottom: 20px;
      border: none;
      border-radius: 8px;
      background: #333;
      color: #f5f5f5;
    }

    form button {
      width: 100%;
      background: #ffd700;
      color: #000;
      font-weight: bold;
      padding: 15px;
      border: none;
      border-radius: 8px;
      cursor: pointer;
      transition: all 0.3s ease;
    }

    form button:hover {
      background: #fff;
      transform: scale(1.05);
    }

    /* Footer */
    footer {
      background: #000;
      padding: 30px;
      text-align: center;
      color: #888;
    }

    footer p {
      margin: 10px 0;
    }

    /* Animations */
    @keyframes fadeIn {
      from { opacity: 0; transform: translateY(20px); }
      to { opacity: 1; transform: translateY(0); }
    }
  </style>
</head>
<body>

  <!-- Navbar -->
  <nav>
    <h1>ZBC Detailing</h1>
    <ul>
      <li><a href="#services">Services</a></li>
      <li><a href="#addons">Add-Ons</a></li>
      <li><a href="#booking">Book Now</a></li>
    </ul>
  </nav>

  <!-- Hero Section -->
  <section class="hero">
    <h1>Luxury Car Detailing</h1>
    <p>Premium quality detailing services to make your car shine like new.</p>
    <a href="#booking" class="btn">Book an Appointment</a>
  </section>

  <!-- Services -->
  <section id="services">
    <div class="service">
      <h3 onclick="this.parentElement.classList.toggle('open')">
        Interior Package <span class="arrow">▼</span>
      </h3>
      <div class="dropdown">
        <p>Sedan – $200</p>
        <p>SUV – $250</p>
        <p>Truck – $275</p>
      </div>
    </div>

    <div class="service">
      <h3 onclick="this.parentElement.classList.toggle('open')">
        Exterior Package <span class="arrow">▼</span>
      </h3>
      <div class="dropdown">
        <p>Sedan – $225</p>
        <p>SUV – $275</p>
        <p>Truck – $325</p>
      </div>
    </div>

    <div class="service">
      <h3 onclick="this.parentElement.classList.toggle('open')">
        Signature Shine <span class="arrow">▼</span>
      </h3>
      <div class="dropdown">
        <p>Sedan – $275</p>
        <p>SUV – $325</p>
        <p>Truck – $375</p>
      </div>
    </div>
  </section>

  <!-- Add-Ons -->
  <section id="addons">
    <div class="addons">
      <h3 onclick="this.parentElement.classList.toggle('open')">
        Add-Ons <span class="arrow">▼</span>
      </h3>
      <div class="dropdown">
        <p>🟡 Stain Removal – $50+</p>
        <p>🟡 Biohazard Cleanup – $100+</p>
        <p>🟡 Pet Hair Removal – $40+</p>
        <p>🟡 Odor Elimination – $75+</p>
        <p>🟡 Headlight Restoration – $60</p>
      </div>
    </div>
  </section>

  <!-- Booking Form -->
  <section id="booking">
    <form>
      <h2>Book Your Appointment</h2>
      <input type="text" placeholder="Full Name" required>
      <input type="email" placeholder="Email Address" required>
      <input type="tel" placeholder="Phone Number" required>
      <select required>
        <option value="">Select Service</option>
        <option>Interior Package</option>
        <option>Exterior Package</option>
        <option>Signature Shine</option>
        <option>Add-On</option>
      </select>
      <textarea rows="5" placeholder="Additional Notes"></textarea>
      <button type="submit">Submit</button>
    </form>
  </section>

  <!-- Footer -->
  <footer>
    <p>&copy; 2025 ZBC Detailing. All Rights Reserved.</p>
    <p>Follow us on Instagram @ZBCDetailing</p>
  </footer>

</body>
</html>
