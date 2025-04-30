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
      font-family: Arial, sans-serif;
    }
    body {
      background-color: #f4f4f4;
    }
    header {
      background-color: #222;
      color: white;
      padding: 20px;
      text-align: center;
    }
    nav {
      background-color: #444;
      display: flex;
      justify-content: center;
    }
    nav a {
      color: white;
      padding: 14px 20px;
      text-decoration: none;
      display: inline-block;
    }
    nav a:hover {
      background-color: #111;
    }
    .container {
      padding: 20px;
    }
    .product {
      background-color: white;
      padding: 15px;
      margin: 10px;
      border-radius: 8px;
      box-shadow: 0 0 10px rgba(0,0,0,0.1);
    }
    .product h3 {
      margin-bottom: 10px;
    }
    .product p {
      margin-bottom: 10px;
    }
    form {
      background-color: white;
      padding: 20px;
      border-radius: 8px;
      box-shadow: 0 0 10px rgba(0,0,0,0.1);
    }
    form input, form select, form textarea {
      width: 100%;
      padding: 10px;
      margin: 10px 0;
      border-radius: 5px;
      border: 1px solid #ccc;
    }
    form button {
      padding: 10px 15px;
      background-color: #222;
      color: white;
      border: none;
      border-radius: 5px;
      cursor: pointer;
    }
    form button:hover {
      background-color: #555;
    }
    footer {
      background-color: #222;
      color: white;
      text-align: center;
      padding: 20px;
      margin-top: 30px;
    }
    .hidden { display: none; }
  </style>
</head>
<body>
  <header>
    <h1>Chief's Footwear</h1>
  </header>

  <nav>
    <a href="#shop" onclick="showPage('shop')">SHOP</a>
    <a href="#about" onclick="showPage('about')">ABOUT US</a>
    <a href="#contact" onclick="showPage('contact')">CONTACT US</a>
  </nav>

  <div class="container">

    <div id="shop" class="page">
      <h2>Shop Sneakers</h2>
      <div class="product">
        <h3>White Nike Airforce 1</h3>
        <p>Price: 700 BWP</p>
      </div>
      <div class="product">
        <h3>Nike Jordan 1 University Blue</h3>
        <p>Price: 1200 BWP</p>
      </div>
      <div class="product">
        <h3>Cactus Jack Jordan 6 British Khaki</h3>
        <p>Price: 2500 BWP</p>
      </div>
      <div class="product">
        <h3>Barca x Patta Nike TN</h3>
        <p>Price: 1400 BWP</p>
      </div>
      <div class="product">
        <h3>Lacoste Nike TN</h3>
        <p>Price: 1400 BWP</p>
      </div>
      <div class="product">
        <h3>Corteiz Airmax 95 Honey Black</h3>
        <p>Price: 1600 BWP</p>
      </div>
      <div class="product">
        <h3>Cactus Jack Jordan 1 High Dark Mocha</h3>
        <p>Price: 2000 BWP</p>
      </div>
      <div class="product">
        <h3>Black Puma Suede</h3>
        <p>Price: 900 BWP</p>
      </div>
      <div class="product">
        <h3>Addidas Campus</h3>
        <p>Price: 1000 BWP</p>
      </div>

      <h3>Pre-Order Now</h3>
      <form>
        <input type="text" placeholder="First Name" required>
        <input type="text" placeholder="Last Name" required>
        <input type="email" placeholder="Email" required>
        <input type="text" placeholder="Contact (+267...)" required>
        <input type="text" placeholder="Address" required>
        <select required>
          <option value="">Select Sneaker</option>
          <option>White Nike Airforce 1 - 700 BWP</option>
          <option>Nike Jordan 1 University Blue - 1200 BWP</option>
          <option>Cactus Jack Jordan 6 British Khaki - 2500 BWP</option>
          <option>Barca x Patta Nike TN - 1400 BWP</option>
          <option>Lacoste Nike TN - 1400 BWP</option>
          <option>Corteiz Airmax 95 Honey Black - 1600 BWP</option>
          <option>Cactus Jack Jordan 1 High Dark Mocha - 2000 BWP</option>
          <option>Black Puma Suede - 900 BWP</option>
          <option>Addidas Campus - 1000 BWP</option>
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
  </script>
</body>
</html>
