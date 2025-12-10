<!DOCTYPE html>
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
      position: relative; /* for snowflakes */
      overflow: hidden;
    }

    .service.winter h3 {
      color: #87CEFA; /* winter blue heading */
    }

    .service.winter .price-toggle:hover {
      background: #87CEFA;
      color: #000; 
    }

    /* Snow animation with drift */
    .snowflakes {
      position: absolute;
      top: 0;
      left: 0;
      width: 100%;
      height: 100%;
      pointer-events: none; /* allow clicks through snow */
    }

    .snowflake {
      position: absolute;
      top: -2em;
      color: #87CEFA;
      font-size: 1rem;
      user-select: none;
      animation-name: fall, drift;
      animation-duration: 6s, 3s;
      animation-timing-function: linear, ease-in-out;
      animation-iteration-count: infinite, infinite;
      opacity: 0.8;
    }

    .snowflake:nth-child(1) { left: 10%; animation-delay: 0s, 0s; font-size:1rem;}
    .snowflake:nth-child(2) { left: 30%; animation-delay: 1s, 0.5s; font-size:1.2rem;}
    .snowflake:nth-child(3) { left: 50%; animation-delay: 2s, 1s; font-size:0.8rem;}
    .snowflake:nth-child(4) { left: 70%; animation-delay: 3s, 1.5s; font-size:1rem;}
    .snowflake:nth-child(5) { left: 90%; animation-delay: 4s, 2s; font-size:1.1rem;}

    @keyframes fall {
      0% { transform: translateY(-2em); opacity: 0.8; }
      50% { opacity: 1; }
      100% { transform: translateY(100%); opacity: 0; }
    }

    @keyframes drift {
      0% { transform: translateX(0); }
      50% { transform: translateX(10px); }
      100% { transform: translateX(0); }
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
    <!-- Other services omitted for brevity, same as before -->

    <!-- Winter Special -->
    <div class="service winter">
      <h3>❄️ Winter Special – Wash Salt Off</h3>
      <p>Protect your car from winter salt damage with a thorough wash and undercarriage cleaning.</p>
      <button class="price-toggle">View Prices by Vehicle Type ⬇️</button>
      <div class="price-dropdown">
        <p>all cars: 💰 $35 — ⏱ 30 mins</p>
      </div>

      <!-- Snowflakes container -->
      <div class="snowflakes" aria-hidden="true">
        <div class="snowflake">❄️</div>
        <div class="snowflake">❄️</div>
        <div class="snowflake">❄️</div>
        <div class="snowflake">❄️</div>
        <div class="snowflake">❄️</div>
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
</html>
