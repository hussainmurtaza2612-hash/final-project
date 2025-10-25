<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Safar e Makkah Madina - The Final Masterpiece</title>
    <link rel="stylesheet" href="css/style.css">

    <!-- Google Fonts & Font Awesome Icons -->
    <link rel="preconnect" href="https://fonts.googleapis.com">
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
    <link
        href="https://fonts.googleapis.com/css2?family=Amiri:wght@700&family=Poppins:wght@300;400;500;600;700&display=swap"
        rel="stylesheet">
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.5.1/css/all.min.css">

    <!-- =================================================================== -->
    <!-- ======================= CSS STARTS HERE =========================== -->
    <!-- =================================================================== -->
    <style>
        :root {
            --primary-color: #0d2c54;
            --secondary-color: #d4af37;
            --light-color: #ffffff;
            --background-light: #f8f9fa;
            --text-color: #495057;
            --heading-color: #0d2c54;
            --body-font: 'Poppins', sans-serif;
            --heading-font: 'Amiri', serif;
            --transition-speed: 0.5s ease;
            --border-radius: 12px;
            --shadow: 0 15px 40px rgba(0, 0, 0, 0.1);
        }

        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        html {
            scroll-behavior: smooth;
        }

        body {
            font-family: var(--body-font);
            color: var(--text-color);
            background-color: var(--light-color);
        }

        .container {
            max-width: 1200px;
            margin: 0 auto;
            padding: 0 15px;
        }

        h1,
        h2,
        h3,
        h4 {
            font-family: var(--heading-font);
            font-weight: 700;
            color: var(--heading-color);
        }

        section {
            padding: 100px 0;
            overflow: hidden;
        }

        .section-header {
            text-align: center;
            margin-bottom: 60px;
        }

        .section-title {
            font-size: 3rem;
        }

        .section-subtitle {
            font-size: 1.1rem;
            color: #6c757d;
            max-width: 600px;
            margin: 10px auto 0;
        }

        a {
            text-decoration: none;
            color: var(--primary-color);
        }

        img {
            max-width: 100%;
            display: block;
        }

        /* --- HEADER & NAVIGATION (PREMIUM FROM START) --- */
        .site-header {
            position: fixed;
            top: 0;
            left: 0;
            width: 100%;
            z-index: 1000;
            transition: var(--transition-speed);
        }

        .top-bar {
            background: #081f3a;
            color: rgba(255, 255, 255, 0.8);
            padding: 10px 0;
            font-size: 0.9rem;
            transition: var(--transition-speed);
            border-bottom: 1px solid rgba(212, 175, 55, 0.3);
        }

        .top-bar .container,
        .main-nav .container {
            display: flex;
            justify-content: space-between;
            align-items: center;
        }

        .auth-buttons a {
            color: var(--light-color);
            margin-left: 10px;
            font-weight: 500;
        }

        .main-nav {
            background: var(--primary-color);
            padding: 15px 0;
            box-shadow: 0 5px 20px rgba(255, 255, 255, 0.2);
        }

        .site-header.scrolled .main-nav {
            box-shadow: var(--shadow);
        }

        .logo img {
            height: 55px;
        }

        .nav-links {
            list-style: none;
            display: flex;
        }

        .nav-links li {
            margin: 0 20px;
        }

        .nav-links a {
            color: var(--light-color);
            font-weight: 500;
            padding-bottom: 5px;
            position: relative;
        }

        .nav-links a::after {
            content: '';
            position: absolute;
            bottom: 0;
            left: 0;
            width: 0;
            height: 2px;
            background: var(--secondary-color);
            transition: 0.4s ease;
        }

        .nav-links a:hover::after {
            width: 100%;
        }

        .mobile-menu-icon {
            display: none;
            background: none;
            border: none;
            font-size: 2rem;
            color: var(--light-color);
            cursor: pointer;
            z-index: 1002;
        }

        /* --- HERO SECTION (VIDEO FIX) --- */
        .hero-section {
            height: 100vh;
            position: relative;
            display: flex;
            align-items: center;
            justify-content: center;
            text-align: center;
            color: var(--light-color);
            padding: 0;
            margin-top: -125px;
            /* Adjust this value to match header height */
        }

        .video-background {
            position: absolute;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            z-index: -2;
            overflow: hidden;
        }

        #bg-video {
            width: 100%;
            height: 100%;
            object-fit: cover;
        }

        .hero-overlay {
            position: absolute;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            background: rgba(0, 0, 0, 0.6);
            z-index: -1;
        }

        .hero-content {
            position: relative;
            z-index: 1;
        }

        .hero-content h1 {
            font-size: 5rem;
        }

        .hero-content p {
            font-size: 1.5rem;
            margin: 20px 0 40px;
        }

        .btn-primary {
            background: var(--secondary-color);
            color: var(--primary-color);
            padding: 18px 40px;
            border-radius: 50px;
            font-weight: 700;
            transition: var(--transition-speed);
        }

        .btn-primary:hover {
            background: var(--light-color);
            transform: scale(1.05);
            box-shadow: 0 10px 20px rgba(255, 255, 255, 0.2);
        }

        /* --- ALL SECTIONS --- */
        .search-section {
            padding: 0;
        }

        .search-form {
            background: var(--light-color);
            display: grid;
            grid-template-columns: repeat(3, 1fr) auto;
            gap: 20px;
            padding: 30px;
            border-radius: var(--border-radius);
            box-shadow: 0 20px 50px rgba(0, 0, 0, 0.1);
            margin: -70px auto 0;
            position: relative;
            z-index: 10;
            max-width: 1000px;
        }

        .why-choose-us-section {
            background: var(--background-light);
        }

        .why-choose-us-grid {
            display: grid;
            grid-template-columns: repeat(4, 1fr);
            gap: 30px;
        }

        .feature-item {
            background: var(--light-color);
            padding: 30px;
            text-align: center;
            border-radius: var(--border-radius);
            box-shadow: var(--shadow);
        }

        .packages-section {
            background: var(--background-light);
        }

        .packages-grid {
            display: grid;
            grid-template-columns: repeat(3, 1fr);
            gap: 30px;
        }

        /* A4 SIZE PACKAGE CARD FIX */
        .package-card {
            background: var(--light-color);
            border-radius: var(--border-radius);
            overflow: hidden;
            box-shadow: var(--shadow);
            transition: var(--transition-speed);
            display: flex;
            flex-direction: column;
        }

        .package-card:hover {
            transform: translateY(-15px);
            box-shadow: 0 25px 50px rgba(0, 0, 0, 0.15);
        }

        .package-image-container {
            width: 100%;
            height: 350px;
            /* Fixed height for consistency */
            overflow: hidden;
        }

        .package-image-container img {
            width: 100%;
            height: 100%;
            object-fit: cover;
            /* Will cover the area, might crop slightly */
        }

        .package-content {
            padding: 25px;
            flex-grow: 1;
            display: flex;
            flex-direction: column;
        }

        .btn-book-now {
            margin-top: auto;
            /* Pushes button to the bottom */
        }

        .testimonials-section {
            background: var(--primary-color);
            color: var(--light-color);
        }

        .testimonials-section .section-title {
            color: var(--light-color);
        }

        .testimonials-grid {
            display: grid;
            grid-template-columns: 1fr 1fr;
            gap: 30px;
        }

        .testimonial-card {
            background: rgba(255, 255, 255, 0.1);
            padding: 30px;
            border-radius: var(--border-radius);
            border-left: 5px solid var(--secondary-color);
        }

        .testimonial-card p {
            font-style: italic;
        }

        .client-info {
            display: flex;
            align-items: center;
            margin-top: 20px;
        }

        .client-info img {
            width: 60px;
            height: 60px;
            border-radius: 50%;
            margin-right: 15px;
        }

        .partners-section {
            background: var(--background-light);
        }

        .partners-grid {
            display: flex;
            justify-content: space-around;
            align-items: center;
            flex-wrap: wrap;
            gap: 20px;
        }

        .partner-logo {
            transition: transform var(--transition-speed);
        }

        .partner-logo:hover {
            transform: scale(1.1);
        }

        .partner-logo img {
            height: 45px;
        }

        .cta-bar {
            background: var(--secondary-color);
            padding: 40px 0;
        }

        .cta-bar .container {
            display: flex;
            justify-content: space-between;
            align-items: center;
        }

        .cta-bar h3 {
            color: var(--primary-color);
        }

        /* --- FOOTER (VIP VERSION) --- */
        .site-footer {
            background: #081f3a;
            color: rgba(255, 255, 255, 0.7);
            padding: 80px 0 0;
        }

        .footer-grid {
            display: grid;
            grid-template-columns: 2fr 1fr 1.5fr 1.5fr;
            gap: 40px;
            text-align: left;
        }

        .footer-logo {
            height: 60px;
            margin-bottom: 20px;
        }

        .footer-widget h3 {
            color: var(--light-color);
            margin-bottom: 20px;
        }

        .footer-widget ul {
            list-style: none;
        }

        .footer-widget ul li {
            margin-bottom: 10px;
        }

        .footer-widget ul li a {
            color: rgba(255, 255, 255, 0.7);
            transition: var(--transition-speed);
        }

        .footer-widget ul li a:hover {
            color: var(--secondary-color);
            padding-left: 5px;
        }

        .map-container {
            border-radius: var(--border-radius);
            overflow: hidden;
            margin-top: 20px;
        }

        .footer-bottom {
            padding: 25px 0;
            margin-top: 60px;
            border-top: 1px solid rgba(255, 255, 255, 0.1);
            text-align: center;
        }

        /* --- WIDGETS --- */
        .whatsapp-flt-btn,
        .scroll-to-top {
            /* ALL PREVIOUS SOLID STYLES APPLY */
        }

        /* --- SCROLL ANIMATIONS --- */
        .hidden {
            opacity: 0;
            transform: translateY(100px);
            transition: opacity 0.8s ease, transform 0.8s ease;
        }

        .visible {
            opacity: 1;
            transform: translateY(0);
        }

        /* Add more staggered delays as needed */

        /* --- RESPONSIVE DESIGN --- */
        @media (max-width: 992px) {

            .search-form,
            .why-choose-us-grid,
            .packages-grid,
            .testimonials-grid,
            .footer-grid {
                grid-template-columns: 1fr 1fr;
            }

            .nav-links-container {
                position: fixed;
                top: 0;
                left: -100%;
                width: 100%;
                height: 100%;
                background: rgba(13, 44, 84, 0.98);
                backdrop-filter: blur(8px);
                display: flex;
                align-items: center;
                justify-content: center;
                transition: left var(--transition-speed);
                z-index: 1001;
            }

            .nav-links-container.active {
                left: 0;
            }

            .nav-links {
                flex-direction: column;
                text-align: center;
            }

            .nav-links li {
                margin: 30px 0;
            }

            .nav-links a {
                font-size: 2.5rem;
                color: var(--light-color);
            }

            .mobile-menu-icon {
                display: block;
            }
        }

        @media (max-width: 768px) {
            body {
                padding-top: 118px;
            }

            .hero-section {
                margin-top: -118px;
            }

            .search-form,
            .why-choose-us-grid,
            .packages-grid,
            .testimonials-grid,
            .footer-grid {
                grid-template-columns: 1fr;
            }
        }
    </style>
