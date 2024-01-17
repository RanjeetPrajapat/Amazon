<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Amazon Clone</title>
    <style>
        body {
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
            margin: 0;
            padding: 0;
        }

        #header {
            background-color: #232f3e;
            color: white;
            display: flex;
            justify-content: space-between;
            padding: 10px 20px;
            align-items: center;
        }

        #logo img {
            height: 40px;
            /* Adjust height as needed */
        }

        #account-info a {
            color: white;
            margin: 0 10px;
            text-decoration: none;
            transition: all ease 0.5sec;
        }

        .product-container {
            display: flex;
            justify-content: space-around;
            flex-wrap: wrap;
            padding: 20px;
        }

        .product {
            text-align: center;
            margin: 15px;
            padding: 15px;
            border: 1px solid #ddd;
            /* Add a border for separation */
            border-radius: 8px;
        }

        .product img {
            width: 100%;
            /* Make the image fill its container */
            border-radius: 8px;
            margin-bottom: 10px;
        }

        .price {
            color: #B12704;
            /* Amazon orange color */
            font-weight: bold;
        }

        .ratings {
            color: #FF9900;
            /* Amazon yellow color */
            margin-bottom: 10px;
        }

        .footer {
            background-color: #232f3e;
            color: white;
            padding: 20px;
            display: flex;
            justify-content: space-around;
            align-items: flex-start;
            flex-wrap: wrap;
        }

        .footer-section {
            margin-bottom: 20px;
        }

        .footer-section a {
            color: white;
            text-decoration: none;
            display: block;
            margin-bottom: 5px;
        }

        h1 {
            color: #f08804;
            /* Amazon yellow color */
            margin-bottom: 10px;
        }

        footer-section h4 a:hover {
            color: #FF9900;
        }

        .product img {
            width: 100%;
            border-radius: 8px;
            margin-bottom: 10px;
            transition: transform 0.3s ease-in-out;
        }

        .product img:hover {
            transform: scale(1.1);
        }

        .buy-now {
            background-color: #f08804;
            color: white;
            border: none;
            border-radius: 5px;
            padding: 8px 15px;
            font-size: 16px;
            cursor: pointer;
            transition: background-color 0.3s ease-in-out;
        }

        .buy-now:hover {
            background-color: #FF9900;
            /* Change the color on hover */
        }

        .contact {
            max-width: 500px;
            margin: auto;
            padding: 20px;
            background-color: #f8f8f8;
            border-radius: 8px;
            box-shadow: 0 0 10px rgba(0, 0, 0, 0.1);
        }

        h2 {
            color: #333;
            text-align: center;
        }

        input,
        textarea {
            width: 100%;
            padding: 10px;
            margin-bottom: 15px;
            border: 1px solid #ccc;
            border-radius: 4px;
            box-sizing: border-box;
        }

        button {
            background-color: #4caf50;
            color: white;
            padding: 10px 20px;
            border: none;
            border-radius: 4px;
            cursor: pointer;
        }

        button:hover {
            background-color: #45a049;
        }

        /* Optional: Style for responsiveness */
        @media (max-width: 600px) {

            input,
            textarea {
                width: calc(100% - 20px);
            }
        }

        #logo {
            text-align: center;
            margin: 20px;
            /* Adjust margin as needed */
        }

        #logo img {
            border-radius: 10px;
            /* Adds a slight border radius for a rounded corner effect */
            box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
            /* Adds a subtle box shadow */
            transition: transform 0.3s ease-in-out;
            /* Adds a smooth transition effect */
        }

        #logo img:hover {
            transform: scale(1.1);
            /* Enlarges the logo slightly on hover */
        }

        #search-bar {
            display: flex;
            align-items: center;
            justify-content: center;
            margin: 20px;
            margin-top: 2px 3px;
            float: right;
        }

        input[type="text"] {
            padding: 10px;
            font-size: 16px;
            border: 1px solid #ccc;
            border-radius: 4px;
            margin-right: 5px;
        }

        button {
            padding: 10px 20px;
            font-size: 16px;
            background-color: #ff9900;
            /* Change to your preferred color */
            color: #fff;
            border: none;
            border-radius: 4px;
            cursor: pointer;
        }

        button:hover {
            background-color: #e68a00;
            /* Change to your preferred color on hover */
        }

        #account-info a:hover {
            text-shadow: 0 0 5px #e68a00,0 0 15px #e68a00,0 0 25px #e68a00,0 0 100px #e68a00;
        }
    </style>
