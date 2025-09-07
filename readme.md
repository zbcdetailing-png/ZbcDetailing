<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>ZBC Mobile Detailing</title>
  <style>
    body {
      margin: 0;
      font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
      background: #0d0d0d;
      color: #f5f5f5;
      line-height: 1.7;
    }

    header {
      background: linear-gradient(135deg, #111, #222);
      text-align: center;
      padding: 2rem 1rem 1rem;
      color: #ffd700;
    }

    /* Logo */
    .hero-logo {
      width: 180px;
      display: block;
      margin: 0 auto 1.5rem;
    }

    header h1 {
      font-size: 2.5rem;
      margin: 0.5rem 0;
    }

    header p {
      font-size: 1.2rem;
      color: #ccc;
      margin-bottom: 1.5rem;
    }

    .hero-img {
      width: 100%;
      height: 60vh;
      object-fit: cover;
      border-bottom: 4px solid #ffd700;
      border-top: 4px solid #ffd700;
      box-shadow: 0 4px 15px rgba(0,0,0,0.7);
    }

    section {
      padding: 3rem 2rem;
      max-width: 1000px;
      margin: auto;
    }

    h2 {
      color: #ffd700;
      border-bottom: 2px solid #ffd700;
      display: inline-block;
      margin-bottom: 1.5rem;
    }

    .services {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(280px, 1fr));
      gap: 2rem;
    }

    .service {
      background: rgba(255, 255, 255, 0.05);
      border-radius: 15px;
      padding: 1.5rem;
      box-shadow: 0 4px 30px rgba(0,0,0,0.5);
      transition: transform 0.3s ease, background 0.3s ease;
    }

    .service:hover {
      transform: translateY(-8px);
      background: rgba(255, 255, 255, 0.08);
    }

    .service h3 {
      color: #ffd700;
    }

    .price-toggle {
      background: none;
      border: 1px solid #ffd700;
      color: #ffd700;
      padding: 8px 14px;
      border-radius: 8px;
      cursor: pointer;
      margin-top: 10px;
      transition: background 0.3s ease;
    }

    .price-toggle:hover {
      background: #ffd700;
      color: #111;
    }

    .price-dropdown {
      margin-top: 10px;
      padding-left: 10px;
      max-height: 0;
      overflow: hidden;
      transition: max-height 0.3s ease, opacity 0.3s ease;
      opacity: 0;
    }

    .price-dropdown.show {
      max-height: 500px;
      opacity: 1;
    }

    footer {
      text-align: center;
      background: #111;
      padding: 2rem 1rem;
      color: #999;
      margin-top: 2rem;
    }

    footer a {
      color: #ffd700;
      text-decoration: none;
    }
  </style>
