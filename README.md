# Ex.06 Restaurant Website
# Date:
# AIM:
To develop a static Restaurant website to display the food items and services provided by them.

# DESIGN STEPS:
## Step 1:
Requirement collection.

## Step 2:
Creating the layout using HTML and CSS.

## Step 3:
Updating the sample content.

## Step 4:
Choose the appropriate style and color scheme.

## Step 5:
Validate the layout in various browsers.

## Step 6:
Validate the HTML code.

## Step 7:
Publish the website in the given URL.

# PROGRAM:
```
HOME PAGE.html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>The Baratie</title>
    <style>
      
        body {
            margin: 0;
            font-family: 'Arial', sans-serif;
            line-height: 1.6;
            color: #333;
            box-sizing: border-box;
        }

        *, *::before, *::after {
            box-sizing: inherit;
        }

        header {
            background: white;
            color: #000000;
            padding: 5px 10px;
            display: flex;
            align-items: center;
            justify-content: space-between;
            position: relative;
            height: 80px;
            overflow: hidden;
            
        }

        header nav a {
            padding-right: 10px;
            text-decoration: none;
            color: #000000;
            font-weight: bold;
            margin: 0 10px;
            transition: color 0.3s ease;
        }

        header nav a:hover {
            color: #ff5722;
        }

        .tblogo{
            display: flex;
            height: 120px;

        }

        .ltext{
            height: 95px;
            margin-top: 5%;
            font-family: Georgia, 'Times New Roman', Times, serif;
        }

        .banner {
            background-size: cover;
            margin-right: 2%;
            margin-left: 2%;
            margin-top: 1%;
            border-radius: 37px;
            display: flex;
            align-items: center;
            justify-content: center;
            padding: 30px 20px;
            background: url('banner.jpg') no-repeat center center/cover;
            color: white;
            height: 300px;
            text-align: center;
        }

        .banner-content {
            max-width: 50%;
        }

        .banner-content h1 {
            font-family: Georgia, 'Times New Roman', Times, serif;
            font-size: 2.5rem;
            margin-bottom: 10px;
            color: rgb(0, 0, 0);
        }

        .banner-content p {
            font-size: 1rem;
            margin-bottom: 15px;
            color: black;
        }

        .banner-content a {
            background: transparent;
            color: rgb(0, 0, 0);
            padding: 8px 15px;
            text-decoration: none;
            font-weight: bold;
            border-radius: 5px;
            border: solid;
            border-color: #000000;
            transition: background 0.3s ease;
        }

        .banner-content a:hover {
            background: #ffffff;
        }

        .features {
            display: flex  ;
            justify-content: space-between;
            align-items: flex-start;
            padding: 20px;
            gap: 15px;
            background: #f9f9f9;
        }

        .feature {
            background: white;
            border-radius: 10px;
            padding: 15px;
            box-shadow: 0 4px 6px rgba(0, 0, 0, 0.1);
            flex: 1;
            text-align: center;
        }

        .feature img {
            width: 100%;
            border-radius: 10px;
            margin-bottom: 10px;
        }

        .feature h3 {
            font-size: 1.2rem;
            margin-bottom: 10px;
            color: #1f1714;
        }

        .feature p {
            font-size: 0.9rem;
            color: #555;
        }

       
            margin-top: 180px;
        }


        @media (max-width: 768px) {
            .banner {
                flex-direction: column;
                height: auto;
                text-align: center;
            }

            .banner-content {
                max-width: 100%;
            }

            .features {
                flex-direction: column;
                gap: 20px;
            }

            .feature {
                flex: none;
            }

            header nav a {
                margin: 0 5px;
            }
        }
    </style>
</head>
<body>

    <header>
        <div class="tblogo">
            <img src="Logo.png" href="home.html" alt="The Baratie Logo">
            <div class="ltext"><h1 >The Baratie</h1></div>
        </div>
        
            <nav>
                <a href="home.html">Home</a>
                <a href="menu.html">Menu</a>
                <a href="contact.html">Contact</a>
                <a href="admin.html">Administration</a>
           </nav>
        
    </header>
    <hr width="95%"> 
    <div class="banner">
        <div class="banner-content">
            <h1>Welcome to THE BARATIE</h1>
            <p>Where the Ocean Meets Your Plate, and Every Meal is an Adventure.</p>
            <a href="#features">Explore Now</a>
        </div>
    </div>

    <section id="features" class="features">
        <div class="feature">
            <img src="ocean.jpeg" alt="Stunning Ocean Views">
            <h3>Stunning Ocean Views</h3>
            <p>Dine with breathtaking panoramic views of the ocean, where every meal is paired with stunning sunsets and serene seascapes.</p>
        </div>
        <div class="feature">
            <img src="ambience.jpeg" alt="Unique Nautical Ambiance">
            <h3>Unique Nautical Ambiance</h3>
            <p>Immerse yourself in a cozy maritime ambiance, complete with elegant nautical decor and the charm of the sea.</p>
        </div>
        <div class="feature">
            <img src="seafood.jpg" alt="Signature Seafood">
            <h3>Signature Seafood</h3>
            <p>Savor the freshest catch, beautifully displayed and expertly prepared to celebrate the flavors of the ocean.</p>
        </div>
    </section>

   

</body>
</html>
```
```
Menu.html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>The Baratie - Menu</title>
    <style>
        body {
            margin: 0;
            font-family: 'Arial', sans-serif;
            line-height: 1.6;
            color: #333;
            box-sizing: border-box;
        }

        *, *::before, *::after {
            box-sizing: inherit;
        }

        header {
            background: white;
            color: #000000;
            padding: 5px 10px;
            display: flex;
            align-items: center;
            justify-content: space-between;
            position: relative;
            height: 80px;
            overflow: hidden;
            
        }

        header nav a {
            padding-right: 10px;
            text-decoration: none;
            color: #000000;
            font-weight: bold;
            margin: 0 10px;
            transition: color 0.3s ease;
        }

        header nav a:hover {
            color: #ff5722;
        }

        .tblogo{
            display: flex;
            height: 120px;

        }

        .ltext{
            height: 95px;
            margin-top: 5%;
            font-family: Georgia, 'Times New Roman', Times, serif;
        }

        .menu-container {
            padding: 20px;
            background: #f9f9f9;
            text-align: center;
        }

        .menu-container h1 {
            font-size: 2rem;
            color: #000000;
            margin-bottom: 15px;
        }

        .menu-items {
            display: flex;
            flex-wrap: wrap;
            gap: 15px;
            justify-content: center;
        }

        .menu-item {
            background: white;
            border-radius: 10px;
            box-shadow: 0 4px 6px rgba(0, 0, 0, 0.1);
            width: 280px;
            overflow: hidden;
            transition: transform 0.3s ease;
        }

        .menu-item img {
            width: 100%;
            height: 180px;
            object-fit: cover;
        }

        .menu-item:hover {
            transform: scale(1.05);
        }

        .menu-details {
            padding: 10px;
        }

        .menu-details h3 {
            font-size: 1.2rem;
            color: #000000;
            margin-bottom: 8px;
        }

        .menu-details p {
            font-size: 0.9rem;
            color: #555;
            margin-bottom: 10px;
        }

        .menu-details .price {
            font-weight: bold;
            font-size: 1rem;
            color: #ff5722;
        }

        

        @media (max-width: 768px) {
            header h1 {
                font-size: 1.2rem;
            }

            .menu-items {
                flex-direction: column;
                gap: 20px;
            }

            .menu-item {
                width: 100%;
            }

            header nav a {
                margin: 0 5px;
            }
        }
    </style>
</head>
<body>

    <header>
        <div class="tblogo">
            <img src="Logo.png" href="home.html" alt="The Baratie Logo">
            <div class="ltext"><h1 >The Baratie</h1></div>
        </div>
        
            <nav>
                <a href="home.html">Home</a>
                <a href="menu.html">Menu</a>
                <a href="contact.html">Contact</a>
                <a href="admin.html">Administration</a>
           </nav>
        
    </header>

    <div class="menu-container">
        <h1>Our Menu</h1>
        <div class="menu-items">
            <div class="menu-item">
                <img src="Lobster_Bisque.jpg" alt="Lobster Bisque">
                <div class="menu-details">
                    <h3>Lobster Bisque</h3>
                    <p class="price">₹1800/-</p>
                </div>
            </div>

            <div class="menu-item">
                <img src="Grilled_Octopus.jpg" alt="Grilled Octopus">
                <div class="menu-details">
                    <h3>Grilled Octopus</h3>
                    <p class="price">₹4600/-</p>
                </div>
            </div>

            <div class="menu-item">
                <img src="Shrimp_Scampi.jpg" alt="Shrimp Scampi">
                <div class="menu-details">
                    <h3>Shrimp Scampi</h3>
                    <p class="price">₹1750/-</p>
                </div>
            </div>

            <div class="menu-item">
                <img src="Bouillabaisse.jpg" alt="Bouillabaisse">
                <div class="menu-details">
                    <h3>Bouillabaisse</h3>
                    <p class="price">₹1200/-</p>
                </div>
            </div>

            <div class="menu-item">
                <img src="Sushi_Sashimi.jpg" alt=" Sushi & Sashimi">
                <div class="menu-details">
                    <h3> Sushi & Sashimi</h3>
                    <p class="price">₹1000/-</p>
                </div>
            </div>

            <div class="menu-item">
                <img src="Ceviche.jpg" alt="Ceviche">
                <div class="menu-details">
                    <h3>Ceviche</h3>
                    <p class="price">₹1700/-</p>
                </div>
            </div>
            <div class="menu-item">
                <img src="Paella_de_Mariscos.jpg" alt=" Paella de Mariscos">
                <div class="menu-details">
                    <h3> Paella de Mariscos</h3>
                    <p class="price">₹2200/-</p>
                </div>
            </div>
            <div class="menu-item">
                <img src="Crab_Cakes.jpg" alt="Crab Cakes">
                <div class="menu-details">
                    <h3>Crab Cakes</h3>
                    <p class="price">₹3500/-</p>
                </div>
            </div>
            <div class="menu-item">
                <img src="Fish_Tacos.jpg" alt="Fish Tacos">
                <div class="menu-details">
                    <h3>Fish Tacos</h3>
                    <p class="price">₹1450/-</p>
                </div>
            </div>
            <div class="menu-item">
                <img src="Salmon_Teriyaki.jpg" alt="Salmon Teriyaki">
                <div class="menu-details">
                    <h3>Salmon Teriyaki</h3>
                    <p class="price">₹2200/-</p>
                </div>
            </div>
            <div class="menu-item">
                <img src="Jambalaya.jpg" alt="Jambalaya">
                <div class="menu-details">
                    <h3>Jambalaya</h3>
                    <p class="price">₹2500/-</p>
                </div>
            </div>
            <div class="menu-item">
                <img src="Chilli_Crab.jpg" alt="Chilli Crab">
                <div class="menu-details">
                    <h3>Chilli Crab</h3>
                    <p class="price">₹2600/-</p>
                </div>
            </div>
        </div>
    </div>

  

</body>
</html>
```
```
Contact.html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>The Baratie - Contact Us</title>
    <style>
        body {
            margin: 0;
            font-family: 'Arial', sans-serif;
            line-height: 1.6;
            color: #333;
            box-sizing: border-box;
        }

        *, *::before, *::after {
            box-sizing: inherit;
        }

        header {
            background: white;
            color: #000000;
            padding: 5px 10px;
            display: flex;
            align-items: center;
            justify-content: space-between;
            position: relative;
            height: 80px;
            overflow: hidden;
            
        }

        header nav a {
            padding-right: 10px;
            text-decoration: none;
            color: #000000;
            font-weight: bold;
            margin: 0 10px;
            transition: color 0.3s ease;
        }

        header nav a:hover {
            color: #ff5722;
        }

        .tblogo{
            display: flex;
            height: 120px;

        }

        .ltext{
            height: 95px;
            margin-top: 5%;
            font-family: Georgia, 'Times New Roman', Times, serif;
        }


        .contact-banner h1 {
            font-family: Georgia, 'Times New Roman', Times, serif;
            font-size: 2.5rem;
            color:white;
        }

        .contact-section {
            display: flex;
            flex-wrap: wrap;
            justify-content: center;
            padding: 30px 15px;
            background: white;
            gap: 20px;
        }

        .contact-details, .contact-form {
            flex: 1;
            max-width: 500px;
            margin: 10px;
            background: white;
            padding: 20px;
            border-radius: 10px;
            box-shadow: 4px 4px 4px 6px rgba(0, 0, 0, 0.1);
        }

        .contact-details h2, .contact-form h2 {
            font-size: 1.8rem;
            margin-bottom: 15px;
            color: #1f1714;
            text-align: center;
        }

        .contact-details p {
            margin: 10px 0;
            font-size: 1rem;
            color: #555;
        }

        .contact-details img {
            max-width: 100%;
            border-radius: 10px;
            margin-bottom: 20px;
        }

        .contact-form input, .contact-form textarea {
            width: 100%;
            padding: 10px;
            margin: 10px 0;
            border: 1px solid #ccc;
            border-radius: 5px;
            font-size: 1rem;
        }

        .contact-form textarea {
            height: 100px;
        }

        .contact-form button {
            width: 100%;
            padding: 10px;
            background: #ff5722;
            color: white;
            font-size: 1.1rem;
            border: none;
            border-radius: 5px;
            cursor: pointer;
            transition: background 0.3s ease;
        }

        .contact-form button:hover {
            background: #e64a19;
        }


        @media (max-width: 768px) {
            .contact-details, .contact-form {
                max-width: 100%;
            }

            .contact-banner h1 {
                font-size: 2rem;
            }
        }
    </style>
</head>
<body>

    <header>
        <div class="tblogo">
            <img src="Logo.png" href="home.html" alt="The Baratie Logo">
            <div class="ltext"><h1 >The Baratie</h1></div>
        </div>
        
            <nav>
                <a href="home.html">Home</a>
                <a href="menu.html">Menu</a>
                <a href="contact.html">Contact</a>
                <a href="admin.html">Administration</a>
           </nav>
        
    </header>

    <div class="contact-banner">
     
    </div>

    <section class="contact-section">
        <div class="contact-details">
            <h2>Get in Touch</h2>
            <img src="contact.png" alt="Contact Us">
            <p><strong>Phone:</strong> +91 8015553500</p>
            <p><strong>Email:</strong> contactus@baratie.com</p>
            <p><strong>Hours:</strong> Mon-Sun(10 AM - 10 PM)</p>
        </div>

        <div class="contact-form">
            <h2>Send Us a Message</h2>
            <form action="/submit-contact" method="POST">
                <label for="name">Full Name</label>
                <input type="text" id="name" name="name" placeholder="Enter your full name" required>

                <label for="email">Email Address</label>
                <input type="email" id="email" name="email" placeholder="Enter your email address" required>

                <label for="message">Message</label>
                <textarea id="message" name="message" placeholder="Your message" required></textarea>

                <button type="submit">Send Message</button>
            </form>
        </div>
    </section>

    
</body>
</html>
```
```
administration.html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>The Baratie - Administration</title>
    <style>
        body {
            margin: 0;
            font-family: 'Arial', sans-serif;
            line-height: 1.6;
            color: #333;
            box-sizing: border-box;
        }

        *, *::before, *::after {
            box-sizing: inherit;
        }

        header {
            background: white;
            color: #000000;
            padding: 5px 10px;
            display: flex;
            align-items: center;
            justify-content: space-between;
            position: relative;
            height: 80px;
            overflow: hidden;
            
        }

        header nav a {
            padding-right: 10px;
            text-decoration: none;
            color: #000000;
            font-weight: bold;
            margin: 0 10px;
            transition: color 0.3s ease;
        }

        header nav a:hover {
            color: #ff5722;
        }

        .tblogo{
            display: flex;
            height: 120px;

        }

        .ltext{
            height: 95px;
            margin-top: 5%;
            font-family: Georgia, 'Times New Roman', Times, serif;
        }


        .admin-container {
            padding: 20px;
            background: #f9f9f9;
            text-align: center;
        }

        .admin-container h1 {
            font-size: 2rem;
            color: #000000;
            margin-bottom: 20px;
        }

        .admin-items {
            display: flex;
            flex-wrap: wrap;
            gap: 20px;
            justify-content: center;
        }

        .admin-item {
            background: white;
            border-radius: 10px;
            box-shadow: 0 4px 6px rgba(0, 0, 0, 0.1);
            width: 300px;
            overflow: hidden;
            transition: transform 0.3s ease;
            text-align: left;
        }

        .admin-item img {
            width: 100%;
            height: 200px;
            object-fit: cover;
        }

        .admin-item:hover {
            transform: scale(1.05);
        }

        .admin-details {
            padding: 15px;
        }

        .admin-details h3 {
            text-align: center;
            font-size: 1.2rem;
            color: #000000;
            margin-bottom: 8px;
        }

        .admin-details p {
            font-size: 0.9rem;
            color: #555;
            margin-bottom: 10px;
        }

       

        @media (max-width: 768px) {
            header h1 {
                font-size: 1.2rem;
            }

            .admin-items {
                flex-direction: column;
                gap: 20px;
            }

            .admin-item {
                width: 100%;
            }

            header nav a {
                margin: 0 5px;
            }
        }
    </style>
</head>
<body>

    <header>
        <div class="tblogo">
            <img src="Logo.png" href="home.html" alt="The Baratie Logo">
            <div class="ltext"><h1 >The Baratie</h1></div>
        </div>
        
            <nav>
                <a href="home.html">Home</a>
                <a href="menu.html">Menu</a>
                <a href="contact.html">Contact</a>
                <a href="admin.html">Administration</a>
           </nav>
        
    </header>
    <div class="admin-container">
        <h1>Our Administration Team</h1>
        <div class="admin-items">
            <div class="admin-item">
                <img src="ceo.jpg" alt="CEO">
                <div class="admin-details">
                    <h3>Roronoa Zoro</h3>
                    <p>CEO - Leading The Baratie with a vision of excellence and innovation in hospitality.</p>
                </div>
            </div>

            <div class="admin-item">
                <img src="manager.jpg" alt="Manager">
                <div class="admin-details">
                    <h3>Monkey D Luffy</h3>
                    <p>Manager - Ensures smooth operations and a great dining experience for all guests.</p>
                </div>
            </div>

            <div class="admin-item">
                <img src="cook.jpg" alt="Master Chef">
                <div class="admin-details">
                    <h3>Vinsmoke Sanji</h3>
                    <p>Master Chef - Brings authentic Italian flavors to every dish served.</p>
                </div>
            </div>

            <div class="admin-item">
                <img src="am.jpg" alt="Assistant Managing Director">
                <div class="admin-details">
                    <h3>Nami</h3>
                    <p>Assistant Managing Director - Supporting the team with strategy and execution excellence.</p>
                </div>
            </div>
        </div>
    </div>

  

</body>
</html>
```
# OUTPUT:
<img width="1612" height="888" alt="image" src="https://github.com/user-attachments/assets/3cce6c8f-1ada-4617-9c85-838d4fcc4c9c" />
<img width="1615" height="796" alt="image" src="https://github.com/user-attachments/assets/44b7abe1-64ea-4c9a-8c6d-91467ef8ee83" />
<img width="1617" height="745" alt="image" src="https://github.com/user-attachments/assets/3a97c7b7-61a0-4f25-99b9-920cb1ee968d" />
<img width="1443" height="576" alt="image" src="https://github.com/user-attachments/assets/fcc68c45-05ad-462f-937c-03f3a4e6db73" />


# RESULT:
The program for designing software company website using HTML and CSS is completed successfully.