</head>

<body>

    <!-- =================================================================== -->
    <!-- ======================= HTML BODY STARTS HERE ======================= -->
    <!-- =================================================================== -->

    <header class="site-header" id="site-header">
        <div class="top-bar">
            <div class="container">
                <div class="contact-info"><span><i class="fas fa-phone-alt"></i> 0310-3212695</span><span><i
                            class="fas fa-envelope"></i> safar.e.makkahmadina@gmail.com</span></div>
                <div class="auth-buttons"><a href="#">Login</a> / <a href="#">Register</a></div>
            </div>
        </div>
        <nav class="main-nav">
            <div class="container">
                <a href="index.html" class="logo"><img src="images/logo.png" alt="Safar e Makkah Madina Logo"></a>
                <div class="nav-links-container">
                    <ul class="nav-links">
                        <li><a href="#home">Home</a></li>
                        <li><a href="#services">Services</a></li>
                        <li><a href="#packages">Packages</a></li>
                        <li><a href="#testimonials">Reviews</a></li>
                        <li><a href="#faq">FAQs</a></li>
                        <li><a href="#contact">Contact</a></li>
                    </ul>
                </div>
                <button class="mobile-menu-icon" id="mobile-menu-toggle">&#9776;</button>
            </div>
        </nav>
    </header>

    <main>
        <section style="margin-top: 8%;" id="home" class="hero-section">
            <div class="video-background"><video autoplay muted loop playsinline id="bg-video">
                    <source src="videos/makkah-video.mp4" type="video/mp4">
                </video></div>
            <div class="hero-overlay"></div>
            <div class="hero-content">
                <h1 style="color: white;" class="hidden">Your Sacred Journey, Our Devotion</h1>
                <p class="hidden">5-Star Hajj & Umrah services for a journey of a lifetime.</p>
                <a href="#packages" class="btn-primary hidden">Explore Packages</a>
            </div>
        </section>



        <!-- ======================= SEARCH BAR SECTION (NEW) ======================= -->
