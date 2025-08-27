<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Luxury Mobile Detailing</title>
  <style>
    /* Global Styles */
    * {
      margin: 0;
      padding: 0;
      box-sizing: border-box;
      font-family: 'Poppins', sans-serif;
    }

    body {
      background-color: #0d0d0d;
      color: #f5f5f5;
      line-height: 1.6;
      overflow-x: hidden;
      scroll-behavior: smooth;
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
    }

    .service p {
      color: #bbb;
    }

    .price-time {
      margin-top: 10px;
      font-weight: bold;
      color: #ffd700;
    }

    .price-toggle {
      margin-top: 10px;
      padding: 10px 15px;
      border: none;
      border-radius: 8px;
      background: #ffd700;
      color: #000;
      font-weight: bold;
      cursor: pointer;
      transition: all 0.3s ease;
    }

    .price-toggle:hover {
      background: #fff;
      transform: scale(1.05);
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
    <h1>🚘 Luxury Detailing</h1>
    <ul>
      <li><a href="#services">Services</a></li>
      <li><a href="#booking">Book</a></li>
      <li><a href="#contact">Contact</a></li>
    </ul>
  </nav>

  <!-- Hero Section -->
  <div class="hero">
    <h1>🚘✨ Luxury Mobile Detailing</h1>
    <p>"Experience showroom shine at your doorstep"</p>
    <a href="#services" class="btn">Book Your Detail</a>
  </div>

  <!-- Services -->
  <section id="services">
    <h2>Our Packages</h2><br><br>

    <!-- Interior Reset -->
    <div class="service">
      <h3>🛋️ The Interior Reset</h3>
      <p>Deep clean & protect every surface. Sub-services: 🐾 Pet Hair • ☣️ Biohazards • 🧴 Stains • 🌫️ Odors</p>
      <button class="price-toggle">View Prices by Vehicle Type ⬇️</button>
      <div class="price-dropdown" style="display:none; margin-top:10px; color:#ffd700;">
        <p>Sedan: 💰 $150 — ⏱ 2.5 hrs</p>
        <p>SUV: 💰 $180 — ⏱ 3 hrs</p>
        <p>Truck: 💰 $200 — ⏱ 3.5 hrs</p>
      </div>
    </div>

    <!-- Exterior Revival -->
    <div class="service">
      <h3>🚿 The Exterior Revival</h3>
      <p>Hand wash, clay bar & wax. Sub-services: 🧲 Tar Removal • 💧 Water Spots • 🛢️ Tire Dressing • 🖤 Trim</p>
      <button class="price-toggle">View Prices by Vehicle Type ⬇️</button>
      <div class="price-dropdown" style="display:none; margin-top:10px; color:#ffd700;">
        <p>Sedan: 💰 $120 — ⏱ 2 hrs</p>
        <p>SUV: 💰 $150 — ⏱ 2.5 hrs</p>
        <p>Truck: 💰 $170 — ⏱ 3 hrs</p>
      </div>
    </div>

    <!-- Other Services -->
    <div class="service">
      <h3>💎 The Signature Shine</h3>
      <p>A complete inside + outside refresh for your ride 🚘✨</p>
      <p class="price-time">💰 $250 — ⏱ 4 hrs</p>
    </div>

    <div class="service">
      <h3>⚙️ The Engine Elegance</h3>
      <p>Degreasing, steam cleaning, and protective dressing.</p>
      <p class="price-time">💰 $80 — ⏱ 1 hr</p>
    </div>

    <div class="service">
      <h3>🛡️ The Diamond Coat</h3>
      <p>Multi-stage paint correction + ceramic coating for ultimate protection.</p>
      <p class="price-time">💰 Starting at $800 — ⏱ 8–12 hrs</p>
    </div>

    <div class="service">
      <h3>🔦 The Clarity Restoration</h3>
      <p>Headlight wet sanding, polish, and UV sealant for clarity.</p>
      <p class="price-time">💰 $100 — ⏱ 1.5 hrs</p>
    </div>

    <div class="service">
      <h3>🪟 The Glass Polish</h3>
      <p>Removes haze, water spots & restores optical clarity to glass.</p>
      <p class="price-time">💰 $70 — ⏱ 1 hr</p>
    </div>
  </section>

  <!-- Booking Form -->
  <section id="booking">
    <h2>📅 Schedule Your Detail</h2><br><br>
    <form>
      <input type="text" placeholder="Full Name" required>
      <input type="tel" placeholder="Phone Number" required>
      <input type="text" placeholder="Vehicle (Make & Model)" required>
      <select required>
        <option value="">Select Package</option>
        <option>The Interior Reset — $150+</option>
        <option>The Exterior Revival — $120+</option>
        <option>The Signature Shine — $250</option>
        <option>The Engine Elegance — $80</option>
        <option>The Diamond Coat — $800+</option>
        <option>The Clarity Restoration — $100</option>
        <option>The Glass Polish — $70</option>
      </select>
      <textarea rows="4" placeholder="Additional Notes / Sub-services"></textarea>
      <button type="submit">Book Now</button>
    </form>
  </section>

  <!-- Contact / Footer -->
  <section id="contact">
    <h2>📍 Contact Us</h2><br>
    <p>Serving your area with premium mobile detailing.</p>
    <p>📲 Instagram: <a href="https://www.instagram.com/zbcdetailing" target="_blank" style="color:#ffd700;">@zbcdetailing</a> • Facebook: <a href="https://www.facebook.com/zbcdetailing" target="_blank" style="color:#ffd700;">@zbcdetailing</a></p>
    <p>☎️ <a href="tel:5703908696" style="color:#ffd700;">570-390-8696</a> • ✉️ <a href="mailto:zbcdetailing@gmail.com" style="color:#ffd700;">zbcdetailing@gmail.com</a></p>
  </section>

  <footer>
    <p>Luxury Mobile Detailing</p>
    <p>"Luxury is in the details."</p>
  </footer>

  <!-- Scroll Animation Script -->
  <script>
    const sections = document.querySelectorAll("section, .service");

    const observer = new IntersectionObserver(entries => {
      entries.forEach(entry => {
        if (entry.isIntersecting) {
          entry.target.classList.add("show");
        }
      });
    }, { threshold: 0.1 });

    sections.forEach(sec => {
      observer.observe(sec);
    });

    // Dropdown toggle functionality
    const toggleButtons = document.querySelectorAll('.price-toggle');
    toggleButtons.forEach(button => {
      button.addEventListener('click', () => {
        const dropdown = button.nextElementSibling;
        if (dropdown.style.display === 'none') {
          dropdown.style.display = 'block';
          button.textContent = "Hide Prices ⬆️";
        } else {
          dropdown.style.display = 'none';
          button.textContent = "View Prices by Vehicle Type ⬇️";
        }
      });
    });
  </script>

</body>
</html>
