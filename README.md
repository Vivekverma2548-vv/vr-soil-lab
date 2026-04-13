<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>VR Soil Health Testing Lab</title>
  <style>
    body { font-family: Arial, sans-serif; margin: 0; background: #f4f4f4; }
    header { background: #2e7d32; color: white; padding: 15px; text-align: center; }
    nav { background: #1b5e20; padding: 10px; text-align: center; }
    nav a { color: white; margin: 0 15px; text-decoration: none; font-weight: bold; }
    section { padding: 20px; }
    .card { background: white; padding: 20px; margin: 15px 0; border-radius: 10px; box-shadow: 0 0 10px rgba(0,0,0,0.1); }
    footer { background: #2e7d32; color: white; text-align: center; padding: 10px; }
    input, button { padding: 10px; margin: 5px 0; width: 100%; }
    button { background: #2e7d32; color: white; border: none; cursor: pointer; }
  </style>
</head>
<body>

<header>
  <h1>VR Soil Health Testing Lab</h1>
  <p>Online Soil Testing Report System</p>
</header>

<nav>
  <a href="#home">Home</a>
  <a href="#services">Services</a>
  <a href="#report">Check Report</a>
  <a href="#contact">Contact</a>
</nav>

<section id="home">
  <div class="card">
    <h2>Welcome</h2>
    <p>Welcome to VR Soil Health Testing Lab. We provide accurate soil testing services for farmers to improve crop productivity.</p>
  </div>
</section>

<section id="services">
  <div class="card">
    <h2>Our Services</h2>
    <ul>
      <li>Soil Testing</li>
      <li>Fertilizer Recommendation</li>
      <li>Soil Health Card</li>
    </ul>
  </div>
</section>

<section id="report">
  <div class="card">
    <h2>Check Your Soil Report</h2>
    <p>Enter your Sample ID to view report:</p>
    <input type="text" id="sampleId" placeholder="Enter Sample ID">
    <button onclick="checkReport()">Check Report</button>
    <p id="result"></p>
  </div>
</section>

<section id="contact">
  <div class="card">
    <h2>Contact Us</h2>
    <p><strong>Address:</strong> Bahadur Nagar, Bachhrawan, Raebareli</p>
    <p><strong>Mobile:</strong> 8707418503</p>
    <p><strong>Email:</strong> vivekverma254850@gmail.com</p>
  </div>
</section>

<footer>
  <p>© 2026 VR Soil Health Testing Lab</p>
</footer>

<script>
  function checkReport() {
    var id = document.getElementById("sampleId").value;
    if(id === "123") {
      document.getElementById("result").innerHTML = "Sample ID 123: Soil is Good. Add Nitrogen fertilizer.";
    } else {
      document.getElementById("result").innerHTML = "Report not found. Please contact lab.";
    }
  }
</script>

</body>
</html>
