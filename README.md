## Ex.07 Restaurant Website
## Date:08.10.2025

## AIM:
To develop a static Restaurant website to display the food items and services provided by them.

## DESIGN STEPS:

### Step 1:
Requirement collection.

### Step 2:
Creating the layout using HTML and CSS.

### Step 3:
Updating the sample content.

### Step 4:
Choose the appropriate style and color scheme.

### Step 5:
Validate the layout in various browsers.

### Step 6:
Validate the HTML code.

### Step 7:
Publish the website in the given URL.

## PROGRAM:
```
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Harini Restaurant</title>
  <style>
    body {
      font-family: Arial, sans-serif;
      margin: 0;
      padding: 0;
      background-color: #f8f8f8;
    }

    /* Header */
    header {
      background: url('https://images.unsplash.com/photo-1600891964599-f61ba0e24092') no-repeat center/cover;
      color: white;
      text-align: center;
      padding: 80px 20px;
    }

    header h1 {
      font-size: 42px;
      margin: 0;
      text-shadow: 2px 2px 6px rgba(0,0,0,0.5);
    }

    nav {
      display: flex;
      justify-content: center;
      background-color: #333;
    }

    nav a {
      color: white;
      padding: 14px 20px;
      text-decoration: none;
      text-transform: uppercase;
    }

    nav a:hover {
      background-color: #575757;
    }

    section {
      padding: 50px 20px;
      max-width: 1000px;
      margin: auto;
    }

    h2 {
      color: #ff6f61;
      text-align: center;
      margin-bottom: 30px;
    }

    /* Menu */
    .menu-grid {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(220px, 1fr));
      gap: 20px;
    }

    .menu-item {
      background: white;
      border-radius: 10px;
      overflow: hidden;
      box-shadow: 0 4px 8px rgba(0,0,0,0.1);
      text-align: center;
    }

    .menu-item img {
      width: 100%;
      height: 150px;
      object-fit: cover;
    }

    .menu-item h3 {
      margin: 10px 0;
    }

    .menu-item span {
      display: block;
      margin-bottom: 10px;
      font-weight: bold;
      color: #ff6f61;
    }

    /* Forms */
    form {
      display: flex;
      flex-direction: column;
      max-width: 400px;
      margin: auto;
    }

    form input, form textarea {
      padding: 10px;
      margin: 5px 0 15px 0;
      border: 1px solid #ccc;
      border-radius: 5px;
    }

    form button {
      padding: 12px;
      background-color: #ff6f61;
      color: white;
      border: none;
      border-radius: 5px;
      cursor: pointer;
    }

    form button:hover {
      background-color: #e65c50;
    }

    /* Footer */
    footer {
      text-align: center;
      padding: 20px;
      background-color: #333;
      color: white;
      margin-top: 50px;
    }
  </style>
</head>
<body>

  <!-- Header -->
  <header>
    <h1>Welcome to Harini Restaurant</h1>
    <p>Delicious food, fresh ingredients!</p>
  </header>

  <!-- Navigation -->
  <nav>
    <a href="#menu">Menu</a>
    <a href="#contact">Contact</a>
    <a href="#admin">Administration</a>
  </nav>

  <!-- Menu Section -->
  <section id="menu">
    <h2>Our Menu</h2>
    <div class="menu-grid">
      <div class="menu-item">
        <img src="Screenshot 2025-09-30 160811.png" alt="Pizza">
        <h3>Margherita Pizza</h3>
        <span>$10</span>
      </div>
      <div class="menu-item">
        <img src="Screenshot 2025-09-30 160420.png" alt="Pasta">
        <h3>Spaghetti Bolognese</h3>
        <span>$12</span>
      </div>
      <div class="menu-item">
        <img src="Screenshot 2025-10-01 150035.png" alt="Salad">
        <h3>Caesar Salad</h3>
        <span>$8</span>
      </div>
      <div class="menu-item">
        <img src="Screenshot 2025-09-30 161022.png" alt="Cake">
        <h3>Chocolate Cake</h3>
        <span>$6</span>
      </div>
    </div>
  </section>

  <!-- Contact Section -->
  <section id="contact">
    <h2>Contact Us</h2>
    <form>
      <input type="text" placeholder="Your name" required>
      <input type="email" placeholder="Your Email" required>
      <textarea rows="4" placeholder="Your Message" required></textarea>
      <button type="submit">Send Message</button>
    </form>
  </section>

  <!-- Admin Section -->
  <section id="admin">
    <h2>Administration</h2>
    <form>
      <input type="text" placeholder="Admin Username" required>
      <input type="password" placeholder="Password" required>
      <button type="submit">Login</button>
    </form>
  </section>

  <!-- Footer -->
  <footer>
    &copy; 2025 Harini Restaurant. All rights reserved.
  </footer>

</body>
</html>

```

## OUTPUT:
![alt text](<Screenshot 2025-09-30 161850.png>)
![alt text](<Screenshot 2025-09-30 161702.png>)

## RESULT:
The program for designing software company website using HTML and CSS is completed successfully.
