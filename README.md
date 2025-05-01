<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Chief's Footwear</title>
  <style>
    /* ... existing styles ... */
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
          <img src="airforce1.jpg" alt="White Nike Airforce 1">
          <h3>White Nike Airforce 1</h3>
          <p>Price: 700 BWP</p>
        </div>
        <div class="product">
          <img src="jordan1blue.jpg" alt="Nike Jordan 1 University Blue">
          <h3>Nike Jordan 1 University Blue</h3>
          <p>Price: 1200 BWP</p>
        </div>
        <div class="product">
          <img src="jordan6khaki.jpg" alt="Cactus Jack Jordan 6 British Khaki">
          <h3>Cactus Jack Jordan 6 British Khaki</h3>
          <p>Price: 2500 BWP</p>
        </div>
        <div class="product">
          <img src="barca_patta_tn.jpg" alt="Barca x Patta Nike TN">
          <h3>Barca x Patta Nike TN</h3>
          <p>Price: 1400 BWP</p>
        </div>
        <div class="product">
          <img src="lacoste_tn.jpg" alt="Lacoste Nike TN">
          <h3>Lacoste Nike TN</h3>
          <p>Price: 1400 BWP</p>
        </div>
        <div class="product">
          <img src="corteiz_airmax.jpg" alt="Corteiz Airmax 95 Honey Black">
          <h3>Corteiz Airmax 95 Honey Black</h3>
          <p>Price: 1600 BWP</p>
        </div>
        <div class="product">
          <img src="jordan1mocha.jpg" alt="Cactus Jack Jordan 1 High Dark Mocha">
          <h3>Cactus Jack Jordan 1 High Dark Mocha</h3>
          <p>Price: 2000 BWP</p>
        </div>
        <div class="product">
          <img src="puma_suede.jpg" alt="Black Puma Suede">
          <h3>Black Puma Suede</h3>
          <p>Price: 900 BWP</p>
        </div>
        <div class="product">
          <img src="adidas_campus.jpg" alt="Adidas Campus">
          <h3>Adidas Campus</h3>
          <p>Price: 1000 BWP</p>
        </div>
      </div>
      <form>
        <h3>Pre-Order Now</h3>
        <input type="text" placeholder="First Name" required>
        <input type="text" placeholder="Last Name" required>
        <input type="email" placeholder="Email" required>
        <input type="text" placeholder="Contact (+267)" required>
        <input type="text" placeholder="Address" required>
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