<section style="padding-top: 20vh;" class="search-section hidden">
    <div class="container">
        <form class="search-form">
            <div class="form-group">
                <i class="fas fa-search"></i>
                <select>
                    <option disabled selected>Looking for...</option>
                    <option>Umrah Package</option>
                    <option>Hajj Package</option>
                </select>
            </div>
            <div class="form-group">
                <i class="fas fa-map-marker-alt"></i>
                <select>
                    <option disabled selected>Departure City...</option>
                    <option>Karachi</option>
                    <option>Lahore</option>
                    <option>Islamabad</option>
                </select>
            </div>
            <div class="form-group">
                <i class="fas fa-calendar-alt"></i>
                <input type="month" placeholder="Select Month">
            </div>
            <button type="submit" class="btn-search">Search Now</button>
        </form>
    </div>
</section>



        <!-- ======================= PACKAGES SECTION (A4 SIZE FIX) ======================= -->
        <section id="packages" class="packages-section">
            <div class="container">
                <div class="section-header hidden">
                    <h2 class="section-title">Our Most Popular Umrah Packages</h2>
                    <p class="section-subtitle">Specially designed packages for your comfort and spiritual needs.</p>
                </div>
                <div class="packages-grid">
                    <!-- Package Card 1 -->
                    <div class="package-card hidden">
                        <div class="package-image-container">
                            <img src="images/package1.jpg" alt="A4 Flyer for Golden Package">
                        </div>
                        <div class="package-content">
                            <h3>15-Day Golden Package</h3>
                            <p class="package-price">Starting from <b>PKR 250,000</b></p>
                            <a href="#" class="btn-book-now">View Details & Itinerary</a>
                        </div>
                    </div>
                    <!-- Package Card 2 -->
                    <div class="package-card hidden">
                        <div class="package-image-container">
                            <img src="images/package2.jpg" alt="A4 Flyer for Family Package">
                        </div>
                        <div class="package-content">
                            <h3>21-Day Family Package</h3>
                            <p class="package-price">Starting from <b>PKR 210,000</b></p>
                            <a href="#" class="btn-book-now">View Details & Itinerary</a>
                        </div>
                    </div>
                    <!-- Package Card 3 -->
                    <div class="package-card hidden">
                        <div class="package-image-container">
                            <img src="images/package3.jpg" alt="A4 Flyer for Express Package">
                        </div>
                        <div class="package-content">
                            <h3>10-Day Express Package</h3>
                            <p class="package-price">Starting from <b>PKR 190,000</b></p>
                            <a href="#" class="btn-book-now">View Details & Itinerary</a>
                        </div>
                    </div>
                </div>
            </div>
        </section>



        <!-- ======================= WHY CHOOSE US SECTION (NEW) ======================= -->
        <section class="why-choose-us-section">
            <div class="container">
                <div class="section-header hidden">
                    <h2 class="section-title">Why Choose Us?</h2>
                    <p class="section-subtitle">We are committed to making your pilgrimage a memorable and blessed
                        experience.</p>
                </div>
                <div class="why-choose-us-grid">
                    <div class="feature-item hidden">
                        <div class="feature-icon"><i class="fas fa-star"></i></div>
                        <h3>5-Star Service</h3>
                        <p>From luxury hotels to dedicated support, we ensure a premium experience.</p>
                    </div>
                    <div class="feature-item hidden">
                        <div class="feature-icon"><i class="fas fa-handshake"></i></div>
                        <h3>Trusted & Experienced</h3>
                        <p>With over 15 years of experience, we are a name you can trust.</p>
                    </div>
                    <div class="feature-item hidden">
                        <div class="feature-icon"><i class="fas fa-tags"></i></div>
                        <h3>Best Price Guarantee</h3>
                        <p>We offer competitive prices without compromising on quality.</p>
                    </div>
                    <div class="feature-item hidden">
                        <div class="feature-icon"><i class="fas fa-headset"></i></div>
                        <h3>24/7 Support</h3>
                        <p>Our team is available round the clock to assist you at every step.</p>
                    </div>
                </div>
            </div>
        </section>

        <!-- ======================= TESTIMONIALS SECTION (NEW) ======================= -->
        <section id="testimonials" class="testimonials-section">
            <div class="container">
                <div class="section-header hidden">
                    <h2 class="section-title">What Our Pilgrims Say</h2>
                </div>
                <div class="testimonials-grid">
                    <div class="testimonial-card hidden">
                        <p>"An absolutely flawless experience. From the visa to the hotels, everything was handled
                            professionally. Highly recommended!"</p>
                        <div class="client-info">
                            <img src="images/client1.jpg" alt="Client 1">
                            <div class="client-details">
                                <h4>Syed Hussain Murtaza</h4>
                                <span>Lahore, Pakistan</span>
                            </div>
                        </div>
                    </div>
                    <div class="testimonial-card hidden">
                        <p>"Safar e Mahkah Madina made our family Umrah a dream come true. The support and care they
                            provided was exceptional."</p>
                        <div class="client-info">
                            <img src="images/client2.jpg" alt="Client 2">
                            <div class="client-details">
                                <h4>Syed Afzal Hussain Shah</h4>
                                <span>Karachi, Pakistan</span>
                            </div>
                        </div>
                    </div>
                </div>
            </div>
        </section>


        <!-- ======================= STATS COUNTER SECTION (NEW) ======================= -->
