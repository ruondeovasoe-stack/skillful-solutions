<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Skillful Solutions | #1 Professional Plumber in Houston, Texas</title>
<link rel="preconnect" href="https://fonts.googleapis.com">
<link href="https://fonts.googleapis.com/css2?family=Poppins:wght@400;500;600;700;800&display=swap" rel="stylesheet">
<style>
  * { margin:0; padding:0; box-sizing:border-box; font-family:'Poppins', sans-serif; }
  html { scroll-behavior:smooth; }
  body { background:#f7f9fc; color:#2b2b2b; }
  img { max-width:100%; display:block; }

  /* ===== Top Bar ===== */
  .topbar {
    background:#082c47;
    color:#cfe3f5;
    font-size:13px;
    padding:8px 30px;
    display:flex;
    justify-content:space-between;
    align-items:center;
  }
  .topbar a { color:#f7a600; text-decoration:none; font-weight:600; }

  /* ===== Header ===== */
  header {
    background:#ffffff;
    padding:18px 30px;
    display:flex;
    justify-content:space-between;
    align-items:center;
    position:sticky;
    top:0;
    z-index:999;
    box-shadow:0 2px 15px rgba(0,0,0,0.08);
  }
  .logo {
    font-size:26px;
    font-weight:800;
    color:#0b3d62;
    display:flex;
    align-items:center;
    gap:8px;
  }
  .logo span { color:#f7a600; }
  nav { display:flex; align-items:center; gap:28px; }
  nav a {
    color:#2b2b2b;
    text-decoration:none;
    font-weight:600;
    font-size:15px;
    position:relative;
    transition:0.3s;
  }
  nav a:hover { color:#f7a600; }
  .call-btn-header {
    background:#f7a600;
    color:#0b3d62 !important;
    padding:12px 24px;
    border-radius:30px;
    font-weight:700;
    box-shadow:0 5px 15px rgba(247,166,0,0.4);
    transition:0.3s;
  }
  .call-btn-header:hover { background:#ffb733; transform:translateY(-2px); }

  /* ===== Hero ===== */
  .hero {
    background:linear-gradient(120deg, rgba(8,44,71,0.92), rgba(11,61,98,0.85)), url('https://images.unsplash.com/photo-1607472829322-9eb33ad6d8a2?auto=format&fit=crop&w=1600&q=80');
    background-size:cover;
    background-position:center;
    color:#fff;
    padding:130px 30px 110px;
    text-align:center;
    position:relative;
    overflow:hidden;
  }
  .hero-badge {
    display:inline-block;
    background:rgba(247,166,0,0.15);
    border:1px solid #f7a600;
    color:#f7a600;
    padding:7px 18px;
    border-radius:30px;
    font-size:13px;
    font-weight:600;
    margin-bottom:20px;
    letter-spacing:0.5px;
  }
  .hero h1 {
    font-size:46px;
    font-weight:800;
    margin-bottom:18px;
    line-height:1.3;
  }
  .hero h1 span { color:#f7a600; }
  .hero p {
    font-size:18px;
    color:#dce9f5;
    max-width:650px;
    margin:0 auto 35px;
    line-height:1.6;
  }
  .hero-buttons { display:flex; justify-content:center; gap:18px; flex-wrap:wrap; }
  .call-now-btn {
    display:inline-flex;
    align-items:center;
    gap:10px;
    background:#f7a600;
    color:#0b3d62;
    font-size:18px;
    font-weight:700;
    padding:17px 38px;
    border-radius:50px;
    text-decoration:none;
    box-shadow:0 10px 25px rgba(0,0,0,0.3);
    transition:0.3s;
  }
  .call-now-btn:hover { background:#ffb733; transform:scale(1.05); }
  .secondary-btn {
    display:inline-flex;
    align-items:center;
    gap:10px;
    background:transparent;
    color:#fff;
    font-size:18px;
    font-weight:600;
    padding:16px 34px;
    border-radius:50px;
    border:2px solid rgba(255,255,255,0.5);
    text-decoration:none;
    transition:0.3s;
  }
  .secondary-btn:hover { background:rgba(255,255,255,0.1); border-color:#fff; }

  /* Trust strip */
  .trust-strip {
    background:#fff;
    padding:25px 20px;
    display:flex;
    justify-content:center;
    flex-wrap:wrap;
    gap:45px;
    box-shadow:0 4px 15px rgba(0,0,0,0.05);
  }
  .trust-item { display:flex; align-items:center; gap:10px; font-weight:600; color:#0b3d62; font-size:15px; }
  .trust-item .num { font-size:22px; }

  /* ===== Section Heading ===== */
  .section { padding:90px 30px; max-width:1180px; margin:auto; }
  .section-head { text-align:center; margin-bottom:55px; }
  .section-head .tag {
    color:#f7a600;
    font-weight:700;
    font-size:14px;
    letter-spacing:1.5px;
    text-transform:uppercase;
  }
  .section-head h2 {
    color:#0b3d62;
    font-size:36px;
    font-weight:800;
    margin-top:10px;
  }
  .section-head p { color:#6b7b8c; max-width:550px; margin:14px auto 0; font-size:15.5px; }

  /* ===== Services ===== */
  .services-grid {
    display:grid;
    grid-template-columns:repeat(auto-fit, minmax(270px,1fr));
    gap:28px;
  }
  .service-card {
    background:#fff;
    padding:38px 28px;
    border-radius:16px;
    text-align:left;
    box-shadow:0 8px 25px rgba(0,0,0,0.06);
    transition:0.35s;
    border-top:4px solid transparent;
  }
  .service-card:hover {
    transform:translateY(-10px);
    box-shadow:0 15px 35px rgba(11,61,98,0.15);
    border-top:4px solid #f7a600;
  }
  .service-card .icon {
    width:60px; height:60px;
    background:linear-gradient(135deg,#0b3d62,#145a8c);
    border-radius:14px;
    display:flex; align-items:center; justify-content:center;
    font-size:28px;
    margin-bottom:20px;
  }
  .service-card h3 { color:#0b3d62; margin-bottom:10px; font-size:19px; }
  .service-card p { color:#6b7b8c; font-size:14.5px; line-height:1.6; }

  /* ===== About ===== */
  .about {
    background:linear-gradient(135deg,#0b3d62,#082c47);
    color:#fff;
    padding:90px 30px;
  }
  .about-grid {
    max-width:1180px;
    margin:auto;
    display:grid;
    grid-template-columns:1fr 1fr;
    gap:60px;
    align-items:center;
  }
  .about-grid img { border-radius:18px; box-shadow:0 20px 50px rgba(0,0,0,0.4); }
  .about-text .tag { color:#f7a600; font-weight:700; font-size:14px; letter-spacing:1.5px; text-transform:uppercase; }
  .about-text h2 { font-size:32px; font-weight:800; margin:12px 0 20px; }
  .about-text p { color:#cfe0ef; line-height:1.8; margin-bottom:25px; font-size:15.5px; }
  .why-grid { display:grid; grid-template-columns:1fr 1fr; gap:18px; }
  .why-item { display:flex; align-items:flex-start; gap:12px; }
  .why-item .chk {
    background:#f7a600; color:#0b3d62; min-width:26px; height:26px;
    border-radius:50%; display:flex; align-items:center; justify-content:center;
    font-weight:800; font-size:14px;
  }
  .why-item p { font-size:14.5px; color:#dce9f5; margin:0; }

  @media(max-width:768px){ .about-grid{ grid-template-columns:1fr; } }

  /* ===== CTA Strip ===== */
  .cta-strip {
    background:linear-gradient(90deg,#f7a600,#ffb733);
    text-align:center;
    padding:55px 20px;
  }
  .cta-strip h2 { color:#0b3d62; margin-bottom:10px; font-size:30px; font-weight:800; }
  .cta-strip p { color:#5a4000; margin-bottom:25px; font-size:16px; }
  .cta-strip .call-now-btn { background:#0b3d62; color:#fff; }
  .cta-strip .call-now-btn:hover { background:#124d7a; }

  /* ===== Testimonials ===== */
  .testimonial-grid {
    display:grid;
    grid-template-columns:repeat(auto-fit, minmax(300px,1fr));
    gap:28px;
  }
  .testimonial-card {
    background:#fff;
    padding:32px;
    border-radius:16px;
    box-shadow:0 8px 25px rgba(0,0,0,0.06);
  }
  .stars { color:#f7a600; font-size:16px; margin-bottom:14px; }
  .testimonial-card p { color:#4b5b6c; font-size:14.5px; line-height:1.7; margin-bottom:18px; font-style:italic; }
  .testimonial-author { display:flex; align-items:center; gap:12px; }
  .avatar {
    width:42px; height:42px; border-radius:50%;
    background:#0b3d62; color:#fff; display:flex; align-items:center; justify-content:center;
    font-weight:700;
  }
  .testimonial-author h4 { font-size:14.5px; color:#0b3d62; }
  .testimonial-author span { font-size:12.5px; color:#8a97a5; }

  /* ===== Contact ===== */
  .contact-wrap {
    background:#fff;
    border-radius:20px;
    box-shadow:0 15px 50px rgba(0,0,0,0.08);
    display:grid;
    grid-template-columns:1fr 1fr;
    overflow:hidden;
  }
  .contact-info {
    background:linear-gradient(135deg,#0b3d62,#082c47);
    color:#fff;
    padding:55px 40px;
  }
  .contact-info h2 { font-size:28px; font-weight:800; margin-bottom:15px; }
  .contact-info p { color:#cfe0ef; margin-bottom:30px; font-size:14.5px; line-height:1.7; }
  .contact-item { display:flex; align-items:center; gap:14px; margin-bottom:22px; }
  .contact-item .ic {
    background:rgba(247,166,0,0.15); width:44px; height:44px; border-radius:10px;
    display:flex; align-items:center; justify-content:center; font-size:18px;
  }
  .contact-item a, .contact-item span { color:#fff; text-decoration:none; font-weight:600; font-size:14.5px; }
  .contact-cta {
    padding:55px 40px;
    display:flex;
    flex-direction:column;
    justify-content:center;
    align-items:center;
    text-align:center;
  }
  .contact-cta h3 { color:#0b3d62; font-size:24px; margin-bottom:12px; font-weight:800; }
  .contact-cta p { color:#6b7b8c; margin-bottom:28px; font-size:14.5px; }

  @media(max-width:768px){ .contact-wrap{ grid-template-columns:1fr; } }

  /* ===== Footer ===== */
  footer {
    background:#082c47;
    color:#9db6cc;
    text-align:center;
    padding:30px;
    font-size:13.5px;
  }
  footer span { color:#f7a600; font-weight:700; }

  /* Floating call button mobile */
  .floating-call {
    display:none;
    position:fixed;
    bottom:20px; right:20px;
    background:#f7a600;
    color:#0b3d62;
    width:60px; height:60px;
    border-radius:50%;
    align-items:center; justify-content:center;
    font-size:26px;
    box-shadow:0 10px 25px rgba(0,0,0,0.3);
    z-index:999;
    text-decoration:none;
  }

  @media(max-width:768px){
    nav { display:none; }
    .hero h1 { font-size:30px; }
    .hero p { font-size:15.5px; }
    .floating-call { display:flex; }
  }
</style>
</head>
<body>

<div class="topbar">
  <span>📍 Serving Houston, TX & Surrounding Areas</span>
  <span>24/7 Emergency Service: <a href="tel:+18337046186">+1 (833) 704-6186</a></span>
</div>

<header>
  <div class="logo">🔧 Skillful <span>Solutions</span></div>
  <nav>
    <a href="#services">Services</a>
    <a href="#about">About</a>
    <a href="#testimonials">Reviews</a>
    <a href="#contact">Contact</a>
  </nav>
  <a href="tel:+18337046186" class="call-btn-header">📞 Call Now</a>
</header>

<section class="hero">
  <div class="hero-badge">⭐ Houston's #1 Rated Plumbing Company</div>
  <h1>Fast, Reliable <span>Plumbing Services</span><br>You Can Trust</h1>
  <p>Licensed & insured plumbers delivering top-quality repairs, installations, and emergency services — 24 hours a day, 7 days a week.</p>
  <div class="hero-buttons">
    <a href="tel:+18337046186" class="call-now-btn">📞 Call Now: +1 (833) 704-6186</a>
    <a href="#services" class="secondary-btn">View Services →</a>
  </div>
</section>

<div class="trust-strip">
  <div class="trust-item"><span class="num">⭐</span> 4.9/5 Rating</div>
  <div class="trust-item"><span class="num">🛡️</span> Licensed & Insured</div>
  <div class="trust-item"><span class="num">⏱️</span> 24/7 Emergency Service</div>
  <div class="trust-item"><span class="num">💯</span> 100% Satisfaction Guaranteed</div>
</div>

<section class="section" id="services">
  <div class="section-head">
    <div class="tag">What We Offer</div>
    <h2>Our Plumbing Services</h2>
    <p>From minor repairs to major installations, our expert team handles it all with precision and care.</p>
  </div>
  <div class="services-grid">
    <div class="service-card">
      <div class="icon">🚰</div>
      <h3>Leak Detection & Repair</h3>
      <p>Advanced leak detection technology to find and fix leaks before they cause major damage.</p>
    </div>
    <div class="service-card">
      <div class="icon">🔧</div>
      <h3>Drain Cleaning</h3>
      <p>Professional hydro-jetting and snaking services to clear even the toughest clogs.</p>
    </div>
    <div class="service-card">
      <div class="icon">🚿</div>
      <h3>Water Heater Services</h3>
      <p>Installation, repair & maintenance for all tank and tankless water heater models.</p>
    </div>
    <div class="service-card">
      <div class="icon">🛁</div>
      <h3>Bathroom Remodeling</h3>
      <p>Complete bathroom plumbing upgrades, fixture installs, and renovation support.</p>
    </div>
    <div class="service-card">
      <div class="icon">🏠</div>
      <h3>Residential Plumbing</h3>
      <p>Comprehensive home plumbing solutions for every room and every issue.</p>
    </div>
    <div class="service-card">
      <div class="icon">🏢</div>
      <h3>Commercial Plumbing</h3>
      <p>Reliable, code-compliant plumbing services for offices, retail & commercial spaces.</p>
    </div>
  </div>
</section>

<section class="about" id="about">
  <div class="about-grid">
    <img src="https://images.unsplash.com/photo-1621905251189-08b45d6a269e?auto=format&fit=crop&w=800&q=80" alt="Professional Plumber at Work">
    <div class="about-text">
      <div class="tag">Why Choose Us</div>
      <h2>Houston's Most Trusted Plumbing Experts</h2>
      <p>At Skillful Solutions, we combine years of hands-on experience with honest pricing and top-tier workmanship. Our licensed plumbers are committed to solving your plumbing problems right the first time.</p>
      <div class="why-grid">
        <div class="why-item"><div class="chk">✓</div><p>Licensed & Insured Team</p></div>
        <div class="why-item"><div class="chk">✓</div><p>24/7 Emergency Response</p></div>
        <div class="why-item"><div class="chk">✓</div><p>Upfront, Honest Pricing</p></div>
        <div class="why-item"><div class="chk">✓</div><p>100% Satisfaction Guarantee</p></div>
      </div>
    </div>
  </div>
</section>

<div class="cta-strip">
  <h2>Got a Plumbing Emergency?</h2>
  <p>Our team is standing by 24/7 to help with any plumbing issue, big or small.</p>
  <a href="tel:+18337046186" class="call-now-btn">📞 Call Now: +1 (833) 704-6186</a>
</div>

<section class="section" id="testimonials">
  <div class="section-head">
    <div class="tag">Testimonials</div>
    <h2>What Our Customers Say</h2>
  </div>
  <div class="testimonial-grid">
    <div class="testimonial-card">
      <div class="stars">★★★★★</div>
      <p>"Fast response, fair pricing, and excellent work. Fixed our water heater same day!"</p>
      <div class="testimonial-author">
        <div class="avatar">J</div>
        <div><h4>James R.</h4><span>Houston, TX</span></div>
      </div>
    </div>
    <div class="testimonial-card">
      <div class="stars">★★★★★</div>
      <p>"Professional, clean, and courteous. Highly recommend Skillful Solutions for any plumbing need."</p>
      <div class="testimonial-author">
        <div class="avatar">M</div>
        <div><h4>Maria S.</h4><span>Houston, TX</span></div>
      </div>
    </div>
    <div class="testimonial-card">
      <div class="stars">★★★★★</div>
      <p>"Called them for an emergency leak at midnight — they showed up within an hour. Amazing service!"</p>
      <div class="testimonial-author">
        <div class="avatar">D</div>
        <div><h4>David K.</h4><span>Houston, TX</span></div>
      </div>
    </div>
  </div>
</section>

<section class="section" id="contact">
  <div class="section-head">
    <div class="tag">Get In Touch</div>
    <h2>Contact Skillful Solutions</h2>
  </div>
  <div class="contact-wrap">
    <div class="contact-info">
      <h2>Let's Fix Your Plumbing Issue Today</h2>
      <p>Reach out anytime — we're available 24/7 for emergencies and scheduled appointments.</p>
      <div class="contact-item"><div class="ic">📞</div><a href="tel:+18337046186">+1 (833) 704-6186</a></div>
      <div class="contact-item"><div class="ic">📍</div><span>Houston, Texas & Surrounding Areas</span></div>
      <div class="contact-item"><div class="ic">🕒</div><span>Available 24/7, Including Weekends</span></div>
    </div>
    <div class="contact-cta">
      <h3>Need Help Right Now?</h3>
      <p>Speak directly with our plumbing experts — no waiting, no hassle.</p>
      <a href="tel:+18337046186" class="call-now-btn">📞 Call Now</a>
    </div>
  </div>
</section>

<footer>
  <p>© 2026 <span>Skillful Solutions</span> — All Rights Reserved | Houston, Texas</p>
</footer>

<a href="tel:+18337046186" class="floating-call">📞</a>

</body>
</html>
