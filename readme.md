<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>ZBC Detailing | Professional Auto Detailing Services</title>
    <link rel="preconnect" href="https://fonts.googleapis.com" />
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin />
    <link
      href="https://fonts.googleapis.com/css2?family=Inter:wght@400;500;600;700;800&display=swap"
      rel="stylesheet"
    />
    <style>
:root {
  --bg: #09121d;
  --card: #112133;
  --muted: #12263a;
  --text: #f3f7fb;
  --text-soft: #b7c8d8;
  --accent: #2dd4bf;
  --accent-dark: #14b8a6;
  --line: #2a3e53;
  --white: #ffffff;
}

* {
  box-sizing: border-box;
}

body {
  margin: 0;
  font-family: "Inter", sans-serif;
  color: var(--text);
  background: linear-gradient(180deg, #07101a 0%, #0b1724 50%, #08111c 100%);
  line-height: 1.6;
}

.container {
  width: min(1120px, 92vw);
  margin: 0 auto;
}

.topbar {
  z-index: 20;
  backdrop-filter: blur(8px);
  background: rgb(6 12 20 / 85%);
  border-bottom: 1px solid var(--line);
}

.topbar-content {
  display: flex;
  align-items: center;
  justify-content: space-between;
  gap: 1rem;
  padding: 1rem 0;
}

.brand {
  text-decoration: none;
  color: var(--white);
  font-weight: 800;
  font-size: 1.2rem;
}

.brand-wrap {
  display: flex;
  flex-direction: column;
  align-items: flex-start;
  gap: 0.35rem;
}

.brand-logo {
  width: 100px;
  height: auto;
  border-radius: 0.45rem;
  border: 1px solid var(--line);
}

.nav-links {
  display: flex;
  align-items: center;
  gap: 1rem;
  flex-wrap: wrap;
}

.nav-links a {
  color: var(--text-soft);
  text-decoration: none;
  font-weight: 600;
}

.nav-links a:hover {
  color: var(--white);
}

.button-link {
  border: 1px solid var(--line);
  padding: 0.45rem 0.75rem;
  border-radius: 999px;
}

.hero {
  padding: 2.25rem 0 3rem;
}

.hero-main-card {
  background: var(--card);
  border: 1px solid var(--line);
  border-radius: 1rem;
  padding: 1.2rem;
  grid-column: 1;
  grid-row: 1;
}

.hero-main-card .eyebrow {
  margin-top: 0;
}

.hero-grid {
  display: grid;
  grid-template-columns: 1.5fr 1fr;
  gap: 1rem;
  align-items: start;
}

.eyebrow {
  color: var(--accent);
  text-transform: uppercase;
  font-weight: 700;
  letter-spacing: 0.06em;
  font-size: 0.84rem;
}

h1,
h2,
h3 {
  line-height: 1.2;
  margin-top: 0;
}

h1 {
  font-size: clamp(2rem, 4vw, 3.2rem);
}

.hero-text {
  color: var(--text-soft);
  max-width: 62ch;
}

.hero-actions {
  display: flex;
  gap: 0.8rem;
  margin-top: 1.4rem;
  flex-wrap: wrap;
}

.btn {
  text-decoration: none;
  display: inline-block;
  padding: 0.75rem 1rem;
  border-radius: 0.65rem;
  font-weight: 700;
}

.btn-primary {
  color: #00120f;
  background: var(--accent);
}

.btn-primary:hover {
  background: var(--accent-dark);
}

.btn-secondary {
  color: var(--text);
  border: 1px solid var(--line);
}

.hero-card {
  background: var(--card);
  border: 1px solid var(--line);
  border-radius: 1rem;
  padding: 1.2rem;
  grid-column: 2;
  grid-row: 1;
}

.hero-card ul {
  padding-left: 1.1rem;
}

.section {
  padding: 4rem 0;
}

.muted {
  background: rgb(15 30 46 / 35%);
}

.section-heading {
  margin-bottom: 1.75rem;
}

.section-heading p {
  color: var(--text-soft);
  max-width: 70ch;
}

.service-grid {
  display: grid;
  grid-template-columns: repeat(3, minmax(0, 1fr));
  gap: 1rem;
  align-items: start;
}

.service-card {
  background: var(--card);
  border: 1px solid var(--line);
  border-radius: 1rem;
  padding: 1rem;
}

.service-card p,
.service-card li {
  color: var(--text-soft);
}

.service-card ul {
  margin: 0;
  padding-left: 1rem;
}

.size-pricing {
  margin: 0.85rem 0 0.95rem;
  padding: 0.65rem 0.75rem;
  border: 1px solid var(--line);
  border-radius: 0.65rem;
  background: rgb(8 19 30 / 60%);
}

.size-pricing p {
  margin: 0 0 0.35rem;
  color: var(--white);
  font-size: 0.88rem;
  font-weight: 700;
}

.size-pricing ul {
  margin: 0;
  padding-left: 1rem;
}

.meta {
  font-size: 0.95rem;
}

.tag {
  display: inline-block;
  background: rgb(45 212 191 / 20%);
  color: var(--accent);
  border: 1px solid rgb(45 212 191 / 45%);
  border-radius: 999px;
  padding: 0.15rem 0.55rem;
  font-size: 0.75rem;
  margin-bottom: 0.6rem;
}

.featured {
  outline: 1px solid rgb(45 212 191 / 50%);
}

.table-wrap {
  border: 1px solid var(--line);
  border-radius: 0.8rem;
  padding: 0.5rem;
  background: rgb(8 19 30 / 45%);
}

.table-inner {
  overflow-x: auto;
  border-radius: 0.65rem;
  background: #f3f6fa;
}

table {
  width: 100%;
  border-collapse: collapse;
  min-width: 880px;
  border-radius: 0.65rem;
  overflow: hidden;
}

th,
td {
  padding: 0.9rem;
  text-align: left;
  border-bottom: 1px solid var(--line);
}

th {
  background: #0f1f31;
  color: #f7fbff;
}

tbody tr {
  background: #f3f6fa;
}

tbody tr:nth-child(even) {
  background: #e9eef5;
}

td {
  color: #233648;
  font-weight: 500;
}

.process-grid {
  display: grid;
  grid-template-columns: repeat(4, minmax(0, 1fr));
  gap: 1rem;
  align-items: start;
}

.process-grid article {
  background: var(--card);
  border: 1px solid var(--line);
  border-radius: 0.9rem;
  padding: 1rem;
}

.process-grid span {
  width: 34px;
  height: 34px;
  display: inline-grid;
  place-items: center;
  border-radius: 50%;
  font-weight: 800;
  margin-bottom: 0.65rem;
  color: #00231f;
  background: var(--accent);
}

.faq-list {
  display: grid;
  gap: 0.65rem;
}

details {
  background: var(--card);
  border: 1px solid var(--line);
  border-radius: 0.8rem;
  padding: 0.85rem 1rem;
}

summary {
  cursor: pointer;
  font-weight: 700;
}

details p {
  color: var(--text-soft);
}

.cta-section {
  padding-bottom: 5rem;
}

.cta-grid {
  display: grid;
  grid-template-columns: 1.3fr 1fr;
  gap: 1rem;
  align-items: start;
}

.contact-card {
  background: var(--card);
  border: 1px solid var(--line);
  border-radius: 0.9rem;
  padding: 1rem;
}

.site-footer {
  border-top: 1px solid var(--line);
  padding: 1.2rem 0 1.8rem;
  color: var(--text-soft);
}

@media (max-width: 980px) {
  .hero-grid,
  .cta-grid {
    grid-template-columns: 1fr;
  }

  .hero-main-card,
  .hero-card {
    grid-column: auto;
    grid-row: auto;
  }

  .service-grid {
    grid-template-columns: repeat(2, minmax(0, 1fr));
  }

  .process-grid {
    grid-template-columns: repeat(2, minmax(0, 1fr));
  }
}

@media (max-width: 640px) {
  .service-grid,
  .process-grid {
    grid-template-columns: 1fr;
  }

  .topbar-content {
    flex-direction: column;
    align-items: flex-start;
  }
}

</style>
  </head>
  <body>
    <header class="topbar">
      <div class="container topbar-content">
        <div class="brand-wrap">
          <a href="#home" class="brand">ZBC Detailing</a>
          <img src="zbc detailing logo.jpg" alt="ZBC Detailing logo" class="brand-logo" />
        </div>
        <nav class="nav-links" aria-label="Main navigation">
          <a href="#services">Services</a>
          <a href="#addons">Add-ons</a>
          <a href="#process">Our Process</a>
          <a href="#faq">FAQ</a>
          <a href="#contact" class="button-link">Book Now</a>
        </nav>
      </div>
    </header>

    <main>
      <section id="home" class="hero">
        <div class="container hero-grid">
          <div class="hero-main-card">
            <p class="eyebrow">Mobile Detailing</p>
            <h1>Big Results, Clear Pricing, and Services Built for Every Vehicle</h1>
            <p class="hero-text">
              From quick maintenance details to full paint correction and ceramic
              protection, ZBC Detailing gives your car, truck, or SUV the care it
              deserves. Choose the package that fits your goals and schedule.
            </p>
            <div class="hero-actions">
              <a href="#services" class="btn btn-primary">Explore Services</a>
              <a href="#contact" class="btn btn-secondary">Get a Quote</a>
            </div>
          </div>
          <aside class="hero-card" aria-label="Business highlights">
            <h2>Why Clients Choose ZBC</h2>
            <ul>
              <li>Clear service tiers with listed time and price</li>
              <li>Interior, exterior, and protection specialists</li>
              <li>Flexible scheduling and fast response</li>
              <li>Quality products safe for all finishes</li>
            </ul>
            <p>
              Need help deciding? We can recommend the best package after a quick
              vehicle assessment.
            </p>
          </aside>
        </div>
      </section>

      <section id="services" class="section">
        <div class="container">
          <div class="section-heading">
            <p class="eyebrow">Core Packages</p>
            <h2>Detailing Services with Time & Price</h2>
            <p>
              Each package includes professional-grade products, attention to
              detail, and a quality check before delivery.
            </p>
          </div>

          <div class="service-grid">
            <article class="service-card">
              <h3>Express Refresh</h3>
              <p class="meta"><strong>Starting at:</strong> $225 | <strong>Time:</strong> 1.5–3 hours</p>
              <p>
                Great for well-kept vehicles that need a quick reset. Restores
                shine and tidiness without a full deep detail.
              </p>
              <div class="size-pricing">
                <p>Vehicle Size Pricing</p>
                <ul>
                  <li>Sedan / Coupe: $225+</li>
                  <li>SUV / Small Truck: $250+</li>
                  <li>3-row SUV: $275+</li>
                  <li>Truck / Van: $300+</li>
                </ul>
              </div>
              <ul>
                <li>Foam hand wash and dry</li>
                <li>Wheel faces cleaned and dressed</li>
                <li>Interior detailed and sanitized</li>
                <li>Windows cleaned inside and out</li>
              </ul>
            </article>

            <article class="service-card featured">
              <p class="tag">Most Popular</p>
              <h3>Complete Interior Detail</h3>
              <p class="meta"><strong>Starting at:</strong> $175 | <strong>Time:</strong> 2–6 hours</p>
              <p>
                Ideal for family cars and daily drivers that need serious inside
                care. Targets dirt, stains, and odors for a refreshed cabin.
              </p>
              <div class="size-pricing">
                <p>Vehicle Size Pricing</p>
                <ul>
                  <li>Sedan / Coupe: $150+</li>
                  <li>Midsize SUV / Small Truck: $175+</li>
                  <li>3-row SUV / Truck / Van: $200+</li>
                </ul>
              </div>
              <ul>
                <li>Deep vacuum and compressed-air crevice cleaning</li>
                <li>Seat extraction if needed</li>
                <li>Leather cleaning and conditioning</li>
                <li>Steam sanitation for high-touch surfaces</li>
                <li>UV protectant on plastics and trim</li>
              </ul>
            </article>

            <article class="service-card">
              <h3>Complete Exterior Detail</h3>
              <p class="meta"><strong>Starting at:</strong> $125 | <strong>Time:</strong> 1–3 hours</p>
              <p>
                Designed for vehicles that have lost gloss and smoothness.
                Removes contamination and boosts paint clarity.
              </p>
              <div class="size-pricing">
                <p>Vehicle Size Pricing</p>
                <ul>
                  <li>Sedan / Coupe: $125+</li>
                  <li>SUV / Small Truck: $150+</li>
                  <li>Truck / Van: $175+</li>
                </ul>
              </div>
              <ul>
                <li>Pre-rinse, foam bath, and contact wash</li>
                <li>tires and trim cleaned</li>
                <li>Spray sealant protection (up to 3 months)</li>
                <li>Tire shine</li>
              </ul>
            </article>

            <article class="service-card">
              <h3>Showroom Signature Full Detail</h3>
              <p class="meta"><strong>Starting at:</strong> $275 | <strong>Time:</strong> 4–6 hours</p>
              <p>
                Full inside-and-out transformation package for clients who want
                a complete reset before events, sale, or long-term care.
              </p>
              <div class="size-pricing">
                <p>Vehicle Size Pricing</p>
                <ul>
                  <li>Sedan / Coupe: $275+</li>
                  <li>Midsize SUV / Small Truck: $325+</li>
                  <li>3-row SUV: $350+</li>
                  <li>Truck / Van: $375+</li>
                </ul>
              </div>
              <ul>
                <li>Everything in Complete Interior + Exterior Detail</li>
              </ul>
            </article>

            <article class="service-card">
              <h3>Paint Correction (2-Step)</h3>
              <p class="meta"><strong>Starting at:</strong> $500 | <strong>Time:</strong> 6–8 hours</p>
              <p>
                Removes light swirls, oxidation, and haze to significantly improve
                paint depth and reflection.
              </p>
              <div class="size-pricing">
                <p>Vehicle Size Pricing</p>
                <ul>
                  <li>Sedan / Coupe: $500+</li>
                  <li>SUV / Small Truck: $600+</li>
                  <li>Truck / Van: $700+</li>
                </ul>
              </div>
              <ul>
                <li>Thorough wash and decontamination prep</li>
                <li>Machine polishing with quality compounds and pads</li>
                <li>Approx. 50–80% defect removal</li>
                <li>Protective sealant application</li>
              </ul>
            </article>

            <article class="service-card">
              <h3>Ceramic Coating Package</h3>
              <p class="meta"><strong>Starting at:</strong> $400 | <strong>Time:</strong> 1–2 days</p>
              <p>
                Best for long-term paint protection and easier maintenance.
                Includes prep and professional coating application.
              </p>
              <div class="size-pricing">
                <p>Vehicle Size Pricing</p>
                <ul>
                  <li>Sedan / Coupe: $400+</li>
                  <li>Midsize SUV / Small Truck: $500+</li>
                  <li>Truck / Van: $600+</li>
                </ul>
              </div>
              <ul>
                <li>Deep decontamination and panel prep</li>
                <li>2-step paint correction before coating (recommended)</li>
                <li>3–5 year ceramic coating</li>
                <li>Aftercare guide and maintenance tips</li>
              </ul>
            </article>
          </div>
        </div>
      </section>

      <section id="addons" class="section muted">
        <div class="container">
          <div class="section-heading">
            <p class="eyebrow">Customization</p>
            <h2>Add-On Services</h2>
            <p>
              Build your perfect detail with optional upgrades that target your
              vehicle’s exact needs.
            </p>
          </div>

          <div class="table-wrap" role="region" aria-label="Add-on pricing table">
            <div class="table-inner">
              <table>
                <thead>
                  <tr>
                    <th>Add-On</th>
                    <th>Price</th>
                    <th>Time</th>
                    <th>Description</th>
                  </tr>
                </thead>
                <tbody>
                  <tr>
                    <td>Pet Hair Removal</td>
                    <td>$35</td>
                    <td>30–90 min</td>
                    <td>Specialized tools and brushes to remove embedded pet hair from carpets and seats.</td>
                  </tr>
                  <tr>
                    <td>Odor Neutralizing Treatment</td>
                    <td>$50</td>
                    <td>60 min</td>
                    <td>Neutralizes smoke, food, and mildew odors for a cleaner cabin smell.</td>
                  </tr>
                  <tr>
                    <td>Headlight Restoration</td>
                    <td>$75</td>
                    <td>45–60 min</td>
                    <td>Removes haze/yellowing and improves nighttime visibility with UV sealant.</td>
                  </tr>
                  <tr>
                    <td>Engine Bay Detail</td>
                    <td>$80</td>
                    <td>30–60 min</td>
                    <td>Safe low-moisture clean and dressing for plastics in engine compartment.</td>
                  </tr>
                  <tr>
                    <td>Fabric Protection</td>
                    <td>$60</td>
                    <td>30 min</td>
                    <td>Hydrophobic treatment to help resist stains on seats and carpet.</td>
                  </tr>
                  <tr>
                    <td>Windshield Ceramic Coating</td>
                    <td>$125</td>
                    <td>60 min</td>
                    <td>Boosts water beading and visibility in heavy rain conditions.</td>
                  </tr>
                  <tr>
                    <td>Seat or floor Extraction (Per Row)</td>
                    <td>$30</td>
                    <td>60 min</td>
                    <td>Deep shampoo extraction for stains, spills, and buildup in cloth seating.</td>
                  </tr>
                </tbody>
              </table>
            </div>
          </div>
        </div>
      </section>

      <section id="process" class="section">
        <div class="container">
          <div class="section-heading">
            <p class="eyebrow">How It Works</p>
            <h2>Simple 4-Step Booking Process</h2>
          </div>
          <div class="process-grid">
            <article>
              <span>1</span>
              <h3>Choose Your Package</h3>
              <p>Pick a service and add-ons based on your goals and budget.</p>
            </article>
            <article>
              <span>2</span>
              <h3>Get Confirmation</h3>
              <p>We confirm vehicle size, condition, location, and appointment time.</p>
            </article>
            <article>
              <span>3</span>
              <h3>Detailing Day</h3>
              <p>Our team performs your selected services with careful quality checks.</p>
            </article>
            <article>
              <span>4</span>
              <h3>Drive Away Protected</h3>
              <p>Receive aftercare guidance so your vehicle stays cleaner longer.</p>
            </article>
          </div>
        </div>
      </section>

      <section id="faq" class="section muted">
        <div class="container">
          <div class="section-heading">
            <p class="eyebrow">Common Questions</p>
            <h2>FAQ</h2>
          </div>
          <div class="faq-list">
            <details>
              <summary>Do prices vary by vehicle size?</summary>
              <p>
                Yes. Listed prices are starting points for standard sedans. Larger
                SUVs, trucks, or heavily soiled vehicles may require an adjusted quote.
              </p>
            </details>
            <details>
              <summary>Do I need to remove personal items?</summary>
              <p>
                Please remove valuables and important paperwork. We can work around
                child seats, but letting us know ahead of time helps with scheduling.
              </p>
            </details>
            <details>
              <summary>How often should I get my vehicle detailed?</summary>
              <p>
                For most daily drivers, every 6–10 weeks is ideal for maintenance.
                If you park outside often or have kids/pets, monthly service helps.
              </p>
            </details>
          </div>
        </div>
      </section>

      <section id="contact" class="section cta-section">
        <div class="container cta-grid">
          <div>
            <p class="eyebrow">Ready to Book?</p>
            <h2>Let’s Get Your Vehicle Looking Its Best</h2>
            <p>
              Call, text, or message us with your vehicle type and preferred service.
              We’ll reply with availability and an exact quote.
            </p>
          </div>
          <div class="contact-card">
            <p><strong>Phone:</strong> 570-390-8696</p>
            <p><strong>Email:</strong> Zbcdetailing@gmail.com</p>
            <p><strong>Hours:</strong> Mon–Sat, 8:00 AM – 6:00 PM</p>
            <a href="mailto:Zbcdetailing@gmail.com" class="btn btn-primary">Request Appointment</a>
          </div>
        </div>
      </section>
    </main>

    <footer class="site-footer">
      <div class="container">
        <p>© <span id="year"></span> ZBC Detailing. All rights reserved.</p>
      </div>
    </footer>

    <script>
const yearElement = document.getElementById('year');
if (yearElement) {
  yearElement.textContent = new Date().getFullYear();
}

</script>
  </body>
</html>