</head>

<body>

    <div id="header">
        <div id="logo">
            <img src="https://img2.cgtrader.com/items/4067074/227536c4aa/large/amazone-logo-3d-model-227536c4aa.jpg"
                alt="Amazon Logo" width="150px" height="100px">
        </div>
        <div id="search-bar">
            <input type="text" placeholder="Search Amazon.in" title="search">
            <button>Search</button>
        </div>
        <div id="account-info">
            <a href="login page.html">Hello, Login</a>
            <a href="#" onclick="showMessage('Returns & Orders')">Returns & Orders</a>
            <a href="#" onclick="showMessage('Try Prime')">Try Prime</a>
            <a href="#" onclick="showMessage('Cart')">Cart</a>
        </div>
    </div>

    <div class="product-container">

        <div class="product">
            <img src="https://i.ytimg.com/vi/spfwj6CsxoE/maxresdefault.jpg" alt="Product 1" width="200px"
                height="100px">
            <p>Study Pen</p>
            <p class="price">$19.99</p>
            <div class="ratings">★★★★☆</div>
            <button class="buy-now">Buy Now</button>
        </div>
        <!-- Add more products as needed -->

        <div class="product">
            <img src="https://i.pinimg.com/originals/ec/85/d1/ec85d1aa08a6194d31542066b2e270dc.jpg" alt="Product 1"
                width="200px" height="150px">
            <p>Pent</p>
            <p class="price">$999.9</p>
            <div class="ratings">★★★★☆</div>
            <button class="buy-now">Buy Now</button>
        </div>
        <!-- Add more products as needed -->

        <div class="product">
            <img src="https://i.ebayimg.com/images/g/KacAAOSw3FpaoKbM/s-l640.jpg" alt="Product 1" width="200px"
                height="100px">
            <p>Cloth Shirt</p>
            <p class="price">$299.9</p>
            <div class="ratings">★★★★☆</div>
            <button class="buy-now">Buy Now</button>
        </div>
        <!-- Add more products as needed -->

        <div class="product">
            <img src="https://th.bing.com/th/id/OIP.AiU8zlxVmm-wr0_2AC-BGgHaEK?pid=ImgDet&rs=1" alt="Product 1"
                width="200px" height="100px">
            <p>Reading Book</p>
            <p class="price">$379.99</p>
            <div class="ratings">★★★★☆</div>
            <button class="buy-now">Buy Now</button>
        </div>
        <!-- Add more products as needed -->

        <div class="product">
            <img src="https://th.bing.com/th/id/OIP.nAypaOPCOdJLCn7OUriIdAHaEK?pid=ImgDet&rs=1" alt="Product 1"
                width="200px" height="100px">
            <p> Stationary Book</p>
            <p class="price">$899.99</p>
            <div class="ratings">★★★★☆</div>
            <button class="buy-now">Buy Now</button>
        </div>

        <div class="product">
            <img src="https://img2.exportersindia.com/product_images/bc-full/2019/7/6451346/mens-formal-shirts-1561984677-4979568.jpeg"
                alt="Product 1" width="200px" height="100px">
            <p>Shirt Combo</p>
            <p class="price">$1299.99</p>
            <div class="ratings">★★★★☆</div>
            <button class="buy-now">Buy Now</button>
        </div>

        <div class="product">
            <img src="https://4.imimg.com/data4/YA/YE/MY-26866359/mens-combo-formal-shirts-500x500.jpg" alt="Product 1"
                width="200px" height="100px">
            <p>Cloth Combo</p>
            <p class="price">$1299.99</p>
            <div class="ratings">★★★★☆</div>
            <button class="buy-now">Buy Now</button>
        </div>
        <div class="product">
            <img src="https://thumbs.dreamstime.com/z/diamond-shape-sweets-lots-45915986.jpg" alt="Product 1"
                width="200px" height="100px">
            <p>Sweet</p>
            <p class="price">$999.99</p>
            <div class="ratings">★★★★☆</div>
            <button class="buy-now">Buy Now</button>

        </div>
        <div class="product">
            <img src="https://th.bing.com/th/id/OIP.1YKUbJJyFSywLSQPvnGL3gHaHc?pid=ImgDet&rs=1" alt="Product 1"
                width="200px" height="100px">
            <p>Tishirt </p>
            <p class="price">$299.99</p>
            <div class="ratings">★★★★☆</div>
            <button class="buy-now">Buy Now</button>
        </div>
        <div class="product">
            <img src="https://m.media-amazon.com/images/I/51+iKE4jmRL._AC_UL960_QL65_.jpg" alt="Product 1" width="200px"
                height="100px">
            <p>chashma</p>
            <p class="price">$399.99</p>
            <div class="ratings">★★★★☆</div>
            <button class="buy-now">Buy Now</button>
        </div>
        <div class="product">
            <img src="https://th.bing.com/th/id/OIP.WWShbiNKs3S4uno0qvLR-AHaFj?pid=ImgDet&rs=1" alt="Product 1"
                width="200px" height="100px">
            <p>Watch</p>
            <p class="price">$5099.99</p>
            <div class="ratings">★★★★☆</div>
            <button class="buy-now">Buy Now</button>
        </div>

        <div class="product">
            <img src="https://i.pinimg.com/originals/f6/d7/cf/f6d7cfce312c70d0884cfbc1713b1330.jpg" alt="Product 1"
                width="200px" height="100px">
            <p>Shadi</p>
            <p class="price">$1199.99</p>
            <div class="ratings">★★★★☆</div>
            <button class="buy-now">Buy Now</button>
        </div>
        <div class="product">
            <img src="https://images.meesho.com/images/products/143119650/rdrri_512.jpg" alt="Product 1" width="200px"
                height="100px">
            <p>Track pent</p>
            <p class="price">$999.99</p>
            <div class="ratings">★★★★☆</div>
            <button class="buy-now">Buy Now</button>
        </div>
        <div class="product">
            <img src="https://n4.sdlcdn.com/imgs/g/1/8/HP-Black-Laptop-Bags-SDL547155957-1-78dac.jpeg" alt="Product 1"
                width="200px" height="100px">
            <p>Laptop bag</p>
            <p class="price">$699.99</p>
            <div class="ratings">★★★★☆</div>
            <button class="buy-now">Buy Now</button>
        </div>
        <div class="product">
            <img src="https://evilato.com/wp-content/uploads/2023/02/IMG-20230212-WA0043.jpg" alt="Product 1"
                width="200px" height="150px">
            <p>Formal pent shirt</p>
            <p class="price">$1200.99</p>
            <div class="ratings">★★★★☆</div>
            <button class="buy-now">Buy Now</button>
        </div>
        <div class="product">
            <img src="https://i.pinimg.com/736x/d9/8a/4a/d98a4ad57e20ec243d97b7fe4654d224--photoshop.jpg"
                alt="Product 1" width="200px" height="100px">
            <p>Bleger</p>
            <p class="price">$1999.99</p>
            <div class="ratings">★★★★☆</div>
            <button class="buy-now">Buy Now</button>
        </div>
        <div class="product">
            <img src="https://th.bing.com/th/id/OIP.yEIkFs96YbiXpFcvy3CjLAHaJ4?rs=1&pid=ImgDetMain" alt="Product 1"
                width="200px" height="100px">
            <p>Hoodie</p>
            <p class="price">$599.99</p>
            <div class="ratings">★★★★☆</div>
            <button class="buy-now">Buy Now</button>
        </div>
        <div class="product">
            <img src="https://th.bing.com/th/id/OIP.HdvM7UXNkr0tXkI6ci9INwHaHa?pid=ImgDet&rs=1" alt="Product 1"
                width="200px" height="100px">
            <p>Sleeper</p>
            <p class="price">$199.99</p>
            <div class="ratings">★★★★☆</div>
            <button class="buy-now">Buy Now</button>
        </div>
        <div class="product">
            <img src="https://th.bing.com/th/id/OIP.n8nBuO0QYOLu25iRABph0QHaHa?pid=ImgDet&rs=1" alt="Product 1"
                width="200px" height="100px">
            <p>Tenish Bol</p>
            <p class="price">$120.99</p>
            <div class="ratings">★★★★☆</div>
            <button class="buy-now">Buy Now</button>
        </div>

        <div class="product">
            <img src="https://i.pinimg.com/originals/9d/64/cb/9d64cb758b016188eaa44b01549d2a13.jpg" alt="Product 1"
                width="200px" height="100px">
            <p>Dixnery book</p>
            <p class="price">$299.99</p>
            <div class="ratings">★★★★☆</div>
            <button class="buy-now">Buy Now</button>
        </div>

        <div class="product">
            <img src="https://5.imimg.com/data5/SELLER/Default/2021/10/DO/WA/CE/138764598/apsara-absolute-premium-pencils-box-500x500.png"
                alt="Product 1" width="200px" height="100px">
            <p>Pencil Box</p>
            <p class="price">$99.99</p>
            <div class="ratings">★★★★☆</div>
            <button class="buy-now">Buy Now</button>
        </div>

    </div>

    <div class="footer">
        <div class="footer-section">
            <h1>Get to Know Us</h1>
            <a href="#">About Us
                <a href="#">Careers</a>
                <a href="#">Press Releases</a>

        </div>
        <div>
            <h4>Social Medea Icon</h4>
            <a href="https://www.facebook.com/YourPage" target="_blank">
                <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24" width="24" height="24">
                    <path fill="currentColor"
                        d="M20 2H4a2 2 0 0 0-2 2v16a2 2 0 0 0 2 2h8v-7H8V9h4V7c0-2.21 1.79-4 4-4h3v3h-3c-1.1 0-2 .9-2 2v2h5l-1 4H14v7h6a2 2 0 0 0 2-2V4a2 2 0 0 0-2-2z" />
                </svg>
            </a>
            <a href="https://twitter.com/YourHandle" target="_blank">
                <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24" width="24" height="24">
                    <path fill="currentColor"
                        d="M22.46 6c-.78.34-1.56.58-2.38.69.85-.51 1.5-1.32 1.8-2.28-.79.47-1.67.81-2.6 1-1.56-1.67-4.03-1.73-5.6-.15-1.23 1.36-2.97 2.23-4.77 2.42a6.823 6.823 0 0 1-4.14-1.4c-.63 1.18-.98 2.54-.98 4.01 0 2.78 1.42 5.26 3.57 6.69-.05-.54-.02-1.09.12-1.63a2.982 2.982 0 0 1 4.26-2.25c.85.37 1.56 1.01 2.04 1.79a5.974 5.974 0 0 0 1.9-.72c-.22.88-.68 1.67-1.3 2.29a6.94 6.94 0 0 1-1.7.99c.61-.39 1.34-.63 2.1-.63.13 0 .26 0 .39.02a9.93 9.93 0 0 0 5.32-1.54c.25-.18.48-.39.68-.63z" />
                </svg>
            </a>
            <a href="https://www.instagram.com/YourUsername" target="_blank">
                <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24" width="24" height="24">
                    <path fill="currentColor"
                        d="M12 2C6.48 2 2 6.48 2 12s4.48 10 10 10 10-4.48 10-10S17.52 2 12 2zm-1 2h2.04C13.55 4 13 4.55 13 5v10c0 .45.55 1 1.04 1H17l.01-9H14c-.55 0-1-.45-1-1V4zM12 18c-2.21 0-4-1.79-4-4s1.79-4 4-4 4 1.79 4 4-1.79 4-4 4zm6-14h-1.5C16.57 4 16 4.56 16 5v10c0 .45.55 1 1.5 1H18c1.1 0 2-.9 2-2V5c0-1.1-.9-2-2-2z" />
                </svg>
            </a>
        </div>



    </div>
    <div class="social-icons">
        <a href="#" target="_blank">
            <svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24">
                <!-- Include your SVG code here -->
                <path
                    d="M12 2C6.48 2 2 6.48 2 12s4.48 10 10 10 10-4.48 10-10S17.52 2 12 2zm0 18c-4.41 0-8-3.59-8-8s3.59-8 8-8 8 3.59 8 8-3.59 8-8 8zm-1-13h2v6h-2zm0 8h2v2h-2z" />
            </svg>
        </a>
        <!-- Add more social icons as needed -->
    </div>
    <div class="contact">
        <h2>Contact us</h2>
        <input type="text" placeholder="Name" name="user_name" required><br><br>
        <input type="email" placeholder="Email" name="user_email" required><br><br>
        <input type="text" placeholder="Subject" name="user_Subject" required><br><br>
        <textarea placeholder="Type Message" rows="6" name="user_msg" required></textarea><br><br>
        <button name="contact_btn" onclick="sendMessage()">Send Message</button>
    </div>

    <script class="js">
        document.addEventListener("DOMContentLoaded", function () {
            var buyNowButtons = document.querySelectorAll(".buy-now");
            var cartCount = document.getElementById("cart-count");

            var cartItems = 0;

            buyNowButtons.forEach(function (button) {
                button.addEventListener("click", function () {
                    cartItems++;
                    cartCount.textContent = cartItems;
                });
            });
        });
        document.addEventListener("DOMContentLoaded", function () {
            var searchInput = document.querySelector("#search-bar input");
            var products = document.querySelectorAll(".product");

            searchInput.addEventListener("input", function () {
                var searchTerm = searchInput.value.toLowerCase();

                products.forEach(function (product) {
                    var productName = product.querySelector("p").textContent.toLowerCase();
                    var isVisible = productName.includes(searchTerm);
                    product.style.display = isVisible ? "block" : "none";
                });
            });
        });
        document.addEventListener("DOMContentLoaded", function () {
            var footerLinks = document.querySelectorAll(".footer-section a");

            footerLinks.forEach(function (link) {
                link.addEventListener("click", function (event) {
                    event.preventDefault();

                    var targetId = link.getAttribute("href").substring(1);
                    var targetElement = document.getElementById(targetId);

                    if (targetElement) {
                        targetElement.scrollIntoView({ behavior: "smooth" });
                    }
                });
            });
        });
        // JavaScript code goes here
        document.addEventListener("DOMContentLoaded", function () {
            // Get all elements with the class "buy-now"
            var buyNowButtons = document.querySelectorAll(".buy-now");

            // Add click event listener to each "Buy Now" button
            buyNowButtons.forEach(function (button) {
                button.addEventListener("click", function () {
                    // You can customize this alert message or perform other actions
                    alert("Item added to cart!");
                });
            });
        });
        document.addEventListener("DOMContentLoaded", function () {
            var menuIcon = document.getElementById("menu-icon");
            var navLinks = document.getElementById("nav-links");

            // Toggle the visibility of the navigation links on menu icon click
            menuIcon.addEventListener("click", function () {
                navLinks.classList.toggle("show");
            });

            // Hide the navigation links if the window is resized to a larger size
            window.addEventListener("resize", function () {
                if (window.innerWidth > 768) {
                    navLinks.classList.remove("show");
                }
            });
        });

        function sendMessage() {
            var form = document.getElementById("contactForm");
            var formData = new FormData(form);

            var xhr = new XMLHttpRequest();
            xhr.open("POST", "send_email.php", true);
            xhr.onreadystatechange = function () {
                if (xhr.readyState == 4 && xhr.status == 200) {
                    // Handle the server response, e.g., show a success message to the user
                    console.log(xhr.responseText);
                }
            };

            xhr.send(formData);
        }

        function sendMessageViaWhatsApp() {
            var name = document.getElementById("user_name").value;
            var email = document.getElementById("user_email").value;
            var subject = document.getElementById("user_Subject").value;
            var message = document.getElementById("user_msg").value;

            // Create a WhatsApp message with the form data
            var whatsappMessage = `Hi, my name is ${name}. My email is ${email}. Subject: ${subject}. Message: ${message}`;

            // Encode the message for the URL
            var encodedMessage = encodeURIComponent(whatsappMessage);

            // Create the WhatsApp URL
            var whatsappUrl = `https://wa.me/1234567890?text=${encodedMessage}`;

            // Open the WhatsApp URL in a new window or tab
            window.open(whatsappUrl, '_blank');
        }

        function sendMessage() {
            // Replace the following values with your WhatsApp number and desired message
            var whatsappNumber = '1234567890'; // Replace with your WhatsApp number
            var message = 'Hello, I want to get in touch!';

            // Construct the WhatsApp URL
            var whatsappUrl = 'https://wa.me/' + whatsappNumber + '?text= 9460232319' + encodeURIComponent(message);

            // Open WhatsApp in a new tab/window
            window.open(whatsappUrl, '_blank');
        }

        function sendMessage() {
            // Replace 'your_phone_number' with the actual phone number including the country code
            var phoneNumber = 'your_phone_number';

            // Replace 'your_message' with the message you want to send
            var message = 'Name: ' + document.getElementsByName('user_name')[0].value + '\n'
                + 'Email: ' + document.getElementsByName('user_email')[0].value + '\n'
                + 'Subject: ' + document.getElementsByName('user_Subject')[0].value + '\n'
                + 'Message: ' + document.getElementsByName('user_msg')[0].value;

            // Construct the WhatsApp API link
            var whatsappLink = 'https://api.whatsapp.com/send?phone=' + phoneNumber + '&text=' + encodeURIComponent(message);

            // Open the WhatsApp link in a new tab
            window.open(whatsappLink, '_blank');
        }

        function showMessage(message) {
            alert(message);
        }

        function sendMessage() {
            // Get user input
            var userName = document.querySelector('[name="user_name"]').value;
            var userEmail = document.querySelector('[name="user_email"]').value;
            var userSubject = document.querySelector('[name="user_Subject"]').value;
            var userMessage = document.querySelector('[name="user_msg"]').value;

            // Construct WhatsApp message
            var whatsappMessage = `Hi, this is ${userName}. My email is ${userEmail}. Subject: ${userSubject}. Message: ${userMessage}`;

            // Encode message for URL
            var encodedMessage = encodeURIComponent(whatsappMessage);

            // Open WhatsApp with pre-filled message
            window.open(`https://wa.me/?text=${encodedMessage}`, '_blank');
        }

        const express = require('express');
        const app = express();
        const port = 3000;

        app.use(express.static('public')); // Assuming your HTML file is in a 'public' folder

        app.listen(port, () => {
            console.log(`Server is running at http://localhost:${port}`);
        });

        document.addEventListener('DOMContentLoaded', function () {
            // Your existing JavaScript code goes here
        });


        function openSection(section) {
            switch (section) {
                case 'signin':
                    showMessage('Hello, Sign in');
                    // Add code to open Sign In section
                    break;
                case 'returns':
                    showMessage('Returns & Orders');
                    // Add code to open Returns & Orders section
                    break;
                case 'tryprime':
                    showMessage('Try Prime');
                    // Add code to open Try Prime section
                    break;
                case 'cart':
                    showMessage('Cart');
                    // Add code to open Cart section
                    break;
                default:
                    break;
            }
        }

        // Your existing JavaScript code

        function showMessage(message) {
            alert(message);
        }

        function openPage(page) {
            // You can add additional logic here before navigating if needed
            showMessage('Navigating to: ' + page);
            window.location.href = page;
        }

        function showMessage(message) {
            // You can customize this function to handle the message display
            alert(message);
        }

        function sendMessageViaSocialMedia(platform) {
            var name = document.getElementById("user_name").value;
            var email = document.getElementById("user_email").value;
            var subject = document.getElementById("user_Subject").value;
            var message = document.getElementById("user_msg").value;

            // Create a message based on the selected platform
            var socialMediaMessage = `Hi, my name is ${name}. My email is ${email}. Subject: ${subject}. Message: ${message}`;

            // Customize the URL or API endpoint based on the social media platform
            var socialMediaUrl;
            switch (platform) {
                case 'Facebook':
                    // Customize the Facebook direct message URL
                    socialMediaUrl = 'https://www.facebook.com/messages/t/your-facebook-page-id';
                    break;
                case 'Twitter':
                    // Customize the Twitter direct message URL
                    socialMediaUrl = 'https://twitter.com/messages/compose?recipient_id=your-twitter-user-id';
                    break;
                case 'Instagram':
                    // Customize the Instagram direct message URL
                    socialMediaUrl = 'https://www.instagram.com/direct/inbox/';
                    break;
                // Add more cases for other social media platforms if needed
                default:
                    socialMediaUrl = '#'; // Default to a placeholder URL or handle other platforms
                    break;
            }

            // Open the social media direct message link in a new window or tab
            window.open(socialMediaUrl, '_blank');
        }

        // ... (your existing JavaScript code) .
    </script>
    </script>

</body>

</html>
