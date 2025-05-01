
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Chief's Footwear</title>
  <style>
    * {
      margin: 0;
      padding: 0;
      box-sizing: border-box;
      font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
    }
    body {
      background: url('graffiti_background.jpg') no-repeat center center fixed;
      background-size: cover;
      color: white;
    }
    header {
      background-color: rgba(0,0,0,0.6);
      color: white;
      padding: 20px;
      text-align: center;
    }
    nav {
      background-color: rgba(0,0,0,0.8);
      display: flex;
      justify-content: center;
    }
    nav a {
      color: white;
      padding: 14px 20px;
      text-decoration: none;
    }
    nav a:hover {
      background-color: rgba(255,255,255,0.2);
    }
    .container {
      padding: 20px;
    }
    .grid {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
      gap: 20px;
    }
    .product {
      background-color: rgba(255,255,255,0.1);
      padding: 15px;
      border-radius: 10px;
      box-shadow: 0 2px 10px rgba(0,0,0,0.3);
      transition: transform 0.3s ease;
    }
    .product:hover {
      transform: translateY(-5px);
    }
    .product img {
      width: 100%;
      border-radius: 10px;
      margin-bottom: 10px;
    }
    form {
      background-color: rgba(255,255,255,0.1);
      padding: 20px;
      border-radius: 10px;
      box-shadow: 0 2px 10px rgba(0,0,0,0.3);
      margin-top: 30px;
    }
    form input, form select {
      width: 100%;
      padding: 12px;
      margin: 10px 0;
      border-radius: 5px;
      border: none;
    }
    form button {
      padding: 12px 20px;
      background-color: black;
      color: white;
      border: none;
      border-radius: 5px;
      cursor: pointer;
    }
    form button:hover {
      background-color: white;
      color: black;
    }
    footer {
      background-color: rgba(0,0,0,0.6);
      color: white;
      text-align: center;
      padding: 20px;
      margin-top: 40px;
    }
    .hidden { display: none; }
    .home-buttons {
      display: flex;
      justify-content: center;
      gap: 20px;
      margin-top: 40px;
    }
    .home-buttons a {
      background-color: rgba(0,0,0,0.7);
      color: white;
      padding: 15px 30px;
      text-decoration: none;
      border-radius: 8px;
      font-size: 18px;
    }
    .home-buttons a:hover {
      background-color: rgba(255,255,255,0.2);
    }
  </style>
</head>
<body>
  <header>
    <h1>Chief's Footwear</h1>
  </header>

  <nav>
    <a href="#home" onclick="showPage('home')">HOME</a>
    <a href="#shop" onclick="showPage('shop')">SHOP</a>
    <a href="#about" onclick="showPage('about')">ABOUT US</a>
    <a href="#contact" onclick="showPage('contact')">CONTACT US</a>
  </nav>

  <div class="container">
    <div id="home" class="page">
      <h2>Welcome to Chief's Footwear</h2>
      <p>Step into the culture. Exclusive sneakers, all in one place.</p>
      <div class="home-buttons">
        <a href="#" onclick="showPage('shop')">Shop Now</a>
        <a href="#" onclick="showPage('about')">Learn More</a>
        <a href="#" onclick="showPage('contact')">Get in Touch</a>
      </div>
    </div>

    <div id="shop" class="page hidden">
      <h2>Shop Sneakers</h2>
      <div class="grid">
        <!-- Sneaker product cards go here (same as before) -->
      </div>
      <!-- Pre-order form goes here (same as before) -->
    </div>

    <div id="about" class="page hidden">
      <h2>About Us</h2>
      <p>Welcome to Chief's Footwear – your go-to online sneaker shop. We offer premium and exclusive sneakers to match your streetwear style. Shop conveniently and pre-order limited editions from the comfort of your home.</p>
    </div>

    <div id="contact" class="page hidden">
      <h2>Contact Us</h2>
      <p>Phone: +267 77545281</p>
      <p>Email: <a href="mailto:nntshosa@gmail.com">nntshosa@gmail.com</a></p>
    </div>
  </div>

  <footer>
    <p>&copy; 2025 Chief's Footwear. All rights reserved.</p>
  </footer>

  <script>
    function showPage(pageId) {
      document.querySelectorAll('.page').forEach(page => {
        page.classList.add('hidden');
      });
      document.getElementById(pageId).classList.remove('hidden');
    }

    // Show home by default
    window.onload = () => showPage('home');
  </script>
</body>
</html>
