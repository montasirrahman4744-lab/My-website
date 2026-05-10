# My-website
    A simple electrical maintenance website
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1" />
    <title>The Legend Electrical Maintenance</title>
    <style>
        /* Reset and basic styles */
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
        }

        body {
            background-color: #000;
            color: #fff;
            line-height: 1.6;
        }

        /* Header and navigation */
        header {
            background-color: #111;
            padding: 20px 40px;
            display: flex;
            align-items: center;
            justify-content: space-between;
            border-bottom: 2px solid #0af;
        }

        .logo {
            display: flex;
            align-items: center;
        }

        .logo svg {
            width: 50px;
            height: 50px;
            margin-right: 15px;
        }

        .logo-text {
            font-size: 1.5rem;
            font-weight: bold;
            letter-spacing: 2px;
            color: #0af;
        }

        .logo-text span.electrical {
            color: #ff2200;
            text-transform: uppercase;
            font-weight: 900;
            margin: 0 5px;
            letter-spacing: 3px;
        }

        nav ul {
            list-style: none;
            display: flex;
            gap: 30px;
        }

        nav ul li a {
            color: #fff;
            text-decoration: none;
            font-size: 1.1rem;
            transition: color 0.3s ease;
        }

        nav ul li a:hover {
            color: #0af;
        }

        /* Hero Section */
        .hero {
            display: flex;
            flex-direction: column;
            justify-content: center;
            align-items: center;
            height: 70vh;
            text-align: center;
            padding: 0 20px;
            border-bottom: 2px solid #0af;
        }

        .hero h1 {
            font-size: 3rem;
            margin-bottom: 20px;
            color: #0af;
            text-shadow: 0 0 15px #0af;
        }

        .hero p {
            font-size: 1.3rem;
            max-width: 700px;
            color: #ddd;
        }

        /* About Section */
        section.about,
        section.services,
        section.products,
        section.contact {
            padding: 60px 40px;
            max-width: 1100px;
            margin: auto;
        }

        section h2 {
            font-size: 2.5rem;
            margin-bottom: 30px;
            color: #0af;
            text-align: center;
            text-shadow: 0 0 10px #0af;
        }

        section p {
            font-size: 1.1rem;
            color: #ccc;
            max-width: 900px;
            margin: 0 auto 40px;
            line-height: 1.5;
            text-align: center;
        }

        /* Services & Products grid */
        .grid-container {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
            gap: 30px;
            max-width: 1000px;
            margin: auto;
        }

        .grid-item {
            background-color: #111;
            padding: 20px;
            border-radius: 10px;
            box-shadow: 0 0 10px #0af;
            text-align: center;
            transition: transform 0.3s ease;
        }

        .grid-item:hover {
            transform: scale(1.05);
            box-shadow: 0 0 20px #ff2200;
        }

        .grid-item h3 {
            margin-bottom: 15px;
            color: #0af;
        }

        .grid-item p {
            color: #bbb;
        }

        /* Contact form */
        form {
            max-width: 600px;
            margin: auto;
            text-align: left;
        }

        form label {
            display: block;
            margin-bottom: 8px;
            color: #0af;
            font-weight: 600;
        }

        form input[type="text"],
        form input[type="email"],
        form textarea {
            width: 100%;
            padding: 10px;
            border-radius: 7px;
            border: none;
            margin-bottom: 20px;
            font-size: 1rem;
            resize: vertical;
        }

        form button {
            background-color: #0af;
            color: #000;
            border: none;
            padding: 15px 30px;
            font-size: 1.1rem;
            font-weight: bold;
            border-radius: 10px;
            cursor: pointer;
            transition: background-color 0.3s ease;
            width: 100%;
        }

        form button:hover {
            background-color: #ff2200;
            color: #fff;
        }

        /* Footer */
        footer {
            text-align: center;
            padding: 20px;
            background-color: #111;
            color: #666;
            margin-top: 40px;
        }

        @media (max-width: 600px) {
            nav ul {
                flex-direction: column;
                gap: 15px;
            }

            header {
                flex-direction: column;
                gap: 15px;
            }

            .hero h1 {
                font-size: 2.2rem;
            }
        }
    </style>
</head>
<body>

<header>
    <div class="logo">
        <!-- Simplified lightning bolt as an SVG to mimic the logo style -->
        <svg viewBox="0 0 64 64" fill="none" xmlns="http://www.w3.org/2000/svg" stroke="#0af" stroke-width="4" stroke-linejoin="round">
            <path d="M20 2 L45 2 L25 35 L40 35 L10 62 L35 25 L20 25 Z"/>
        </svg>
        <div class="logo-text">
            THE LEGEND <span class="electrical">ELECTRICAL</span> MAINTENANCE
        </div>
    </div>
    <nav>
        <ul>
            <li><a href="#about">About</a></li>
            <li><a href="#services">Services</a></li>
            <li><a href="#products">Products</a></li>
            <li><a href="#contact">Contact</a></li>
        </ul>
    </nav>
</header>

<section class="hero">
    <h1>Your Trusted Electrical Panel Board Experts</h1>
    <p>Delivering quality electrical maintenance and premium panel boards to keep your power safe and reliable.</p>
</section>

<section id="about" class="about">
    <h2>About Us</h2>
    <p>
        The Legend Electrical Maintenance has been a leader in electrical panel board manufacturing and maintenance for over 20 years. 
        We specialize in providing customized electrical solutions that ensure safety, efficiency, and durability for residential, commercial, and industrial clients.
    </p>
</section>

<section id="services" class="services">
    <h2>Our Services</h2>
    <div class="grid-container">
        <div class="grid-item">
            <h3>Panel Board Manufacturing</h3>
            <p>Custom electrical panel boards crafted with precision and premium components to meet your specific needs.</p>
        </div>
        <div class="grid-item">
            <h3>Electrical Maintenance</h3>
            <p>Comprehensive maintenance services to ensure optimal performance and longevity of your electrical systems.</p>
        </div>
        <div class="grid-item">
            <h3>Installation & Testing</h3>
            <p>Professional installation and rigorous testing to guarantee safety and compliance with industry standards.</p>
        </div>
    </div>
</section>

<section id="products" class="products">
    <h2>Our Products</h2>
    <div class="grid-container">
        <div class="grid-item">
            <h3>Distribution Boards</h3>
            <p>Robust and reliable distribution boards designed for precise power distribution and protection.</p>
        </div>
        <div class="grid-item">
            <h3>Control Panels</h3>
            <p>Advanced control panels for industrial and commercial electrical systems with user-friendly interfaces.</p>
        </div>
        <div class="grid-item">
            <h3>Switchgear Assemblies</h3>
            <p>Durable switchgear assemblies ensuring safety and efficiency in power control and protection.</p>
        </div>
    </div>
</section>

<section id="contact" class="contact">
    <h2>Contact Us</h2>
    <form action="#" method="post">
        <label for="name">Full Name</label>
        <input type="text" id="name" name="name" required placeholder="Your full name" />

        <label for="email">Email Address</label>
        <input type="email" id="email" name="email" required placeholder="Your email address" />

        <label for="message">Message</label>
        <textarea id="message" name="message" rows="5" required placeholder="Write your message here"></textarea>

        <button type="submit">Send Message</button>
    </form>
</section>

<footer>
    &copy; 2024 The Legend Electrical Maintenance. All rights reserved.
</footer>

</body>
</html>
