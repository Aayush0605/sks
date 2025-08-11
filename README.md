<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Shree Krishna Store And Boutique - Premium Fashion & Boutique Services</title>
    
    <!-- Enhanced SEO Meta Tags -->
    <meta name="description" content="Shree Krishna Store And Boutique - Your premier destination for elegant fashion, custom boutique services, and traditional wear. GST registered business offering quality apparel and personalized styling.">
    <meta name="keywords" content="Shree Krishna Store, Boutique, Fashion Store, Custom Tailoring, Traditional Wear, Modern Fashion, GST Registered, Premium Apparel, Wedding Outfits">
    <meta name="author" content="Shree Krishna Store And Boutique">
    <meta name="robots" content="index, follow">
    
    <!-- Open Graph Tags for Social Media -->
    <meta property="og:title" content="Shree Krishna Store And Boutique">
    <meta property="og:description" content="Premium Fashion & Boutique Services - Custom tailoring and elegant apparel">
    <meta property="og:type" content="business.business">
    <meta property="og:url" content="https://shreekrishnaboutique.com">
    
    <!-- Favicon -->
    <link rel="icon" href="logo.png" type="image/png">
    <link rel="apple-touch-icon" href="logo.png">
    
    <!-- Google Fonts -->
    <link href="https://fonts.googleapis.com/css2?family=Playfair+Display:wght@400;600;700&family=Inter:wght@300;400;500;600&display=swap" rel="stylesheet">
    
    <style>
        :root {
            --primary: #2c3e50;
            --secondary: #ecf0f1;
            --accent: #e74c3c;
            --gold: #f39c12;
            --text-dark: #2c3e50;
            --text-light: #7f8c8d;
            --white: #ffffff;
            --shadow: 0 4px 15px rgba(0,0,0,0.1);
        }

        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        body {
            font-family: 'Inter', sans-serif;
            line-height: 1.6;
            background: var(--secondary);
            color: var(--text-dark);
        }

        /* Compact Header */
        .header-wrapper {
            background: linear-gradient(135deg, var(--primary) 0%, #34495e 100%);
            box-shadow: var(--shadow);
            position: sticky;
            top: 0;
            z-index: 1000;
        }

        .top-header {
            background: rgba(0,0,0,0.1);
            padding: 5px 0;
            font-size: 0.8rem;
            color: rgba(255,255,255,0.9);
            text-align: center;
        }

        .container {
            max-width: 1200px;
            margin: 0 auto;
            padding: 0 20px;
        }

        .main-header {
            padding: 15px 0;
        }

        .header-content {
            display: flex;
            align-items: center;
            justify-content: space-between;
            flex-wrap: wrap;
        }

        .logo-section {
            display: flex;
            align-items: center;
            gap: 12px;
        }

        .logo {
            width: 50px;
            height: 50px;
            border-radius: 50%;
            border: 2px solid var(--gold);
            object-fit: cover;
            background: var(--white);
            padding: 3px;
        }

        .brand-text h1 {
            font-family: 'Playfair Display', serif;
            font-size: 1.8rem;
            font-weight: 700;
            color: var(--white);
            text-shadow: 2px 2px 4px rgba(0,0,0,0.3);
            margin-bottom: 2px;
        }

        .brand-text .tagline {
            color: var(--gold);
            font-size: 0.75rem;
            font-weight: 500;
            letter-spacing: 0.5px;
        }

        .business-info {
            background: rgba(255,255,255,0.1);
            padding: 10px 15px;
            border-radius: 8px;
            margin: 12px 0;
            backdrop-filter: blur(10px);
        }

        .info-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(200px, 1fr));
            gap: 10px;
            color: var(--white);
            font-size: 0.85rem;
        }

        .info-item {
            display: flex;
            align-items: center;
            gap: 8px;
        }

        .info-icon {
            width: 16px;
            height: 16px;
            background: var(--gold);
            border-radius: 50%;
            display: flex;
            align-items: center;
            justify-content: center;
            font-size: 10px;
        }

        /* Navigation */
        .nav-wrapper {
            background: rgba(0,0,0,0.1);
            backdrop-filter: blur(10px);
        }

        .horizontal-nav {
            display: flex;
            justify-content: center;
            padding: 0;
        }

        .horizontal-nav a {
            color: var(--white);
            text-decoration: none;
            padding: 12px 20px;
            font-weight: 500;
            font-size: 0.95rem;
            transition: all 0.3s ease;
            position: relative;
            overflow: hidden;
        }

        .horizontal-nav a:hover {
            background: var(--gold);
            transform: translateY(-2px);
        }

        .horizontal-nav a::before {
            content: '';
            position: absolute;
            bottom: 0;
            left: 0;
            width: 0;
            height: 3px;
            background: var(--gold);
            transition: width 0.3s ease;
        }

        .horizontal-nav a:hover::before {
            width: 100%;
        }

        /* Hamburger Menu */
        .hamburger {
            display: none;
            flex-direction: column;
            cursor: pointer;
            padding: 8px;
        }

        .hamburger-line {
            width: 25px;
            height: 2px;
            background: var(--white);
            margin: 2px 0;
            transition: 0.3s;
            border-radius: 2px;
        }

        .hamburger.active .hamburger-line:nth-child(1) {
            transform: rotate(-45deg) translate(-4px, 5px);
        }

        .hamburger.active .hamburger-line:nth-child(2) {
            opacity: 0;
        }

        .hamburger.active .hamburger-line:nth-child(3) {
            transform: rotate(45deg) translate(-4px, -5px);
        }

        /* Sidebar */
        .sidebar {
            position: fixed;
            top: 0;
            left: -300px;
            width: 300px;
            height: 100vh;
            background: linear-gradient(180deg, var(--primary) 0%, #34495e 100%);
            transition: left 0.4s ease;
            z-index: 1001;
            padding-top: 80px;
            box-shadow: 2px 0 15px rgba(0,0,0,0.3);
        }

        .sidebar.open {
            left: 0;
        }

        .sidebar-close {
            position: absolute;
            top: 20px;
            right: 20px;
            background: none;
            border: none;
            color: var(--white);
            font-size: 30px;
            cursor: pointer;
            transition: transform 0.3s ease;
        }

        .sidebar-close:hover {
            transform: rotate(90deg);
        }

        .sidebar-nav {
            padding: 0;
        }

        .sidebar-nav a {
            display: block;
            color: var(--white);
            text-decoration: none;
            padding: 20px 30px;
            font-size: 1.1rem;
            font-weight: 500;
            border-bottom: 1px solid rgba(255,255,255,0.1);
            transition: all 0.3s ease;
        }

        .sidebar-nav a:hover {
            background: var(--gold);
            padding-left: 40px;
        }

        /* Overlay */
        .overlay {
            position: fixed;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            background: rgba(0,0,0,0.5);
            z-index: 1000;
            opacity: 0;
            visibility: hidden;
            transition: all 0.3s ease;
        }

        .overlay.active {
            opacity: 1;
            visibility: visible;
        }

        /* Main Content */
        .main-content {
            padding: 40px 0;
        }

        .section {
            margin-bottom: 60px;
            scroll-margin-top: 100px;
        }

        .section-title {
            font-family: 'Playfair Display', serif;
            font-size: 2.5rem;
            color: var(--primary);
            margin-bottom: 20px;
            text-align: center;
            position: relative;
        }

        .section-title::after {
            content: '';
            position: absolute;
            bottom: -10px;
            left: 50%;
            transform: translateX(-50%);
            width: 80px;
            height: 3px;
            background: var(--gold);
        }

        .section-content {
            background: var(--white);
            padding: 40px;
            border-radius: 15px;
            box-shadow: var(--shadow);
            margin-top: 30px;
        }

        /* Gallery */
        .gallery-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(350px, 1fr));
            gap: 30px;
            margin-top: 30px;
        }

        .carousel-card {
            background: var(--white);
            border-radius: 15px;
            overflow: hidden;
            box-shadow: var(--shadow);
            transition: transform 0.3s ease;
        }

        .carousel-card:hover {
            transform: translateY(-10px);
        }

        .carousel-container {
            position: relative;
            height: 250px;
            overflow: hidden;
        }

        .carousel-image {
            width: 100%;
            height: 100%;
            object-fit: cover;
            transition: transform 0.3s ease;
        }

        .carousel-controls {
            position: absolute;
            top: 50%;
            transform: translateY(-50%);
            background: rgba(0,0,0,0.7);
            color: var(--white);
            border: none;
            width: 40px;
            height: 40px;
            border-radius: 50%;
            cursor: pointer;
            font-size: 18px;
            transition: all 0.3s ease;
        }

        .carousel-controls:hover {
            background: var(--gold);
            transform: translateY(-50%) scale(1.1);
        }

        .prev { left: 15px; }
        .next { right: 15px; }

        .carousel-info {
            padding: 20px;
            text-align: center;
        }

        .carousel-info h3 {
            font-family: 'Playfair Display', serif;
            color: var(--primary);
            margin-bottom: 10px;
        }

        .carousel-dots {
            display: flex;
            justify-content: center;
            gap: 8px;
            margin-top: 15px;
        }

        .dot {
            width: 12px;
            height: 12px;
            border-radius: 50%;
            background: #ddd;
            cursor: pointer;
            transition: all 0.3s ease;
        }

        .dot.active {
            background: var(--gold);
            transform: scale(1.2);
        }

        /* Map - Properly Responsive */
        .map-container {
            border-radius: 15px;
            overflow: hidden;
            box-shadow: var(--shadow);
            margin-top: 30px;
            position: relative;
            width: 100%;
            height: 0;
            padding-bottom: 56.25%; /* 16:9 aspect ratio */
        }

        .map-container iframe {
            position: absolute;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            border: none;
        }

        /* Footer */
        .footer {
            background: linear-gradient(135deg, var(--primary) 0%, #34495e 100%);
            color: var(--white);
            padding: 40px 0 20px;
            margin-top: 60px;
        }

        .footer-content {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
            gap: 30px;
            margin-bottom: 30px;
        }

        .footer-section h3 {
            font-family: 'Playfair Display', serif;
            color: var(--gold);
            margin-bottom: 15px;
        }

        .social-links {
            display: flex;
            gap: 15px;
            margin-top: 15px;
        }

        .social-links a {
            display: flex;
            align-items: center;
            justify-content: center;
            width: 40px;
            height: 40px;
            background: var(--gold);
            border-radius: 50%;
            color: var(--white);
            text-decoration: none;
            transition: all 0.3s ease;
        }

        .social-links a:hover {
            transform: translateY(-3px);
            box-shadow: 0 5px 15px rgba(243, 156, 18, 0.4);
        }

        .footer-bottom {
            text-align: center;
            padding-top: 20px;
            border-top: 1px solid rgba(255,255,255,0.1);
            color: rgba(255,255,255,0.8);
        }

        /* Responsive Design */
        @media (max-width: 768px) {
            .horizontal-nav {
                display: none;
            }

            .hamburger {
                display: flex;
            }

            .brand-text h1 {
                font-size: 1.4rem;
            }

            .header-content {
                flex-direction: column;
                gap: 10px;
                text-align: center;
            }

            .info-grid {
                grid-template-columns: 1fr;
                font-size: 0.8rem;
            }

            .section-title {
                font-size: 2rem;
            }

            .section-content {
                padding: 20px;
            }

            .gallery-grid {
                grid-template-columns: 1fr;
            }

            .business-info {
                padding: 8px 12px;
            }

            .main-header {
                padding: 10px 0;
            }
        }

        @media (max-width: 480px) {
            .container {
                padding: 0 15px;
            }

            .brand-text h1 {
                font-size: 1.2rem;
            }

            .brand-text .tagline {
                font-size: 0.7rem;
            }

            .logo {
                width: 40px;
                height: 40px;
            }

            .section-title {
                font-size: 1.8rem;
            }

            .top-header {
                font-size: 0.7rem;
                padding: 3px 0;
            }

            .info-grid {
                font-size: 0.75rem;
            }

            .info-item {
                gap: 6px;
            }

            .info-icon {
                width: 14px;
                height: 14px;
                font-size: 8px;
            }
        }

        /* Smooth scrolling */
        html {
            scroll-behavior: smooth;
        }

        /* Loading animation */
        .loading {
            opacity: 0;
            transform: translateY(20px);
            transition: all 0.6s ease;
        }

        .loading.loaded {
            opacity: 1;
            transform: translateY(0);
        }
    </style>
</head>
<body>
    <!-- Header -->
    <header class="header-wrapper">
        <div class="top-header">
            <div class="container">
                📞 +91-9876543210 | 📧 info@shreekrishnaboutique.com | 🕒 Mon-Sat: 10AM-8PM
            </div>
        </div>
        
        <div class="main-header">
            <div class="container">
                <div class="header-content">
                    <div class="logo-section">
                        <img src="logo.png" alt="Shree Krishna Store Logo" class="logo">
                        <div class="brand-text">
                            <h1>Shree Krishna Store And Boutique</h1>
                            <div class="tagline">Premium Fashion & Custom Tailoring</div>
                        </div>
                    </div>
                    
                    <div class="hamburger" onclick="toggleSidebar()">
                        <div class="hamburger-line"></div>
                        <div class="hamburger-line"></div>
                        <div class="hamburger-line"></div>
                    </div>
                </div>
                
                <div class="business-info">
                    <div class="info-grid">
                        <div class="info-item">
                            <div class="info-icon">📋</div>
                            <span>GST No: 27AAAPL1234S1Z5</span>
                        </div>
                        <div class="info-item">
                            <div class="info-icon">📅</div>
                            <span>Established: 2015</span>
                        </div>
                        <div class="info-item">
                            <div class="info-icon">⭐</div>
                            <span>Premium Quality Assured</span>
                        </div>
                        <div class="info-item">
                            <div class="info-icon">✂️</div>
                            <span>Custom Tailoring Available</span>
                        </div>
                    </div>
                </div>
            </div>
        </div>
        
        <nav class="nav-wrapper">
            <div class="container">
                <div class="horizontal-nav">
                    <a href="#home">Home</a>
                    <a href="#shop">Shop</a>
                    <a href="#boutique">Boutique</a>
                    <a href="#gallery">Gallery</a>
                    <a href="#map">Location</a>
                </div>
            </div>
        </nav>
    </header>

    <!-- Sidebar -->
    <div class="overlay" onclick="closeSidebar()"></div>
    <nav class="sidebar" id="sidebar">
        <button class="sidebar-close" onclick="closeSidebar()">&times;</button>
        <div class="sidebar-nav">
            <a href="#home" onclick="closeSidebar()">Home</a>
            <a href="#shop" onclick="closeSidebar()">Shop</a>
            <a href="#boutique" onclick="closeSidebar()">Boutique</a>
            <a href="#gallery" onclick="closeSidebar()">Gallery</a>
            <a href="#map" onclick="closeSidebar()">Location</a>
        </div>
    </nav>

    <!-- Main Content -->
    <main class="main-content">
        <div class="container">
            <!-- Home Section -->
            <section id="home" class="section loading">
                <h2 class="section-title">Welcome to Our Store</h2>
                <div class="section-content">
                    <p>Welcome to Shree Krishna Store And Boutique, your premier destination for exquisite fashion and personalized styling. Since 2015, we have been serving our customers with the finest collection of traditional and contemporary wear, complemented by our expert boutique services.</p>
                    <p>Our commitment to quality, craftsmanship, and customer satisfaction has made us a trusted name in the fashion industry. Whether you're looking for everyday wear or special occasion outfits, we have something perfect for every style and budget.</p>
                </div>
            </section>

            <!-- Shop Section -->
            <section id="shop" class="section loading">
                <h2 class="section-title">Our Shop</h2>
                <div class="section-content">
                    <p>Discover our extensive collection of carefully curated fashion items for men, women, and children. Our shop features:</p>
                    <ul style="margin: 20px 0; padding-left: 20px;">
                        <li>Designer Sarees & Lehengas</li>
                        <li>Ethnic Wear & Traditional Outfits</li>
                        <li>Contemporary Fashion</li>
                        <li>Formal & Casual Wear</li>
                        <li>Accessories & Jewelry</li>
                        <li>Wedding Collection</li>
                    </ul>
                    <p>All our products are sourced from trusted manufacturers and undergo strict quality checks to ensure you receive only the best.</p>
                </div>
            </section>

            <!-- Boutique Section -->
            <section id="boutique" class="section loading">
                <h2 class="section-title">Boutique Services</h2>
                <div class="section-content">
                    <p>Our boutique services offer personalized fashion solutions tailored to your unique style and preferences:</p>
                    <ul style="margin: 20px 0; padding-left: 20px;">
                        <li>Custom Tailoring & Alterations</li>
                        <li>Personal Styling Consultation</li>
                        <li>Bridal & Groom Outfit Design</li>
                        <li>Party Wear Customization</li>
                        <li>Corporate Uniform Solutions</li>
                        <li>Fashion Design Services</li>
                    </ul>
                    <p>Our experienced team of designers and tailors work closely with you to create outfits that perfectly fit your vision and body type.</p>
                </div>
            </section>

            <!-- Gallery Section -->
            <section id="gallery" class="section loading">
                <h2 class="section-title">Gallery</h2>
                <div class="gallery-grid">
                    <!-- Shop Collection Carousel -->
                    <div class="carousel-card">
                        <div class="carousel-container">
                            <img class="carousel-image" id="carousel-0" src="shop1.jpg" alt="Shop Collection">
                            <button class="carousel-controls prev" onclick="changeSlide(0, -1)">❮</button>
                            <button class="carousel-controls next" onclick="changeSlide(0, 1)">❯</button>
                        </div>
                        <div class="carousel-info">
                            <h3>Shop Collections</h3>
                            <p>Browse our latest arrivals and trending fashion pieces</p>
                            <div class="carousel-dots" id="dots-0"></div>
                        </div>
                    </div>

                    <!-- Boutique Work Carousel -->
                    <div class="carousel-card">
                        <div class="carousel-container">
                            <img class="carousel-image" id="carousel-1" src="boutique1.jpg" alt="Boutique Work">
                            <button class="carousel-controls prev" onclick="changeSlide(1, -1)">❮</button>
                            <button class="carousel-controls next" onclick="changeSlide(1, 1)">❯</button>
                        </div>
                        <div class="carousel-info">
                            <h3>Custom Designs</h3>
                            <p>Explore our exclusive boutique creations and custom work</p>
                            <div class="carousel-dots" id="dots-1"></div>
                        </div>
                    </div>

                    <!-- Bridal Collection Carousel -->
                    <div class="carousel-card">
                        <div class="carousel-container">
                            <img class="carousel-image" id="carousel-2" src="bridal1.jpg" alt="Bridal Collection">
                            <button class="carousel-controls prev" onclick="changeSlide(2, -1)">❮</button>
                            <button class="carousel-controls next" onclick="changeSlide(2, 1)">❯</button>
                        </div>
                        <div class="carousel-info">
                            <h3>Bridal Special</h3>
                            <p>Stunning bridal wear and wedding collection pieces</p>
                            <div class="carousel-dots" id="dots-2"></div>
                        </div>
                    </div>
                </div>
            </section>

            <!-- Map Section -->
            <section id="map" class="section loading">
                <h2 class="section-title">Visit Our Store</h2>
                <div class="section-content">
                    <p>Come visit us at our conveniently located store. We're easily accessible and offer ample parking for your convenience.</p>
                </div>
                <div class="map-container">
                    <iframe 
                        src="https://www.google.com/maps/embed?pb=!4v1754203732224!6m8!1m7!1su6mOY7SaJlCCU504dS-znw!2m2!1d30.92690430824867!2d75.82649617618698!3f99.70628912152816!4f8.689456381317555!5f0.7820865974627469"
                        allowfullscreen="" 
                        loading="lazy" 
                        referrerpolicy="no-referrer-when-downgrade">
                    </iframe>
                </div>
            </section>
        </div>
    </main>

    <!-- Footer -->
    <footer class="footer">
        <div class="container">
            <div class="footer-content">
                <div class="footer-section">
                    <h3>Contact Information</h3>
                    <p>📍 123 Fashion Street, Main Market<br>
                    Your City, State 123456</p>
                    <p>📞 +91-9876543210<br>
                    📧 info@shreekrishnaboutique.com</p>
                </div>
                
                <div class="footer-section">
                    <h3>Business Hours</h3>
                    <p>Monday - Saturday: 10:00 AM - 8:00 PM<br>
                    Sunday: 11:00 AM - 6:00 PM</p>
                    <p>GST No: 27AAAPL1234S1Z5</p>
                </div>
                
                <div class="footer-section">
                    <h3>Follow Us</h3>
                    <p>Stay connected for latest updates and offers</p>
                    <div class="social-links">
                        <a href="https://instagram.com/shreekrishnaboutique" target="_blank" title="Instagram">📷</a>
                        <a href="https://facebook.com/shreekrishnaboutique" target="_blank" title="Facebook">📘</a>
                        <a href="https://whatsapp.com/9876543210" target="_blank" title="WhatsApp">💬</a>
                    </div>
                </div>
            </div>
            
            <div class="footer-bottom">
                <p>&copy; 2025 Shree Krishna Store And Boutique. All rights reserved. | Designed with ❤️</p>
            </div>
        </div>
    </footer>

    <script>
        // Gallery carousel data
        const carouselData = [
            {
                images: ['shop1.jpg', 'shop2.jpg', 'shop3.jpg', 'shop4.jpg'],
                currentIndex: 0
            },
            {
                images: ['boutique1.jpg', 'boutique2.jpg', 'boutique3.jpg'],
                currentIndex: 0
            },
            {
                images: ['bridal1.jpg', 'bridal2.jpg', 'bridal3.jpg', 'bridal4.jpg', 'bridal5.jpg'],
                currentIndex: 0
            }
        ];

        // Sidebar functionality
        function toggleSidebar() {
            const sidebar = document.getElementById('sidebar');
            const overlay = document.querySelector('.overlay');
            const hamburger = document.querySelector('.hamburger');
            
            sidebar.classList.toggle('open');
            overlay.classList.toggle('active');
            hamburger.classList.toggle('active');
        }

        function closeSidebar() {
            const sidebar = document.getElementById('sidebar');
            const overlay = document.querySelector('.overlay');
            const hamburger = document.querySelector('.hamburger');
            
            sidebar.classList.remove('open');
            overlay.classList.remove('active');
            hamburger.classList.remove('active');
        }

        // Carousel functionality
        function changeSlide(carouselIndex, direction) {
            const carousel = carouselData[carouselIndex];
            const totalImages = carousel.images.length;
            
            carousel.currentIndex += direction;
            
            if (carousel.currentIndex >= totalImages) {
                carousel.currentIndex = 0;
            } else if (carousel.currentIndex < 0) {
                carousel.currentIndex = totalImages - 1;
            }
            
            updateCarousel(carouselIndex);
        }

        function goToSlide(carouselIndex, slideIndex) {
            carouselData[carouselIndex].currentIndex = slideIndex;
            updateCarousel(carouselIndex);
        }

        function updateCarousel(carouselIndex) {
            const carousel = carouselData[carouselIndex];
            const imageElement = document.getElementById(`carousel-${carouselIndex}`);
            const dotsContainer = document.getElementById(`dots-${carouselIndex}`);
            
            // Update image
            imageElement.src = carousel.images[carousel.currentIndex];
            
            // Update dots
            dotsContainer.innerHTML = '';
            carousel.images.forEach((_, index) => {
                const dot = document.createElement('span');
                dot.className = `dot ${index === carousel.currentIndex ? 'active' : ''}`;
                dot.onclick = () => goToSlide(carouselIndex, index);
                dotsContainer.appendChild(dot);
            });
        }

        // Auto-play carousels
        function autoPlayCarousels() {
            carouselData.forEach((_, index) => {
                changeSlide(index, 1);
            });
        }

        // Initialize carousels
        function initializeCarousels() {
            carouselData.forEach((_, index) => {
                updateCarousel(index);
            });
        }

        // Smooth scrolling for navigation links
        function initializeSmoothScroll() {
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
        }

        // Loading animation
        function initializeLoadingAnimation() {
            const observer = new IntersectionObserver((entries) => {
                entries.forEach(entry => {
                    if (entry.isIntersecting) {
                        entry.target.classList.add('loaded');
                    }
                });
           });

            document.querySelectorAll('.loading').forEach(el => {
                observer.observe(el);
            });
        }

        // Initialize everything when DOM is loaded
        document.addEventListener('DOMContentLoaded', function() {
            initializeCarousels();
            initializeSmoothScroll();
            initializeLoadingAnimation();
            
            // Auto-play carousels every 5 seconds
            setInterval(autoPlayCarousels, 5000);
        });

        // Close sidebar when clicking outside
        document.addEventListener('click', function(e) {
            const sidebar = document.getElementById('sidebar');
            const hamburger = document.querySelector('.hamburger');
            
            if (!sidebar.contains(e.target) && !hamburger.contains(e.target)) {
                closeSidebar();
            }
        });
    </script>
</body>
</htm
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