<section style="margin-top: 30vh;" class="stats-section">
    <div class="stats-overlay"></div>
    <div class="container">
        <div class="stats-grid">
            <div class="stat-item hidden">
                <i class="fas fa-users"></i>
                <h3 class="counter" data-target="10000">0</h3>
                <p>Happy Pilgrims</p>
            </div>
            <div class="stat-item hidden">
                <i class="fas fa-star"></i>
                <h3 class="counter" data-target="5">0</h3>
                <p>Star Rating</p>
            </div>
            <div class="stat-item hidden">
                <i class="fas fa-handshake"></i>
                <h3 class="counter" data-target="250">0</h3>
                <p>Global Partners</p>
            </div>
            <div class="stat-item hidden">
                <i class="fas fa-briefcase"></i>
                <h3 class="counter" data-target="15">0</h3>
                <p>Years of Experience</p>
            </div>
        </div>
    </div>
</section>

<!-- ======================= HAJJ PACKAGES SECTION (NEW) ======================= -->
<section class="packages-section" style="background: var(--light-color);">
    <div class="container">
        <div class="section-header hidden">
            <h2 class="section-title">Hajj 2026 Packages</h2>
            <p class="section-subtitle">Register your interest for the journey of a lifetime.</p>
        </div>
        <div class="packages-grid">
            <div class="package-card hidden">
                <div class="package-image-container"><img src="images/hajj1.jpg" alt="Hajj Package"></div>
                <div class="package-content"><h3>Executive Hajj Package</h3><a href="#" class="btn-book-now">View Details</a></div>
            </div>
            <div class="package-card hidden">
                <div class="package-image-container"><img src="images/hajj2.jpg" alt="Hajj Package"></div>
                <div class="package-content"><h3>Economy Hajj Package</h3><a href="#" class="btn-book-now">View Details</a></div>
            </div>
            <div class="package-card hidden">
                <div class="package-image-container"><img src="images/hajj3.jpg" alt="Hajj Package"></div>
                <div class="package-content"><h3>Short Hajj Package</h3><a href="#" class="btn-book-now">View Details</a></div>
            </div>
        </div>
    </div>
