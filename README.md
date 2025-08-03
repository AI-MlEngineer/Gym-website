# Gym-website
THIS IS MY FIRST GIT REPOSITORY
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>IronForge Gym</title>
  <style>
    * {
      margin: 0;
      padding: 0;
      box-sizing: border-box;
      font-family: Arial, sans-serif;
    }
    body {
      background-color: #121212;
      color: #e0e0e0;
    }
    header {
      background: url('https://images.unsplash.com/photo-1594737625785-c0b68d70d0c1') no-repeat center center/cover;
      height: 100vh;
      display: flex;
      justify-content: center;
      align-items: center;
      text-align: center;
    }
    header h1 {
      font-size: 3rem;
      background: rgba(0, 0, 0, 0.6);
      padding: 20px;
      border-radius: 10px;
    }
    .background-design {
      background: url('https://images.unsplash.com/photo-1554284126-aa88f22d8b74') no-repeat center center/cover;
      height: 80vh;
      display: flex;
      justify-content: center;
      align-items: center;
      text-align: center;
    }
    .background-design h2 {
      font-size: 2.5rem;
      background: rgba(0, 0, 0, 0.5);
      padding: 20px;
      border-radius: 10px;
      color: white;
    }
    nav {
      background-color: #1c1c1c;
      padding: 1rem;
      text-align: center;
    }
    nav a {
      margin: 0 15px;
      color: #ffd700;
      text-decoration: none;
      font-weight: bold;
    }
    section {
      padding: 40px;
      text-align: center;
    }
    .fees-section input {
      padding: 10px;
      margin: 10px;
      width: 200px;
      font-size: 1rem;
    }
    .fees-section button {
      padding: 10px 20px;
      font-size: 1rem;
      background-color: #ffd700;
      color: #000;
      border: none;
      cursor: pointer;
    }
    .fees-section button:hover {
      background-color: #e6c200;
    }
    .quote {
      margin: 40px 0;
      font-size: 1.5rem;
      font-style: italic;
      color: #ccc;
    }
    .video-section {
      padding: 40px;
      text-align: center;
    }
    .video-section h2 {
      margin-bottom: 20px;
      color: #ffd700;
    }
    .video-section iframe {
      width: 80%;
      height: 400px;
      border: none;
      border-radius: 10px;
    }
    .subscription-section {
      padding: 40px;
      background-color: #1c1c1c;
      text-align: center;
    }
    .subscription-section h2 {
      color: #ffd700;
      margin-bottom: 20px;
    }
    .plan {
      margin: 20px auto;
      padding: 20px;
      background-color: #2a2a2a;
      border-radius: 10px;
      width: 80%;
      color: #e0e0e0;
    }
    .plan h3 {
      color: #ffd700;
      margin-bottom: 10px;
    }
    .plan ul {
      list-style: none;
      padding: 0;
    }
    .plan ul li {
      margin: 5px 0;
    }
    .corporate-section {
      background: url('https://images.unsplash.com/photo-1517960413843-0aee8e2b3286') no-repeat center center/cover;
      padding: 60px 20px;
      color: #fff;
      text-align: center;
    }
    .corporate-section h2 {
      margin-bottom: 20px;
      font-size: 2.5rem;
      background: rgba(0, 0, 0, 0.6);
      display: inline-block;
      padding: 10px 20px;
      border-radius: 10px;
      color: #ffd700;
    }
    .corporate-section .program {
      background: rgba(0, 0, 0, 0.7);
      margin: 20px auto;
      padding: 20px;
      border-radius: 10px;
      max-width: 800px;
    }
    .corporate-section .program h3 {
      color: #ffd700;
    }
    .corporate-section .program p {
      font-size: 1rem;
      line-height: 1.6;
    }
    .location-section {
      padding: 60px 20px;
      background-color: #000;
      color: #fff;
      text-align: center;
    }
    .location-section h2 {
      color: #ffd700;
      margin-bottom: 20px;
    }
    .location-list {
      display: flex;
      flex-wrap: wrap;
      justify-content: center;
      gap: 20px;
      padding: 20px 0;
    }
    .location-item {
      background-color: #1c1c1c;
      border-radius: 10px;
      padding: 15px 25px;
      font-size: 1.1rem;
      min-width: 150px;
    }
    footer {
      background-color: #1c1c1c;
      color: #e0e0e0;
      text-align: center;
      padding: 20px;
    }
  </style>
