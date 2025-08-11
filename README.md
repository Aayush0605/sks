<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Shree Krishna Store And Boutique - Premium Fashion & Accessories</title>
    <meta name="description" content="Shree Krishna Store And Boutique - Your premier destination for fashion, clothing, and accessories. Discover our exclusive collection of traditional and modern wear.">
    <meta name="keywords" content="fashion store, boutique, clothing, accessories, traditional wear, modern fashion, Shree Krishna">
    <meta name="author" content="Shree Krishna Store And Boutique">
    <meta property="og:title" content="Shree Krishna Store And Boutique">
    <meta property="og:description" content="Premium Fashion & Accessories Store">
    <meta property="og:type" content="website">
    <link rel="preconnect" href="https://fonts.googleapis.com">
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
    <link href="https://fonts.googleapis.com/css2?family=Playfair+Display:wght@400;600;700&family=Inter:wght@300;400;500;600&display=swap" rel="stylesheet">
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0/css/all.min.css">
    
    <style>
        :root {
            --primary-color: #8B4513;
            --secondary-color: #D4AF37;
            --accent-color: #FF6B35;
            --dark-color: #2C1810;
            --light-color: #F8F6F0;
            --text-dark: #333;
            --text-light: #666;
        }

        /* Dark Mode Variables */
        [data-theme="dark"] {
            --primary-color: #D4AF37;
            --secondary-color: #8B4513;
            --accent-color: #FF8C42;
            --dark-color: #1a1a1a;
            --light-color: #2d2d2d;
            --text-dark: #e0e0e0;
            --text-light: #b0b0b0;
        }

        [data-theme="dark"] body {
            background-color: #1a1a1a;
            color: #e0e0e0;
        }

        [data-theme="dark"] .hero {
            background: linear-gradient(135deg, #2d2d2d, #1a1a1a);
        }

        [data-theme="dark"] .section:nth-child(even) {
            background: #242424 !important;
        }

        [data-theme="dark"] .carousel-container {
            background: #2d2d2d;
            box-shadow: 0 10px 30px rgba(0,0,0,0.3);
        }

        [data-theme="dark"] .nav {
            background: rgba(0,0,0,0.3);
        }

        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        body {
            font-family: 'Inter', sans-serif;
            line-height: 1.6;
            color: var(--text-dark);
            overflow-x: hidden;
        }

        /* Header */
        .header {
            background: linear-gradient(135deg, var(--primary-color), var(--dark-color));
            color: white;
            padding: 1rem 0;
            position: relative;
            box-shadow: 0 2px 20px rgba(0,0,0,0.1);
        }

        .container {
            max-width: 1200px;
            margin: 0 auto;
            padding: 0 2rem;
        }

        .header-top {
            display: flex;
            justify-content: space-between;
            align-items: center;
            flex-wrap: wrap;
            gap: 1rem;
            position: relative;
        }

        /* Theme Toggle */
        .theme-toggle {
            position: absolute;
            top: -0.5rem;
            right: 0;
            background: rgba(255,255,255,0.2);
            border: 2px solid rgba(255,255,255,0.3);
            border-radius: 50px;
            padding: 0.5rem;
            cursor: pointer;
            transition: all 0.3s ease;
            display: flex;
            align-items: center;
            gap: 0.5rem;
            font-size: 0.9rem;
            color: white;
            backdrop-filter: blur(10px);
        }

        .theme-toggle:hover {
            background: rgba(255,255,255,0.3);
            transform: scale(1.05);
        }

        .theme-icon {
            font-size: 1.2rem;
            transition: transform 0.3s ease;
        }

        .theme-toggle.rotating .theme-icon {
            transform: rotate(180deg);
        }

        /* Enhanced animations */
        .fade-in {
            opacity: 0;
            transform: translateY(20px);
            animation: fadeInUp 0.8s ease forwards;
        }

        .slide-in-left {
            opacity: 0;
            transform: translateX(-30px);
            animation: slideInLeft 0.8s ease forwards;
        }

        .slide-in-right {
            opacity: 0;
            transform: translateX(30px);
            animation: slideInRight 0.8s ease forwards;
        }

        @keyframes slideInLeft {
            to {
                opacity: 1;
                transform: translateX(0);
            }
        }

        @keyframes slideInRight {
            to {
                opacity: 1;
                transform: translateX(0);
            }
        }

        /* Improved carousel styling */
        .carousel-slide {
            min-width: 100%;
            height: 100%;
            background: linear-gradient(45deg, var(--primary-color), var(--secondary-color));
            display: flex;
            align-items: center;
            justify-content: center;
            color: white;
            font-size: 1.2rem;
            position: relative;
            font-weight: 600;
            text-shadow: 0 2px 4px rgba(0,0,0,0.3);
        }

        /* Enhanced hover effects */
        .nav-link {
            color: white;
            text-decoration: none;
            padding: 0.5rem 1rem;
            border-radius: 25px;
            transition: all 0.3s ease;
            position: relative;
            overflow: hidden;
        }

        .nav-link::before {
            content: '';
            position: absolute;
            top: 0;
            left: -100%;
            width: 100%;
            height: 100%;
            background: linear-gradient(90deg, transparent, rgba(255,255,255,0.2), transparent);
            transition: left 0.5s ease;
        }

        .nav-link:hover::before {
            left: 100%;
        }

        /* Floating elements */
        .floating {
            animation: floating 3s ease-in-out infinite;
        }

        @keyframes floating {
            0%, 100% { transform: translateY(0px); }
            50% { transform: translateY(-10px); }
        }

        /* Enhanced button styles */
        .cta-button {
            background: linear-gradient(135deg, var(--accent-color), var(--secondary-color));
            color: white;
            padding: 1rem 2rem;
            border: none;
            border-radius: 50px;
            font-size: 1.1rem;
            cursor: pointer;
            transition: all 0.3s ease;
            animation: fadeInUp 1s ease 0.4s both;
            position: relative;
            overflow: hidden;
        }

        .cta-button::before {
            content: '';
            position: absolute;
            top: 0;
            left: -100%;
            width: 100%;
            height: 100%;
            background: linear-gradient(90deg, transparent, rgba(255,255,255,0.2), transparent);
            transition: left 0.5s ease;
        }

        .cta-button:hover::before {
            left: 100%;
        }

        .logo-section {
            display: flex;
            align-items: center;
            gap: 1rem;
        }

        .logo {
            width: 60px;
            height: 60px;
            background: var(--secondary-color);
            border-radius: 50%;
            display: flex;
            align-items: center;
            justify-content: center;
            font-size: 1.5rem;
            font-weight: bold;
            color: var(--dark-color);
            animation: pulse 2s infinite;
        }

        .business-name {
            font-family: 'Playfair Display', serif;
            font-size: 1.8rem;
            font-weight: 600;
        }

        .business-details {
            text-align: right;
            font-size: 0.9rem;
            opacity: 0.9;
        }

        @keyframes pulse {
            0%, 100% { transform: scale(1); }
            50% { transform: scale(1.05); }
        }

        /* Navigation */
        .nav {
            background: rgba(255,255,255,0.1);
            backdrop-filter: blur(10px);
            margin-top: 1rem;
            border-radius: 10px;
        }

        .nav-container {
            display: flex;
            justify-content: space-between;
            align-items: center;
            padding: 0.5rem 1rem;
        }

        .nav-menu {
            display: flex;
            list-style: none;
            gap: 2rem;
        }

        .nav-link {
            color: white;
            text-decoration: none;
            padding: 0.5rem 1rem;
            border-radius: 5px;
            transition: all 0.3s ease;
            position: relative;
        }

        .nav-link:hover {
            background: rgba(255,255,255,0.2);
            transform: translateY(-2px);
        }

        .hamburger {
            display: none;
            flex-direction: column;
            cursor: pointer;
            gap: 4px;
        }

        .hamburger span {
            width: 25px;
            height: 3px;
            background: white;
            transition: 0.3s;
        }

        /* Sidebar */
        .sidebar {
            position: fixed;
            top: 0;
            right: -300px;
            width: 300px;
            height: 100vh;
            background: linear-gradient(135deg, var(--primary-color), var(--dark-color));
            color: white;
            transition: 0.3s ease;
            z-index: 1000;
            padding: 2rem;
        }

        .sidebar.active {
            right: 0;
        }

        .sidebar-close {
            position: absolute;
            top: 1rem;
            right: 1rem;
            background: none;
            border: none;
            color: white;
            font-size: 1.5rem;
            cursor: pointer;
        }

        .sidebar-menu {
            list-style: none;
            margin-top: 3rem;
        }

        .sidebar-menu li {
            margin: 1rem 0;
        }

        .sidebar-menu a {
            color: white;
            text-decoration: none;
            font-size: 1.1rem;
            display: block;
            padding: 0.5rem;
            border-radius: 5px;
            transition: 0.3s;
        }

        .sidebar-menu a:hover {
            background: rgba(255,255,255,0.1);
            transform: translateX(10px);
        }

        /* Main Content */
        .hero {
            background: linear-gradient(135deg, var(--light-color), #fff);
            padding: 4rem 0;
            text-align: center;
        }

        .hero h1 {
            font-family: 'Playfair Display', serif;
            font-size: 3rem;
            color: var(--primary-color);
            margin-bottom: 1rem;
            animation: fadeInUp 1s ease;
        }

        .hero p {
            font-size: 1.2rem;
            color: var(--text-light);
            max-width: 600px;
            margin: 0 auto 2rem;
            animation: fadeInUp 1s ease 0.2s both;
        }

        .cta-button {
            background: linear-gradient(135deg, var(--accent-color), var(--secondary-color));
            color: white;
            padding: 1rem 2rem;
            border: none;
            border-radius: 50px;
            font-size: 1.1rem;
            cursor: pointer;
            transition: 0.3s;
            animation: fadeInUp 1s ease 0.4s both;
        }

        .cta-button:hover {
            transform: translateY(-3px);
            box-shadow: 0 10px 30px rgba(0,0,0,0.2);
        }

        @keyframes fadeInUp {
            from {
                opacity: 0;
                transform: translateY(30px);
            }
            to {
                opacity: 1;
                transform: translateY(0);
            }
        }

        /* Sections */
        .section {
            padding: 4rem 0;
        }

        .section-title {
            font-family: 'Playfair Display', serif;
            font-size: 2.5rem;
            text-align: center;
            margin-bottom: 3rem;
            color: var(--primary-color);
        }

        /* Gallery */
        .gallery-container {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 2rem;
            margin-bottom: 3rem;
        }

        .carousel-container {
            background: white;
            border-radius: 15px;
            overflow: hidden;
            box-shadow: 0 10px 30px rgba(0,0,0,0.1);
            transition: 0.3s;
        }

        .carousel-container:hover {
            transform: translateY(-5px);
            box-shadow: 0 20px 40px rgba(0,0,0,0.15);
        }

        .carousel {
            position: relative;
            height: 250px;
            overflow: hidden;
        }

        .carousel-track {
            display: flex;
            height: 100%;
            transition: transform 0.5s ease;
        }

        .carousel-slide {
            min-width: 100%;
            height: 100%;
            background: linear-gradient(45deg, var(--primary-color), var(--secondary-color));
            display: flex;
            align-items: center;
            justify-content: center;
            color: white;
            font-size: 1.2rem;
            position: relative;
        }

        .carousel-slide::before {
            content: '';
            position: absolute;
            top: 0;
            left: 0;
            right: 0;
            bottom: 0;
            background: url('data:image/svg+xml,<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 100 100"><circle cx="20" cy="20" r="2" fill="rgba(255,255,255,0.1)"/><circle cx="50" cy="50" r="3" fill="rgba(255,255,255,0.1)"/><circle cx="80" cy="30" r="2" fill="rgba(255,255,255,0.1)"/></svg>');
        }

        .carousel-nav {
            position: absolute;
            bottom: 10px;
            left: 50%;
            transform: translateX(-50%);
            display: flex;
            gap: 5px;
        }

        .carousel-dot {
            width: 10px;
            height: 10px;
            border-radius: 50%;
            background: rgba(255,255,255,0.5);
            cursor: pointer;
            transition: 0.3s;
        }

        .carousel-dot.active {
            background: white;
        }

        .carousel-title {
            text-align: center;
            padding: 1rem;
            font-weight: 600;
            color: var(--primary-color);
        }

        /* Map */
        .map-container {
            width: 100%;
            height: 400px;
            border-radius: 15px;
            overflow: hidden;
            box-shadow: 0 10px 30px rgba(0,0,0,0.1);
        }

        /* Footer */
        .footer {
            background: var(--dark-color);
            color: white;
            padding: 3rem 0 1rem;
        }

        .footer-content {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
            gap: 2rem;
            margin-bottom: 2rem;
        }

        .footer-section h3 {
            font-family: 'Playfair Display', serif;
            margin-bottom: 1rem;
            color: var(--secondary-color);
        }

        .footer-section p, .footer-section a {
            color: #ccc;
            text-decoration: none;
            margin-bottom: 0.5rem;
            display: block;
        }

        .footer-section a:hover {
            color: var(--secondary-color);
        }

        .social-links {
            display: flex;
            gap: 1rem;
            margin-top: 1rem;
        }

        .social-links a {
            display: inline-flex;
            align-items: center;
            justify-content: center;
            width: 40px;
            height: 40px;
            background: var(--primary-color);
            border-radius: 50%;
            transition: 0.3s;
        }

        .social-links a:hover {
            background: var(--secondary-color);
            transform: translateY(-3px);
        }

        .footer-bottom {
            text-align: center;
            padding-top: 2rem;
            border-top: 1px solid #444;
            color: #999;
        }

        /* Responsive */
        @media (max-width: 768px) {
            .hamburger {
                display: flex;
            }

            .nav-menu {
                display: none;
            }

            .header-top {
                flex-direction: column;
                text-align: center;
            }

            .business-details {
                text-align: center;
            }

            .hero h1 {
                font-size: 2rem;
            }

            .container {
                padding: 0 1rem;
            }

            .theme-toggle {
                position: static;
                margin-bottom: 1rem;
            }

            .gallery-container {
                grid-template-columns: 1fr;
            }

            .footer-content {
                grid-template-columns: 1fr;
                text-align: center;
            }
        }
    </style>
</head>
<body>
    <!-- Header -->
    <header class="header">
        <div class="container">
            <div class="header-top">
                <!-- Theme Toggle Button -->
                <div class="theme-toggle" onclick="toggleTheme()" id="themeToggle">
                    <span class="theme-icon" id="themeIcon">🌙</span>
                    <span id="themeText">Night</span>
                </div>
                
                <div class="logo-section slide-in-left">
                    <div class="logo floating">SK</div>
                    <div>
                        <div class="business-name">Shree Krishna Store And Boutique</div>
                    </div>
                </div>
                <div class="business-details slide-in-right">
                    <div><strong>GST No:</strong> 24ABCDE1234F1Z5</div>
                    <div><strong>Est:</strong> 2015 | <strong>License:</strong> RET/2015/001</div>
                    <div><strong>Phone:</strong> +91 98765 43210</div>
                </div>
            </div>
            
            <nav class="nav">
                <div class="nav-container">
                    <ul class="nav-menu">
                        <li><a href="#home" class="nav-link">Home</a></li>
                        <li><a href="#shop" class="nav-link">Shop</a></li>
                        <li><a href="#boutique" class="nav-link">Boutique</a></li>
                        <li><a href="#gallery" class="nav-link">Gallery</a></li>
                        <li><a href="#map" class="nav-link">Location</a></li>
                    </ul>
                    <div class="hamburger" onclick="toggleSidebar()">
                        <span></span>
                        <span></span>
                        <span></span>
                    </div>
                </div>
            </nav>
        </div>
    </header>

    <!-- Sidebar -->
    <div class="sidebar" id="sidebar">
        <button class="sidebar-close" onclick="toggleSidebar()">&times;</button>
        <ul class="sidebar-menu">
            <li><a href="#home" onclick="toggleSidebar()">Home</a></li>
            <li><a href="#shop" onclick="toggleSidebar()">Shop</a></li>
            <li><a href="#boutique" onclick="toggleSidebar()">Boutique</a></li>
            <li><a href="#gallery" onclick="toggleSidebar()">Gallery</a></li>
            <li><a href="#map" onclick="toggleSidebar()">Location</a></li>
        </ul>
    </div>

    <!-- Hero Section -->
    <section id="home" class="hero">
        <div class="container">
            <h1 class="fade-in">Welcome to Shree Krishna Store And Boutique</h1>
            <p class="fade-in">Discover premium fashion, traditional wear, and exclusive accessories. Experience the perfect blend of tradition and modern style at our boutique.</p>
            <button class="cta-button" onclick="scrollToSection('gallery')">Explore Collections</button>
        </div>
    </section>

    <!-- Shop Section -->
    <section id="shop" class="section">
        <div class="container">
            <h2 class="section-title">Our Shop</h2>
            <p style="text-align: center; max-width: 800px; margin: 0 auto; font-size: 1.1rem; color: var(--text-light);">
                From everyday essentials to special occasion wear, our shop offers a curated collection of high-quality clothing and accessories. We pride ourselves on providing authentic products that blend traditional craftsmanship with contemporary style.
            </p>
        </div>
    </section>

    <!-- Boutique Section -->
    <section id="boutique" class="section" style="background: var(--light-color);">
        <div class="container">
            <h2 class="section-title">Boutique Collection</h2>
            <p style="text-align: center; max-width: 800px; margin: 0 auto; font-size: 1.1rem; color: var(--text-light);">
                Our boutique specializes in exclusive designer wear, custom tailoring, and premium fashion accessories. Each piece is carefully selected to ensure uniqueness and superior quality for our discerning customers.
            </p>
        </div>
    </section>

    <!-- Gallery Section -->
    <section id="gallery" class="section">
        <div class="container">
            <h2 class="section-title">Gallery</h2>
            <div class="gallery-container">
                <div class="carousel-container">
                    <div class="carousel" data-carousel="0">
                        <div class="carousel-track">
                            <div class="carousel-slide">Traditional Wear Collection</div>
                            <div class="carousel-slide">Ethnic Sarees & Lehengas</div>
                            <div class="carousel-slide">Handcrafted Designs</div>
                        </div>
                        <div class="carousel-nav">
                            <div class="carousel-dot active" onclick="goToSlide(0, 0)"></div>
                            <div class="carousel-dot" onclick="goToSlide(0, 1)"></div>
                            <div class="carousel-dot" onclick="goToSlide(0, 2)"></div>
                        </div>
                    </div>
                    <div class="carousel-title">Traditional Collection</div>
                </div>

                <div class="carousel-container">
                    <div class="carousel" data-carousel="1">
                        <div class="carousel-track">
                            <div class="carousel-slide">Modern Fashion</div>
                            <div class="carousel-slide">Designer Outfits</div>
                            <div class="carousel-slide">Contemporary Styles</div>
                        </div>
                        <div class="carousel-nav">
                            <div class="carousel-dot active" onclick="goToSlide(1, 0)"></div>
                            <div class="carousel-dot" onclick="goToSlide(1, 1)"></div>
                            <div class="carousel-dot" onclick="goToSlide(1, 2)"></div>
                        </div>
                    </div>
                    <div class="carousel-title">Modern Collection</div>
                </div>

                <div class="carousel-container">
                    <div class="carousel" data-carousel="2">
                        <div class="carousel-track">
                            <div class="carousel-slide">Premium Accessories</div>
                            <div class="carousel-slide">Jewelry & Bags</div>
                            <div class="carousel-slide">Fashion Essentials</div>
                        </div>
                        <div class="carousel-nav">
                            <div class="carousel-dot active" onclick="goToSlide(2, 0)"></div>
                            <div class="carousel-dot" onclick="goToSlide(2, 1)"></div>
                            <div class="carousel-dot" onclick="goToSlide(2, 2)"></div>
                        </div>
                    </div>
                    <div class="carousel-title">Accessories</div>
                </div>

                <div class="carousel-container">
                    <div class="carousel" data-carousel="3">
                        <div class="carousel-track">
                            <div class="carousel-slide">Store Interior</div>
                            <div class="carousel-slide">Shopping Experience</div>
                            <div class="carousel-slide">Customer Service</div>
                        </div>
                        <div class="carousel-nav">
                            <div class="carousel-dot active" onclick="goToSlide(3, 0)"></div>
                            <div class="carousel-dot" onclick="goToSlide(3, 1)"></div>
                            <div class="carousel-dot" onclick="goToSlide(3, 2)"></div>
                        </div>
                    </div>
                    <div class="carousel-title">Store Experience</div>
                </div>
            </div>
        </div>
    </section>

    <!-- Map Section -->
    <section id="map" class="section" style="background: var(--light-color);">
        <div class="container">
            <h2 class="section-title">Find Us</h2>
            <div class="map-container">
                <iframe 
                    src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d3423.4!2d75.8573!3d30.9009!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x0%3A0x0!2zMzDCsDU0JzAzLjIiTiA3NcKwNTEnMjYuMyJF!5e0!3m2!1sen!2sin!4v1234567890"
                    width="100%" 
                    height="100%" 
                    style="border:0;" 
                    allowfullscreen="" 
                    loading="lazy">
                </iframe>
            </div>
        </div>
    </section>

    <!-- Footer -->
    <footer class="footer">
        <div class="container">
            <div class="footer-content">
                <div class="footer-section">
                    <h3>Contact Information</h3>
                    <p><i class="fas fa-map-marker-alt"></i> 123 Fashion Street, Commercial Complex</p>
                    <p>Ludhiana, Punjab - 141001</p>
                    <p><i class="fas fa-phone"></i> +91 98765 43210</p>
                    <p><i class="fas fa-envelope"></i> info@shreekrishnastore.com</p>
                </div>
                
                <div class="footer-section">
                    <h3>Business Hours</h3>
                    <p>Monday - Saturday: 10:00 AM - 8:00 PM</p>
                    <p>Sunday: 11:00 AM - 7:00 PM</p>
                    <p>Closed on major festivals</p>
                </div>
                
                <div class="footer-section">
                    <h3>Follow Us</h3>
                    <p>Stay connected for latest collections</p>
                    <div class="social-links">
                        <a href="https://instagram.com/shreekrishnastore" target="_blank">
                            <i class="fab fa-instagram"></i>
                        </a>
                        <a href="https://facebook.com/shreekrishnastore" target="_blank">
                            <i class="fab fa-facebook-f"></i>
                        </a>
                    </div>
                </div>
            </div>
            
            <div class="footer-bottom">
                <p>&copy; 2025 Shree Krishna Store And Boutique. All rights reserved.</p>
            </div>
        </div>
    </footer>

    <script>
        // Theme Toggle Functionality
        function toggleTheme() {
            const body = document.body;
            const themeToggle = document.getElementById('themeToggle');
            const themeIcon = document.getElementById('themeIcon');
            const themeText = document.getElementById('themeText');
            
            // Add rotation animation
            themeToggle.classList.add('rotating');
            
            setTimeout(() => {
                const currentTheme = body.getAttribute('data-theme');
                
                if (currentTheme === 'dark') {
                    body.setAttribute('data-theme', 'light');
                    themeIcon.textContent = '🌙';
                    themeText.textContent = 'Night';
                    localStorage.setItem('theme', 'light');
                } else {
                    body.setAttribute('data-theme', 'dark');
                    themeIcon.textContent = '☀️';
                    themeText.textContent = 'Day';
                    localStorage.setItem('theme', 'dark');
                }
                
                themeToggle.classList.remove('rotating');
            }, 150);
        }

        // Load saved theme
        function loadTheme() {
            const savedTheme = localStorage.getItem('theme') || 'light';
            const body = document.body;
            const themeIcon = document.getElementById('themeIcon');
            const themeText = document.getElementById('themeText');
            
            body.setAttribute('data-theme', savedTheme);
            
            if (savedTheme === 'dark') {
                themeIcon.textContent = '☀️';
                themeText.textContent = 'Day';
            } else {
                themeIcon.textContent = '🌙';
                themeText.textContent = 'Night';
            }
        }

        // Scroll to section function
        function scrollToSection(sectionId) {
            const section = document.getElementById(sectionId);
            if (section) {
                section.scrollIntoView({
                    behavior: 'smooth',
                    block: 'start'
                });
            }
        }

        // Sidebar functionality
        function toggleSidebar() {
            const sidebar = document.getElementById('sidebar');
            sidebar.classList.toggle('active');
        }

        // Smooth scrolling for navigation links
        document.querySelectorAll('a[href^="#"]').forEach(anchor => {
            anchor.addEventListener('click', function (e) {
                e.preventDefault();
                const target = document.querySelector(this.getAttribute('href'));
                if (target) {
                    target.scrollIntoView({
                        behavior: 'smooth',
                        block: 'start'
                    });
                }
            });
        });

        // Carousel functionality
        const carousels = document.querySelectorAll('.carousel');
        
        function goToSlide(carouselIndex, slideIndex) {
            const carousel = carousels[carouselIndex];
            const track = carousel.querySelector('.carousel-track');
            const dots = carousel.querySelectorAll('.carousel-dot');
            
            track.style.transform = `translateX(-${slideIndex * 100}%)`;
            
            dots.forEach((dot, index) => {
                dot.classList.toggle('active', index === slideIndex);
            });
        }

        // Auto-play carousels
        let carouselIntervals = [];
        
        carousels.forEach((carousel, carouselIndex) => {
            let currentSlide = 0;
            const totalSlides = carousel.querySelectorAll('.carousel-slide').length;
            
            const interval = setInterval(() => {
                currentSlide = (currentSlide + 1) % totalSlides;
                goToSlide(carouselIndex, currentSlide);
            }, 4000 + (carouselIndex * 1000)); // Stagger the timing
            
            carouselIntervals.push(interval);
        });

        // Enhanced Intersection Observer for animations
        const observerOptions = {
            threshold: 0.1,
            rootMargin: '0px 0px -50px 0px'
        };

        const observer = new IntersectionObserver((entries) => {
            entries.forEach(entry => {
                if (entry.isIntersecting) {
                    entry.target.style.opacity = '1';
                    entry.target.style.transform = 'translateY(0) translateX(0)';
                    
                    // Add staggered animation for gallery items
                    if (entry.target.classList.contains('carousel-container')) {
                        const delay = Array.from(entry.target.parentNode.children).indexOf(entry.target) * 200;
                        entry.target.style.transitionDelay = `${delay}ms`;
                    }
                }
            });
        }, observerOptions);

        // Observe elements for scroll animations
        document.querySelectorAll('.carousel-container, .fade-in, .slide-in-left, .slide-in-right').forEach(element => {
            if (!element.style.opacity) {
                element.style.opacity = '0';
                element.style.transform = element.classList.contains('slide-in-left') ? 'translateX(-30px)' :
                                         element.classList.contains('slide-in-right') ? 'translateX(30px)' :
                                         'translateY(30px)';
                element.style.transition = 'opacity 0.8s ease, transform 0.8s ease';
            }
            observer.observe(element);
        });

        // Close sidebar when clicking outside
        document.addEventListener('click', (e) => {
            const sidebar = document.getElementById('sidebar');
            const hamburger = document.querySelector('.hamburger');
            
            if (!sidebar.contains(e.target) && !hamburger.contains(e.target)) {
                sidebar.classList.remove('active');
            }
        });

        // Parallax effect for hero section
        window.addEventListener('scroll', () => {
            const scrolled = window.pageYOffset;
            const hero = document.querySelector('.hero');
            if (hero) {
                hero.style.transform = `translateY(${scrolled * 0.5}px)`;
            }
        });

        // Initialize theme and loading animation
        window.addEventListener('load', () => {
            loadTheme();
            document.body.style.opacity = '1';
            document.body.style.transition = 'opacity 0.5s ease';
            
            // Trigger initial animations
            setTimeout(() => {
                document.querySelectorAll('.fade-in, .slide-in-left, .slide-in-right').forEach(el => {
                    if (el.getBoundingClientRect().top < window.innerHeight) {
                        el.style.opacity = '1';
                        el.style.transform = 'translateY(0) translateX(0)';
                    }
                });
            }, 100);
        });

        // Set initial body opacity
        document.body.style.opacity = '0';
    </script>
</body>
</html>