</section>

<!-- ======================= AIRLINES SECTION (NEW) ======================= -->
<section class="partners-section">
    <div class="container">
        <div class="section-header hidden">
            <h2 class="section-title">Most Popular Airlines For Umrah</h2>
        </div>
        <div class="partners-grid">
            <div class="partner-logo hidden"><img src="images/partner-saudi.png" alt="Saudi Airlines"></div>
            <div class="partner-logo hidden"><img src="images/partner-pia.png" alt="PIA"></div>
            <div class="partner-logo hidden"><img src="images/partner-airblue.png" alt="Air Blue"></div>
            <div class="partner-logo hidden"><img src="images/partner-serene.png" alt="Serene Air"></div>
            <div class="partner-logo hidden"><img src="images/partner-flynas.png" alt="Flynas"></div>
        </div>
    </div>
</section>

<!-- ======================= CALL TO ACTION BAR (NEW) ======================= -->
<section class="cta-bar hidden">
    <div class="container">
        <h3>Ready to Plan Your Blessed Journey?</h3>
        <a href="tel:03103212695" class="btn-primary">Call Us Now</a>
    </div>
</section>


    </main>

    <!-- ======================= FOOTER (VIP VERSION) ======================= -->
<footer id="contact" class="site-footer">
    <div class="container">
        <div class="footer-grid">
            <div class="footer-widget hidden">
                <img src="images/logo-white.png" class="footer-logo" alt="Footer Logo">
                <p>Pakistan's most trusted travel partner for a blessed pilgrimage to the holy cities of Makkah and Madina.</p>
                <div class="footer-social-links">
                    <a href="#"><i class="fab fa-facebook-f"></i></a>
                    <a href="#"><i class="fab fa-instagram"></i></a>
                    <a href="#"><i class="fab fa-whatsapp"></i></a>
                </div>
            </div>
            <div class="footer-widget hidden">
                <h3>Quick Links</h3>
                <ul>
                    <li><a href="#home">Home</a></li>
                    <li><a href="#services">Services</a></li>
                    <li><a href="#packages">Packages</a></li>
                    <li><a href="#gallery">Gallery</a></li>
                    <li><a href="#faq">FAQs</a></li>
                </ul>
            </div>
            <div class="footer-widget hidden">
                <h3>Contact Us</h3>
                <ul class="contact-list">
                    <li><i class="fas fa-map-marker-alt"></i><span>Your Office Address, City, Pakistan</span></li>
                    <li><i class="fas fa-phone"></i><span>0310-3212695 / 0300-9312695</span></li>
                    <li><i class="fas fa-envelope"></i><span>safar.e.makkahmadina@gmail.com</span></li>
                </ul>
            </div>
            <div class="footer-widget hidden">
                <h3>Our Location</h3>
                <div class="map-container">
                    <iframe src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d3401.832641029283!2d74.329379!3d31.502008!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x3919045a0b7f1e5b%3A0x1b8b2b9b7b6b1b5!2sLahore%2C%20Punjab%2C%20Pakistan!5e0!3m2!1sen!2s" width="100%" height="150" style="border:0;" allowfullscreen="" loading="lazy"></iframe>
                </div>
            </div>
        </div>
        <div class="footer-bottom">
            <p>&copy; 2025 Safar e Makkah Madina. All Rights Reserved.</p>
        </div>
    </div>
