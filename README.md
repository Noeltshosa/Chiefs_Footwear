<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Chief's Footwear</title>
  <style>
    body {
      background-image: Graffiti art_Chief's Footwear.png;
      background-size: cover;
      background-repeat:no-repeat;
      background-attachment:fixed;
      background position:center;
      color:black;
      min-height:100vh;
      margin: 0;
    }

    header, footer {
      background-color: #111;
      text-align: center;
      padding: 1em;
    }

    nav {
      background-color: #222;
      display: flex;
      justify-content: center;
      gap: 1em;
      padding: 1em;
    }

    nav a {
      color: #fff;
      text-decoration: none;
      padding: 0.5em 1em;
      background-color: #444;
      border-radius: 5px;
    }

    nav a:hover {
      background-color: #666;
    }

    .container {
      padding: 2em;
    }

    .hidden {
      display: none;
    }

    .home-buttons a {
      display: inline-block;
      margin: 0.5em;
      padding: 0.5em 1em;
      background-color: #444;
      color: #fff;
      text-decoration: none;
      border-radius: 5px;
    }

    .grid {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(200px, 1fr));
      gap: 1em;
    }

    .product {
      background-color: #1a1a1a;
      border: 1px solid #333;
      border-radius: 10px;
      padding: 1em;
      text-align: center;
    }

    .product img {
      max-width: 100%;
      height: auto;
      border-radius: 5px;
    }

    form {
      background-color: #111;
      padding: 1em;
      margin-top: 2em;
      border-radius: 10px;
    }

    form input, form select {
      width: 100%;
      padding: 0.5em;
      margin: 0.5em 0;
      border: none;
      border-radius: 5px;
    }

    form button {
      padding: 0.5em 1em;
      background-color: #444;
      color: #fff;
      border: none;
      border-radius: 5px;
      cursor: pointer;
    }

    form button:hover {
      background-color: #666;
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
        <div class="product">
          <img src="White airforce 1.jpeg" alt="White Nike Airforce 1">
          <h3>White Nike Airforce 1</h3>
          <p>Price: 700 BWP</p>
        </div>
        <div class="product">
          <img src="Nike Jordan 1 university blue.jpeg" alt="Nike Jordan 1 University Blue">
          <h3>Nike Jordan 1 University Blue</h3>
          <p>Price: 1200 BWP</p>
        </div>
        <div class="product">
          <img src="Jordan 6 cactus jack british khaki img.png" alt="Cactus Jack Jordan 6 British Khaki">
          <h3>Cactus Jack Jordan 6 British Khaki</h3>
          <p>Price: 2500 BWP</p>
        </div>
        <div class="product">
          <img src="barca x patta tn.jpeg" alt="Barca x Patta Nike TN">
          <h3>Barca x Patta Nike TN</h3>
          <p>Price: 1400 BWP</p>
        </div>
        <div class="product">
          <img src="lacoste tn img.jpeg" alt="Lacoste Nike TN">
          <h3>Lacoste Nike TN</h3>
          <p>Price: 1400 BWP</p>
        </div>
        <div class="product">
          <img src="Corteiz honey black img.png" alt="Corteiz Airmax 95 Honey Black">
          <h3>Corteiz Airmax 95 Honey Black</h3>
          <p>Price: 1600 BWP</p>
        </div>
        <div class="product">
          <img src="cactus jack Jordan 1 high dark mocha img.jpeg" alt="Cactus Jack Jordan 1 High Dark Mocha">
          <h3>Cactus Jack Jordan 1 High Dark Mocha</h3>
          <p>Price: 2000 BWP</p>
        </div>
        <div class="product">
          <img src="black puma suede.jpeg" alt="Black Puma Suede">
          <h3>Black Puma Suede</h3>
          <p>Price: 900 BWP</p>
        </div>
        <div class="product">
          <img src="adidas campus.jpeg" alt="Adidas Campus">
          <h3>Adidas Campus</h3>
          <p>Price: 1000 BWP</p>
        </div>
      </div>
      <form>
        <h3>Pre-Order Now</h3>
        <input type="text" placeholder="First Name" required>
        <input type="text" placeholder="Surname" required>
        <input type="email" placeholder="Email" required>
        <input type="text" placeholder="Contact (+267)" required>
        <input type="text" placeholder="Postal Address" required>
        <input type="text" placeholder="Shoe size" required>
        <select required>
          <option value="">Select a Sneaker</option>
          <option>White Nike Airforce 1 - 700 BWP</option>
          <option>Nike Jordan 1 University Blue - 1200 BWP</option>
          <option>Cactus Jack Jordan 6 British Khaki - 2500 BWP</option>
          <option>Barca x Patta Nike TN - 1400 BWP</option>
          <option>Lacoste Nike TN - 1400 BWP</option>
          <option>Corteiz Airmax 95 Honey Black - 1600 BWP</option>
          <option>Cactus Jack Jordan 1 High Dark Mocha - 2000 BWP</option>
          <option>Black Puma Suede - 900 BWP</option>
          <option>Adidas Campus - 1000 BWP</option>
        </select>
        <button type="submit">Checkout</button>
      </form>
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
    <p>&copy; 2025 Chief's Footwear. All rights reserved.By Mr Noel N. Tshosa</p>
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

