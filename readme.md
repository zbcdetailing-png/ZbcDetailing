<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>ZBC Mobile Detailing</title>
  <style>
    /* General Styles */
    body {
      margin: 0;
      font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
      background: #000000; /* true black background */
      color: #f5f5f5;
      line-height: 1.7;
    }

    header {
      background: #000000; /* true black */
      text-align: center;
      padding: 1rem 1rem;
      color: #ffd700;
    }

    header h1 {
      display: none; /* hide the top text */
    }

    header p {
      font-size: 1.1rem;
      color: #ccc;
      margin-bottom: 0.8rem;
    }

    header img {
      width: 100%;
      max-width: 300px;
      height: auto;
      margin-top: 0.5rem;
    }

    section {
      padding: 3rem 2rem;
      max-width: 1000px;
      margin: auto;
    }

    h2 {
      color: #ffd700;
      border-bottom: none; /* removed the line */
      display: inline-block;
      margin-bottom: 1.5rem;
    }

    .service-container {
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

    /* Winter Special Card */
    .service.winter {
      background: rgba(173, 216, 230, 0.05); /* very light icy blue */
      border: 2px solid #87CEFA; /* light sky blue border */
      box-shadow: 0 4px 30px rgba(135, 206, 250, 0.5);
    }

    .service.winter h3 {
      color: #87CEFA; /* winter blue heading */
    }

    .service.winter .price-toggle:hover {
      background: #87CEFA;
      color: #000; 
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

<header>
  <p>"Making Detailing Great Again"</p>
  <img src="https://raw.githubusercontent.com/zbcdetailing-png/ZbcDetailing/209c8c5ff7527ffa6dcf4833bec9e192d08bc8ba/zbc%20detailing%20logo.jpg" alt="ZBC Detailing Logo" style="max-width:300px; height:auto;">
</header>

<section class="services">
  <h2>💎 Our Packages</h2>
  <div class="service-container">
   <!-- Winter Special -->
    <div class="service winter">
      <h3>❄️ Winter Special – Wash Salt Off</h3>
      <p>Protect your car from winter salt damage with a undercarriage cleaning.</p>
      <button class="price-toggle">View Prices by Vehicle Type ⬇️</button>
      <div class="price-dropdown">
        <p>all cars: 💰 $35 — ⏱ 30 mins</p>
      </div>
    </div>
    
     <!-- Interior Reset -->
    <div class="service">
      <h3>🛋️ The Interior Reset</h3>
      <p>Deep clean & protect every surface. Addons if requested: 🐾 Pet Hair • ☣️ Biohazards • 🧴 Stains • 🌫️ Odors</p>
      <button class="price-toggle">View Prices by Vehicle Type ⬇️</button>
      <div class="price-dropdown">
        <p>Sedan: 💰 $150 — ⏱ 2 hrs</p>
        <p>SUV: 💰 $175 — ⏱ 2.5 hrs</p>
        <p>Truck: 💰 $185 — ⏱ 3 hrs</p>
      </div>
    </div>

    <!-- Exterior Revival -->
    <div class="service">
      <h3>🚿 The Exterior Revival</h3>
      <p>Hand wash🧼, bug removal🪲, shined tires🌟, clear windows⚪️, & wax/spray ceramic🧴. Addons if requested: 🧲 Tar Removal • 💧 Water Spots • 🛢️ Tire Dressing • 🖤 Trim</p>
      <button class="price-toggle">View Prices by Vehicle Type ⬇️</button>
      <div class="price-dropdown">
        <p>Sedan: 💰 $125 — ⏱ 1 hr</p>
        <p>SUV: 💰 $150 — ⏱ 1.5 hrs</p>
        <p>Truck: 💰 $200 — ⏱ 2 hrs</p>
      </div>
    </div>

    <!-- Signature Shine -->
    <div class="service">
      <h3>✨ Signature Shine (Full Interior + Exterior)</h3>
      <p>The ultimate full detail inside & out.</p>
      <button class="price-toggle">View Prices by Vehicle Type ⬇️</button>
      <div class="price-dropdown">
        <p>Sedan: 💰 $265 — ⏱ 4 hrs</p>
        <p>SUV: 💰 $315 — ⏱ 4.5 hrs</p>
        <p>Truck: 💰 $365 — ⏱ 5 hrs</p>
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
      <p>💰 Starting at $800 — ⏱ 6–8 hrs</p>
    </div>

    <!-- Headlight -->
    <div class="service">
      <h3>🔦 Headlight Restoration</h3>
      <p>Restore clarity, improve visibility & protection.</p>
      <p>💰 $100 — ⏱ 1 hr</p>
    </div>

    <!-- Glass Polish -->
    <div class="service">
      <h3>🪟 Glass Polish</h3>
      <p>Remove water spots & restore perfect clarity to windows.</p>
      <p>💰 $75 — ⏱ 1 hr</p>
    </div>

    <!-- Add-Ons -->
    <div class="service">
      <h3>➕ Add-Ons</h3>
      <p>Specialized services for tougher jobs.</p>
      <button class="price-toggle">View Add-Ons ⬇️</button>
      <div class="price-dropdown">
        <p>🟡 Stain Removal – $25+</p>
        <p>🟡 Biohazard Cleanup – $90+</p>
        <p>🟡 Excessive Pet Hair Removal – $35+</p>
        <p>🟡 Odor Elimination – $75+</p>
        <p>🟡 Trim Restoration – $125</p>
        <p>🟡 Water Spot Removal – $75+</p>
        <p>🟡 Clay Bar + Iron Remover – $75</p>
        <p>🟡 Leather Ceramic Coating – $150+</p>
      </div>
    </div>
    
  </div>
</section>

<section class="contact">
  <h2>📍 Contact Us</h2>
  <p>Serving your area with premium mobile detailing.</p>
  <p>📲 Instagram: @zbcdetailing • Facebook: @zbcdetailing</p>
  <p>☎️ 570-390-8696 • ✉️ zbcdetailing@gmail.com</p>
  <p>"Luxury is in the details."</p>
</section>

<footer>
  <p>Luxury Mobile Detailing • © 2025 ZBC Detailing</p>
</footer>

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
</html>  ok i change my mind can you get rid of all the text above it and only keep the logo