</footer>

    <a href="https://wa.me/923103212695" target="_blank" class="whatsapp-flt-btn"><i class="fab fa-whatsapp"></i></a>
    <button id="scroll-to-top" class="scroll-to-top"><i class="fas fa-arrow-up"></i></button>

    <!-- =================================================================== -->
    <!-- ==================== JAVASCRIPT STARTS HERE ======================= -->
    <!-- =================================================================== -->
    <script>
        document.addEventListener('DOMContentLoaded', function () {
            const header = document.getElementById('site-header');
            if (header) { window.addEventListener('scroll', () => { header.classList.toggle('scrolled', window.scrollY > 50); }); }
            const menuToggle = document.getElementById('mobile-menu-toggle');
            const navLinksContainer = document.querySelector('.nav-links-container');
            if (menuToggle && navLinksContainer) { menuToggle.addEventListener('click', () => { navLinksContainer.classList.toggle('active'); menuToggle.innerHTML = navLinksContainer.classList.contains('active') ? '&times;' : '&#9776;'; }); }
            const scrollTopBtn = document.getElementById('scroll-to-top');
            if (scrollTopBtn) { window.addEventListener('scroll', () => { scrollTopBtn.classList.toggle('active', window.scrollY > 400); }); scrollTopBtn.addEventListener('click', () => { window.scrollTo({ top: 0, behavior: 'smooth' }); }); }
            const observer = new IntersectionObserver((entries) => { entries.forEach((entry) => { if (entry.isIntersecting) { entry.target.classList.add('visible'); } }); }, { threshold: 0.1 });
            const hiddenElements = document.querySelectorAll('.hidden');
            hiddenElements.forEach((el) => observer.observe(el));
        });
    </script>

</body>

</html>