</head>
<body>
  <div class="background-design">
    <h2>Welcome to the Ultimate Fitness Zone</h2>
  </div>

  <header>
    <h1>Welcome to IronForge Gym</h1>
  </header>

  <nav>
    <a href="#home">Home</a>
    <a href="#fees">Calculate Fees</a>
    <a href="#about">About</a>
    <a href="#address">Address</a>
  </nav>

  <section id="home">
    <h2>Build your strength, build your life</h2>
    <div class="quote">"Train insane or remain the same."</div>
  </section>

  <section class="fees-section" id="fees">
    <h2>Calculate Your Gym Fees</h2>
    <input type="number" id="days" placeholder="Enter number of days">
    <button onclick="calculateFees()">Calculate</button>
    <h3 id="result"></h3>
  </section>

  <section id="about">
    <h2>About IronForge Gym</h2>
    <p>IronForge Gym is equipped with state-of-the-art equipment, experienced trainers, and a mission to transform your fitness journey. We are dedicated to helping you reach your maximum potential in strength, endurance, and confidence.</p>
    <div class="quote">"No pain, no gain. Shut up and train."</div>
  </section>

  <section id="address">
    <h2>Visit Us</h2>
    <p>IronForge Gym</p>
    <p>Palam Colony, New Delhi</p>
    <p>Near Kennedy Public School</p>
  </section>

  <section class="video-section">
    <h2>Feel the Power – Gym in Action</h2>
    <iframe src="https://www.youtube.com/embed/0Bmhjf0rKe8?start=10&end=60" title="Motivational Gym Video" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
  </section>

  <section class="subscription-section">
    <h2>Membership Plans</h2>
    <div class="plan">
      <h3>3-Month Plan – ₹4,500</h3>
      <ul>
        <li>Unlimited gym access</li>
        <li>Free 2 personal training sessions</li>
        <li>Basic diet chart & fitness tips</li>
      </ul>
    </div>
    <div class="plan">
      <h3>6-Month Plan – ₹8,000</h3>
      <ul>
        <li>Unlimited gym access</li>
        <li>Weekly fitness assessment</li>
        <li>Access to cardio + weight training zone</li>
        <li>Free consultation with certified nutritionist</li>
      </ul>
    </div>
    <div class="plan">
      <h3>1-Year Plan – ₹14,000</h3>
      <ul>
        <li>All benefits of 6-month plan</li>
        <li>Exclusive access to premium equipment</li>
        <li>Personal locker</li>
        <li>Monthly personal training session</li>
        <li>Discount on gym merchandise</li>
      </ul>
    </div>
  </section>

  <section class="corporate-section">
    <h2>Corporate Wellness Programs</h2>
    <div class="program">
      <h3>IT & Tech Companies</h3>
      <p>Posture correction, stress management & strength training customized for sedentary jobs.</p>
    </div>
    <div class="program">
      <h3>Call Centers & BPOs</h3>
      <p>Energy‑boosting workouts timed for shifts, light cardio, rest-focused sessions.</p>
    </div>
    <div class="program">
      <h3>Finance & Banking</h3>
      <p>HIIT, yoga breaks, and focus-enhancing routines for high-stress workdays.</p>
    </div>
    <div class="program">
      <h3>Team & Group Building</h3>
      <p>Monthly group challenges, bootcamps & fitness marathons to boost employee wellness.</p>
    </div>
  </section>

  <section class="location-section">
    <h2>Our Locations Across India</h2>
    <div class="location-list">
      <div class="location-item">Delhi</div>
      <div class="location-item">Mumbai</div>
      <div class="location-item">Bengaluru</div>
      <div class="location-item">Hyderabad</div>
      <div class="location-item">Pune</div>
      <div class="location-item">Ahmedabad</div>
      <div class="location-item">Chennai</div>
      <div class="location-item">Kolkata</div>
      <div class="location-item">Jaipur</div>
      <div class="location-item">Lucknow</div>
    </div>
  </section>

  <footer>
    <p>&copy; 2025 IronForge Gym. All rights reserved.</p>
  </footer>

  <script>
    function calculateFees() {
      const days = document.getElementById('days').value;
      if (days && days > 0) {
        const total = days * 60;
        document.getElementById('result').innerText = `Total fees for ${days} days is ₹${total}`;
      } else {
        document.getElementById('result').innerText = "Please enter a valid number of days.";
      }
    }
  </script>
</body>
</html>
