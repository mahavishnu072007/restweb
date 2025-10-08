# Ex.07 Restaurant Website
## Date:09.10.2025

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
    <title>Vijay's Restaurant</title>
    <style>
        body {
            background-color: #FFF8F0;
            margin: 0;
            font-family: 'Segoe UI', Arial, sans-serif;
            color: #4B1D0F;
        }
        header {
            background-color: #B23A48;
            color: #FFF8F0;
            text-align: center;
            padding: 30px 10px 20px 10px;
        }
        nav {
            background-color: #F39237;
            overflow: hidden;
        }
        nav a {
            float: left;
            display: block;
            color: #4B1D0F;
            text-align: center;
            padding: 16px 36px;
            text-decoration: none;
            font-weight: bold;
        }
        nav a:hover {
            background-color: #FFD166;
            color: #B23A48;
        }
        .banner {
            width: 100%;
            height: 280px;
            background-image: url('https://images.unsplash.com/photo-1504674900247-0877df9cc836?auto=format&fit=crop&w=1100&q=80');
            background-size: cover;
            background-position: center;
        }
        .container {
            max-width: 1000px;
            margin: 40px auto;
            padding: 24px;
            background-color: #fff;
            border-radius: 12px;
            box-shadow: 0 4px 24px rgba(180,58,72,0.07);
        }
        .menu-grid {
            display: grid;
            grid-template-columns: repeat(4, 1fr);
            gap: 22px;
        }
        .menu-item {
            background: #FFF8F0;
            border: 1px solid #FFD166;
            border-radius: 8px;
            padding: 20px 12px;
            text-align: center;
        }
        .menu-item img {
            width: 90px;
            height: 70px;
            object-fit: cover;
            border-radius: 8px;
        }
        .admin-grid {
            display: grid;
            grid-template-columns: repeat(3, 1fr);
            gap: 28px;
            margin-top: 18px;
        }
        .admin-card {
            background: #FFF8F0;
            border: 1px solid #FFD166;
            border-radius: 8px;
            text-align: center;
            padding: 24px 12px;
        }
        .admin-card img {
            width: 78px;
            height: 78px;
            border-radius: 50%;
            object-fit: cover;
        }
        footer {
            background: #B23A48;
            color: #FFF8F0;
            text-align: center;
            padding: 18px 0 8px 0;
            position: relative;
        }
        .active {
            background-color: #FFD166;
            color: #B23A48 !important;
        }
        @media (max-width: 800px) {
            .menu-grid {
                grid-template-columns: repeat(2, 1fr);
            }
            .admin-grid {
                grid-template-columns: repeat(2, 1fr);
            }
        }
        @media (max-width: 500px) {
            .menu-grid, .admin-grid {
                grid-template-columns: 1fr;
            }
            nav a {
                float: none;
                display: block;
            }
        }
    </style>
    <script>
        function showPage(pageId) {
            document.querySelectorAll('.container').forEach(c=>c.style.display='none');
            document.getElementById(pageId).style.display = 'block';
            document.querySelectorAll('nav a').forEach(a=>a.classList.remove('active'));
            document.getElementById('nav-' + pageId).classList.add('active');
        }
        window.onload = function() {
            showPage('home');
        }
    </script>