</head>
<body>

  <!-- Header -->
  <header>
    <!-- Logo -->
    <img src="0bb472_b1564ee42f6a4271ad8486c554b7d804~mv2.png" alt="ZBC Detailing Logo" class="hero-logo">

    <h1>ZBC Mobile Detailing</h1>
    <p>"Making Detailing Great Again"</p>

    <!-- Hero Car Image -->
    <img src="https://images.unsplash.com/photo-1503736334956-4c8f8e92946d" alt="Luxury Car Detailing" class="hero-img">
  </header>

  <!-- Services -->
  <section id="services">
    <h2>💎 Our Packages</h2>
    <div class="services">

      <!-- Interior Reset -->
      <div class="service">
        <h3>🛋️ The Interior Reset</h3>
        <p>Deep clean & protect every surface. Addons if asked for: 🐾 Pet Hair • ☣️ Biohazards • 🧴 Stains • 🌫️ Odors</p>
        <button class="price-toggle">View Prices by Vehicle Type ⬇️</button>
        <div class="price-dropdown">
          <p>Sedan: 💰 $150 — ⏱ 2.5 hrs</p>
          <p>SUV: 💰 $180 — ⏱ 3 hrs</p>
          <p>Truck: 💰 $200 — ⏱ 3.5 hrs</p>
        </div>
      </div>

      <!-- Exterior Revival -->
      <div class="service">
        <h3>🚿 The Exterior Revival</h3>
        <p>Hand wash, clay bar & wax. Addons if asked for: 🧲 Tar Removal • 💧 Water Spots • 🛢️ Tire Dressing • 🖤 Trim</p>
        <button class="price-toggle">View Prices by Vehicle Type ⬇️</button>
        <div class="price-dropdown">
          <p>Sedan: 💰 $120 — ⏱ 2 hrs</p>
          <p>SUV: 💰 $150 — ⏱ 2.5 hrs</p>
          <p>Truck: 💰 $170 — ⏱ 3 hrs</p>
        </div>
      </div>

      <!-- Signature Shine -->
      <div class="service">
        <h3>✨ The Signature Shine (Full Interior + Exterior)</h3>
        <p>The ultimate full detail inside & out.</p>
        <button class="price-toggle">View Prices by Vehicle Type ⬇️</button>
        <div class="price-dropdown">
          <p>Sedan: 💰 $250 — ⏱ 4 hrs</p>
          <p>SUV: 💰 $300 — ⏱ 4.5 hrs</p>
          <p>Truck: 💰 $350 — ⏱ 5 hrs</p>
        </div>
      </div>

      <!-- Engine Bay -->
      <div class="service">
        <h3>⚙️ Engine Bay Revival</h3>
        <p>Degrease, clean, and protect engine components.</p>
        <p>💰 $80 — ⏱ 1 hr</p>
      </div>

      <!-- Ceramic Coating -->
      <div class="service">
        <h3>🛡️ Ceramic Coating + Paint Correction</h3>
        <p>Enhance gloss, protect paint & remove imperfections.</p>
        <p>💰 Starting at $600 — ⏱ 6–8 hrs</p>
      </div>

      <!-- Headlight -->
      <div class="service">
        <h3>🔦 Headlight Restoration</h3>
        <p>Restore clarity, improve visibility & protection.</p>
        <p>💰 $60 — ⏱ 45 mins</p>
      </div>

      <!-- Glass Polish -->
      <div class="service">
        <h3>🪟 Glass Polish</h3>
        <p>Remove water spots & restore perfect clarity to windows.</p>
        <p>💰 $70 — ⏱ 1 hr</p>
      </div>

      <!-- Add-Ons -->
      <div class="service">
        <h3>➕ Add-Ons</h3>
        <p>Specialized services for tougher jobs.</p>
        <button class="price-toggle">View Add-Ons ⬇️</button>
        <div class="price-dropdown">
          <p>🟡 Stain Removal – 💰 $25+</p>
          <p>🟡 Biohazard Cleanup – 💰 $90+</p>
          <p>🟡 Excessive Pet Hair Removal – 💰 $35+</p>
          <p>🟡 Odor Elimination – 💰 $75+</p>
          <p>🟡 Trim Restoration – 💰 $125</p>
          <p>🟡 Water Spot Removal – 💰 $75+</p>
          <p>🟡 Clay Bar + Iron Remover – 💰 $75</p>
          <p>🟡 Leather Ceramic Coating – 💰 $150+</p>
        </div>
      </div>

    </div>
  </section>

  <!-- Contact -->
  <section id="contact">
    <h2>📍 Contact Us</h2><br>
    <p>Serving your area with premium mobile detailing.</p>
    <p>📲 Instagram: <a href="https://www.instagram.com/zbcdetailing" target="_blank">@zbcdetailing</a> • Facebook: <a href="https://www.facebook.com/zbcdetailing" target="_blank">@zbcdetailing</a></p>
    <p>☎️ <a href="tel:5703908696">570-390-8696</a> • ✉️ <a href="mailto:zbcdetailing@gmail.com">zbcdetailing@gmail.com</a></p>
  </section>

  <!-- Footer -->
  <footer>
    <p>Luxury Mobile Detailing</p>
    <p>☎️ <a href="tel:5703908696">570-390-8696</a> • ✉️ <a href="mailto:zbcdetailing@gmail.com">zbcdetailing@gmail.com</a></p>
    <p>"Luxury is in the details."</p>
  </footer>

  <!-- Script for Dropdowns -->
  <script>
    const toggles = document.querySelectorAll(".price-toggle");
    toggles.forEach(button => {
      button.addEventListener("click", () => {
        const dropdown = button.nextElementSibling;
        dropdown.classList.toggle("show");
      });
    });
  </script>

</body>
</html>
