# Ex02 Commercial Website

## Date: 07-08-2025

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

### index.html
```
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>GadgetHive</title>
  <link rel="stylesheet" href="style.css">
  <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0/css/all.min.css">
</head>
<body>
  <header>
    <nav class="navbar">
      <div class="container">
        <a href="#" class="logo">GadgetHive</a>
        <ul class="nav-links">
          <li><a href="#home">Home</a></li>
          <li><a href="#products">Products</a></li>
          <li><a href="#about">About</a></li>
          <li><a href="#contact">Contact</a></li>
        </ul>
      </div>
    </nav>
  </header>
  <main>
    <section id="home" class="hero">
      <div class="container">
        <h1>Discover the Latest Tech</h1>
        <p>Your one-stop shop for cutting-edge gadgets and electronics.</p>
        <a href="#products" class="btn">Explore Products</a>
      </div>
    </section>
    <section id="products" class="products">
      <div class="container">
        <h2>Featured Products</h2>
        <div class="product-grid">
          <div class="product">
            <img src="iphone.png" alt="Smartwatch">
            <h3>I phone</h3>
            <p>The iPhone is a line of smartphones developed and marketed by Apple Inc.</p>
            <p>₹98,000</p>
            <a href="#" class="btn">View Details</a>
          </div>
          <div class="product">
            <img src="gaming laptop.png" alt="Wireless Earbuds">
            <h3>Gaming laptop</h3>
            <p>Lenovo LOQ </p>
            <p>₹80,000</p>
            <a href="#" class="btn">View Details</a>
          </div>
          <div class="product">
            <img src="bluetooth speaker.png" alt="Portable Speaker">
            <h3> Boat stone Bluetooth Speaker </h3>
            <p>Powerful sound in a compact design.</p>
            <p>₹3500</p>
            <a href="#" class="btn">View Details</a>
          </div>
        </div>
      </div>
    </section>
    <section id="about" class="about">
      <div class="container">
        <h2>About GadgetHive</h2>
        <p>GadgetHive is your buzzing hub for the latest and greatest in technology. From cutting-edge smartphones and innovative wearables to must-have accessories and smart home devices, we bring together a curated collection of gadgets that make life smarter, faster, and more fun.</p>
      </div>
    </section>
    <section id="contact" class="contact">
      <div class="container">
        <h2>Contact Us</h2>
        <p>Email : GadgetHive@gmail.com</p>
        <p>Phone : +91 6369184404</p>
      </div>
    </section>
  </main>
  <footer>
    <div class="container">
      <center><p>&copy; 2024 GadgetHive All rights reserved.</p></center>
    </div>
  </footer>
 
</body>
</html>
```
## style.css
```
body {
    font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
    margin: 0;
    padding: 0;
    line-height: 1.6;
    background-color: #121212;
    color: #e0e0e0;
  }
  .container {
    max-width: 1200px;
    margin: 0 auto;
    padding: 0 20px;
  }
  .btn {
    display: inline-block;
    background-color: #ff930e;
    color: #121212;
    padding: 12px 25px;
    text-decoration: none;
    border-radius: 5px;
    transition: background-color 0.3s ease, box-shadow 0.3s ease;
    box-shadow: 0 2px 5px rgba(243, 146, 67, 0.5);
  }
  .btn:hover {
    background-color: #ff930e;
    background-color: #ff930e;
    box-shadow: 0 4px 10px ;
  }
  .navbar {
    background-color: #1e1e1e;
    padding: 15px 0;
    position: sticky;
    top: 0;
    z-index: 1000;
  }
  .navbar .container {
    display: flex;
    justify-content: space-between;
    align-items: center;
  }
  .navbar .logo {
    font-size: 1.8em;
    font-weight: bold;
    color: #ff930e;
    text-decoration: none;
  }
  .navbar .nav-links {
    list-style: none;
    display: flex;
  }
  .navbar .nav-links li {
    margin-left: 25px;
  }
  .navbar .nav-links li a {
    color: #e0e0e0;
    text-decoration: none;
    transition: color 0.3s ease;
  }
  .navbar .nav-links li a:hover {
    color: #ff930e;
  }
  .hero {
    background-image: linear-gradient(rgba(0, 0, 0, 0.6), rgba(0, 0, 0, 0.6)), url('hero-bg.jpg');
    background-size: cover;
    background-position: center;
    color: #e0e0e0;
    text-align: center;
    padding: 150px 0;
  }
  .hero h1 {
    font-size: 3em;
    margin-bottom: 20px;
    text-shadow: 2px 2px 5px rgba(0, 0, 0, 0.8);
  }
  .hero p {
    font-size: 1.2em;
    margin-bottom: 30px;
    text-shadow: 1px 1px 3px rgba(0, 0, 0, 0.6);
  }
  .products {
    padding: 80px 0;
  }
  .products h2 {
    text-align: center;
    margin-bottom: 50px;
    color: #ff930e;
    text-shadow: 1px 1px 3px rgba(0, 0, 0, 0.6);
  }
  .product-grid {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
    grid-gap: 30px;
  }
  .product {
    background-color: #1e1e1e;
    border-radius: 8px;
    box-shadow: 0 4px 10px rgba(0, 0, 0, 0.3);
    overflow: hidden;
    transition: transform 0.3s ease, box-shadow 0.3s ease;
  }
  .product:hover {
    transform: translateY(-5px);
    box-shadow: 0 6px 15px rgba(0, 0, 0, 0.4);
  }
  .product img {
    width: 100%;
    height: auto;
    display: block;
  }
  .product h3 {
    color: #ff930e;
    margin: 20px 0 10px;
    text-align: center;
  }
  .product p {
    text-align: center;
    padding: 0 20px;
    margin-bottom: 20px;
  }
  .about {
    padding: 80px 0;
    background-color: #1a1a1a;
    border-radius: 10px;
    box-shadow: 0 4px 10px rgba(0, 0, 0, 0.3);
    margin: 30px 20px;
  }
  .about .container {
    max-width: 800px;
    text-align: center;
  }
  .about h2 {
    color: #ff930e;
    margin-bottom: 30px;
    text-shadow: 1px 1px 3px rgba(0, 0, 0, 0.6);
  }
  .about p {
    font-size: 1.1em;
    line-height: 1.8;
    padding: 0 30px;
  }
  .contact {
    padding: 80px 0;
    background-color: #222222;
    border-radius: 10px;
    box-shadow: 0 4px 10px rgba(0, 0, 0, 0.3);
    margin: 30px 20px;
  }
  .contact .container {
    max-width: 600px;
    text-align: center;
  }
  .contact h2 {
    color: #ff930e;
    margin-bottom: 30px;
    text-shadow: 1px 1px 3px rgba(0, 0, 0, 0.6);
  }
  .contact p {
    font-size: 1.1em;
    margin-bottom: 20px;
    display: flex;
    justify-content: center;
    align-items: center;
  }
  .contact p::before {
    content: "";
    display: inline-block;
    width: 20px;
    height: 20px;
    background-size: contain;
    background-repeat: no-repeat;
    margin-right: 10px;
  }
  .contact p:nth-child(2)::before {
    background-image: url('email-icon.png');
  }
  .contact p:nth-child(3)::before {
    background-image: url('phone-icon.png');
```





## OUTPUT
<img width="1910" height="713" alt="Screenshot 2025-08-11 134448" src="https://github.com/user-attachments/assets/bfe7c411-ae3b-42c5-8ce6-778a6ab745a0" />
<img width="1918" height="973" alt="Screenshot 2025-08-11 134506" src="https://github.com/user-attachments/assets/f0324f85-44f1-47a2-94b4-b864f3acc190" />
<img width="1918" height="963" alt="Screenshot 2025-08-11 134528" src="https://github.com/user-attachments/assets/bdef459f-70cd-4c10-8a13-cd26fad3e91e" />



## RESULT

The program for creating commercial website using CSS Flexbox is executed successfully.