</head>
<body>
    <header>
        <div class="banner"></div>
        <h1>Vijay's Restaurant</h1>
        <p>The Crunchiest Fries and Chicken in Town!</p>
    </header>
    <nav>
        <a id="nav-home" href="#" onclick="showPage('home');return false;">Home</a>
        <a id="nav-menu" href="#" onclick="showPage('menu');return false;">Menu</a>
        <a id="nav-admin" href="#" onclick="showPage('admin');return false;">Administration</a>
        <a id="nav-contact" href="#" onclick="showPage('contact');return false;">Contact Us</a>
    </nav>
    <div id="home" class="container">
        <h2>Welcome to Vijay'sRestaurant!</h2>
        <p>Enjoy delicious, golden-brown chicken fries and a variety of tastebud-tantalizing treats. Savor our special selection made with the freshest ingredients and cooked to perfection. Whether you dine in or take away, we promise every bite will leave you craving for more!</p>
        <img src="https://images.unsplash.com/photo-1519864600265-abb23847ef2c?auto=format&fit=crop&w=500&q=80" style="width:100%;max-width:600px;margin-top:20px;border-radius:10px;">
    </div>
    <div id="menu" class="container" style="display:none;">
        <h2>Our Menu</h2>
        <div class="menu-grid">

            <div class="menu-item"><img src="https://images.unsplash.com/photo-1502741338009-cac2772e18bc?auto=format&fit=crop&w=200&q=80"><br>Cheesy Chicken Fries<br>₹140</div>
            <div class="menu-item"><img src="https://images.unsplash.com/photo-1504674900247-0877df9cc836?auto=format&fit=crop&w=200&q=80"><br>Spicy Chicken Fries<br>₹130</div>
            <div class="menu-item"><img src="https://images.unsplash.com/photo-1452195100486-9cc805987862?auto=format&fit=crop&w=200&q=80"><br>BBQ Chicken Fries<br>₹150</div>
            <div class="menu-item"><img src="https://images.unsplash.com/photo-1467003909585-2f8a72700288?auto=format&fit=crop&w=200&q=80"><br>Peri Peri Chicken Fries<br>₹145</div>
            <div class="menu-item"><img src="https://images.unsplash.com/photo-1504674900247-0877df9cc836?auto=format&fit=crop&w=200&q=80"><br>Curly Fries<br>₹90</div>
            <div class="menu-item"><img src="https://images.unsplash.com/photo-1502741338009-cac2772e18bc?auto=format&fit=crop&w=200&q=80"><br>Loaded Fries<br>₹150</div>
            <div class="menu-item"><img src="https://images.unsplash.com/photo-1504674900247-0877df9cc836?auto=format&fit=crop&w=200&q=80"><br>Chicken Burger<br>₹170</div>
            <div class="menu-item"><img src="https://images.unsplash.com/photo-1467003909585-2f8a72700288?auto=format&fit=crop&w=200&q=80"><br>Veggie Fries<br>₹110</div>
            <div class="menu-item"><img src="https://images.unsplash.com/photo-1452195100486-9cc805987862?auto=format&fit=crop&w=200&q=80"><br>Paneer Fries<br>₹120</div>
            <div class="menu-item"><img src="https://images.unsplash.com/photo-1502741338009-cac2772e18bc?auto=format&fit=crop&w=200&q=80"><br>Crispy Chicken Wrap<br>₹160</div>
        </div>
    </div>
    <div id="admin" class="container" style="display:none;">
        <h2>Administration</h2>
        <div class="admin-grid">
            <div class="admin-card">

                <b>Rahul</b><br>
                Manager
            </div>
            <div class="admin-card">

                <b>Priya</b><br>
                Head Chef
            </div>
            <div class="admin-card">

                <b>Arjun</b><br>
                Operations Lead
            </div>
            <div class="admin-card">

                <b>Anjali</b><br>
                Marketing Head
            </div>
            <div class="admin-card">

                <b>Sanjay</b><br>
                Finance Manager
            </div>
            <div class="admin-card">
                <b>Meera</b><br>
                Customer Relations
            </div>
        </div>
    </div>
    <div id="contact" class="container" style="display:none;">
        <h2>Contact Us</h2>
        <p><b>Address:</b> 53 BANGALA STREET, PANRUTI, CUDDALORE, 607 205</p>
        <p><b>Phone:</b> +91-9876543210</p>
        <p><b>Email:</b> vijay12@gmail.com</p>
        <p>We welcome all your feedback and enquiries!</p>
    </div>
    <footer>
        &copy; DESIGNED BY MAHA VISHNU(25018250)
    </footer>
</body>
</html>

```



## OUTPUT:

![alt text](<Restaurent/restapp/static/Screenshot (52).png>)
![alt text](<Restaurent/restapp/static/Screenshot (53).png>)
![alt text](<Restaurent/restapp/static/Screenshot (54).png>)
![alt text](<Restaurent/restapp/static/Screenshot (55).png>)

## RESULT:
The program for designing software company website using HTML and CSS is completed successfully.

