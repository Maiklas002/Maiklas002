<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>My Online Store</title>
    <link rel="stylesheet" href="styles.css">
</head>
<body>
    <header>
        <h1>My Online Store</h1>
        <nav>
            <ul>
                <li><a href="#">Home</a></li>
                <li><a href="#products">Products</a></li>
                <li><a href="#about">About</a></li>
                <li><a href="#contact">Contact</a></li>
            </ul>
        </nav>
    </header>

    <main>
        <section id="products">
            <h2>Our Products</h2>
            <div class="product-list">
                <div class="product-item">
                    <img src="product1.jpg" alt="Product 1">
                    <h3>Product 1</h3>
                    <p>$19.99</p>
                    <button onclick="addToCart('Product 1', 19.99)">Add to Cart</button>
                </div>
                <div class="product-item">
                    <img src="product2.jpg" alt="Product 2">
                    <h3>Product 2</h3>
                    <p>$29.99</p>
                    <button onclick="addToCart('Product 2', 29.99)">Add to Cart</button>
                </div>
                <div class="product-item">
                    <img src="product3.jpg" alt="Product 3">
                    <h3>Product 3</h3>
                    <p>$39.99</p>
                    <button onclick="addToCart('Product 3', 39.99)">Add to Cart</button>
                </div>
            </div>
        </section>

        <section id="cart">
            <h2>Shopping Cart</h2>
            <ul id="cart-items">
                <!-- Items will be added here dynamically -->
            </ul>
            <p>Total: $<span id="total-price">0.00</span></p>
            <button onclick="checkout()">Checkout</button>
        </section>

        <section id="about">
            <h2>About Us</h2>
            <p>Learn more about our store and what we offer.</p>
        </section>

        <section id="contact">
            <h2>Contact Us</h2>
            <form id="contact-form">
                <label for="name">Name:</label>
                <input type="text" id="name" name="name" required>

                <label for="email">Email:</label>
                <input type="email" id="email" name="email" required>

                <label for="message">Message:</label>
                <textarea id="message" name="message" required></textarea>

                <button type="submit">Send</button>
            </form>
        </section>
    </main>

    <footer>
        <p>&copy; 2024 My Online Store</p>
    </footer>

    <script src="script.js"></script>
</body>
</html>
