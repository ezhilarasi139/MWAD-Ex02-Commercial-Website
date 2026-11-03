
# Ex02 Commercial Website
## Date: 03.11.2026

## AIM
To create a commercial website using CSS Flexbox.

## ALGORITHM
### STEP 1
Create an HTML file (index.html)

### STEP 2
Create a CSS file (style.css)

### STEP 3
Include a navigation bar with links to different sections.

### STEP 4
Add structured sections for Homepage, Products / Services, About Us, Contact Details and User Account.

### STEP 5
Include social media links at the footer with copyright information.

### STEP 6
Define global styles for fonts, colors, and layout.

### STEP 7
Style the header, navigation bar, and sections.

### STEP 8
Use Flexbox for layout design.

### STEP 9
Add hover effects and transitions for interactivity.

### STEP 10
Add Images and Media.

### STEP 11
Use optimized images for a professional look.

### STEP 12
Open the HTML file in a browser to check layout and functionality.

### STEP 13
Fix styling issues and refine content placement.

### STEP 14
Deploy the website.

### STEP 15
Upload to GitHub Pages for free hosting.

## PROGRAM
###index.html
```

<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>ShopEase - Online Shopping</title>
    <link rel="stylesheet" href="style.css">
</head>
<body>

    <!-- Header -->
    <header>
        <h1>ShopEase</h1>
        <nav>
            <a href="#home">Home</a>
            <a href="#products">Products</a>
            <a href="#about">About Us</a>
            <a href="#contact">Contact</a>
            <a href="#account">Account</a>
        </nav>
    </header>

    <!-- Home Section -->
    <section id="home" class="hero">
        <h2>Welcome to ShopEase</h2>
        <p>Discover amazing products at the best prices!</p>
        <a href="#products" class="btn">Shop Now</a>
    </section>

    <!-- Products Section -->
    <section id="products">
        <h2>Our Products</h2>

        <div class="product-container">

            <div class="product">
                <img src="https://images.unsplash.com/photo-1505740420928-5e560c06d30e?w=500" alt="Headphones">
                <h3>Headphones</h3>
                <p>Price: ₹999</p>
                <button>Buy Now</button>
            </div>

            <div class="product">
                <img src="https://images.unsplash.com/photo-1523275335684-37898b6baf30?w=500" alt="Watch">
                <h3>Smart Watch</h3>
                <p>Price: ₹1499</p>
                <button>Buy Now</button>
            </div>

            <div class="product">
                <img src="https://images.unsplash.com/photo-1542291026-7eec264c27ff?w=500" alt="Shoes">
                <h3>Sports Shoes</h3>
                <p>Price: ₹1999</p>
                <button>Buy Now</button>
            </div>

        </div>
    </section>

    <!-- About Us -->
    <section id="about">
        <h2>About Us</h2>
        <p>
            ShopEase is an online shopping website that provides
            quality products at affordable prices.
            Our goal is to make shopping simple and convenient.
        </p>
    </section>

    <!-- Contact -->
    <section id="contact">
        <h2>Contact Us</h2>
        <p>Email: support@shopease.com</p>
        <p>Phone: +91 9876543210</p>
    </section>

    <!-- User Account -->
    <section id="account">
        <h2>User Account</h2>
        <p>Welcome! Manage your shopping account here.</p>
        <button>Login</button>
        <button>Register</button>
    </section>

    <!-- Footer -->
    <footer>
        <p>Follow Us</p>
        <div class="social">
            <a href="https://www.instagram.com/">Instagram</a>
            <a href="https://www.facebook.com/">Facebook</a>
            <a href="https://www.youtube.com/">YouTube</a>
        </div>
        <p>© 2026 ShopEase. All Rights Reserved.</p>
    </footer>

</body>
</html>

```
### style.css

```

/* Global Styles */
* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
    font-family: Arial, sans-serif;
}

html {
    scroll-behavior: smooth;
}

body {
    background-color: #f5f5f5;
    color: #333;
}

/* Header */
header {
    background-color: #172554;
    color: white;
    padding: 20px 40px;
    display: flex;
    justify-content: space-between;
    align-items: center;
    flex-wrap: wrap;
}

header h1 {
    color: #facc15;
}

nav {
    display: flex;
    gap: 25px;
    flex-wrap: wrap;
}

nav a {
    color: white;
    text-decoration: none;
    font-weight: bold;
    transition: 0.3s;
}

nav a:hover {
    color: #facc15;
}

/* Home Section */
.hero {
    background: linear-gradient(120deg, #2563eb, #7c3aed);
    color: white;
    text-align: center;
    padding: 100px 20px;
}

.hero h2 {
    font-size: 40px;
    margin-bottom: 15px;
}

.hero p {
    font-size: 18px;
    margin-bottom: 25px;
}

.btn {
    display: inline-block;
    background-color: #facc15;
    color: #172554;
    padding: 12px 25px;
    text-decoration: none;
    border-radius: 5px;
    font-weight: bold;
}

/* Common Sections */
section {
    padding: 50px 30px;
    text-align: center;
}

section h2 {
    margin-bottom: 25px;
    color: #172554;
}

/* Products Section - Flexbox */
.product-container {
    display: flex;
    justify-content: center;
    align-items: stretch;
    gap: 25px;
    flex-wrap: wrap;
}

.product {
    background-color: white;
    width: 280px;
    padding: 20px;
    border-radius: 10px;
    box-shadow: 0 3px 10px rgba(0,0,0,0.1);
    transition: 0.3s;
}

.product:hover {
    transform: translateY(-8px);
    box-shadow: 0 8px 20px rgba(0,0,0,0.2);
}

.product img {
    width: 100%;
    height: 180px;
    object-fit: cover;
    border-radius: 8px;
}

.product h3 {
    margin: 15px 0;
}

.product p {
    margin-bottom: 15px;
}

/* Buttons */
button {
    background-color: #2563eb;
    color: white;
    border: none;
    padding: 10px 20px;
    border-radius: 5px;
    cursor: pointer;
    transition: 0.3s;
}

button:hover, .btn:hover {
    background-color: #f59e0b;
    color: white;
}

/* About and Contact */
#about, #contact {
    background-color: white;
    margin-top: 10px;
}

#about p, #contact p {
    line-height: 1.8;
}

/* User Account */
#account {
    background-color: #e0e7ff;
}

#account button {
    margin: 10px;
}

/* Footer */
footer {
    background-color: #172554;
    color: white;
    text-align: center;
    padding: 25px;
}

.social {
    display: flex;
    justify-content: center;
    gap: 25px;
    margin: 15px 0;
    flex-wrap: wrap;
}

.social a {
    color: #facc15;
    text-decoration: none;
}

.social a:hover {
    color: white;
}

/* Responsive Design */
@media (max-width: 600px) {
    header {
        flex-direction: column;
        gap: 20px;
    }

    nav {
        justify-content: center;
        gap: 15px;
    }

    .hero h2 {
        font-size: 28px;
    }

    .product {
        width: 100%;
        max-width: 320px;
    }
}

```

## OUTPUT

<img width="1731" height="2339" alt="Screenshot_3-11-2026_135437_127 0 0 1" src="https://github.com/user-attachments/assets/b74d86d7-a871-42df-b81c-99926f4878c3" />


## RESULT
The program for creating commercial website using CSS Flexbox is executed successfully.
