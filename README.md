# mhumaylm.github.io
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Lovitranix | Get Your Business on Google Search & Maps</title>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    <link href="https://fonts.googleapis.com/css2?family=Poppins:wght@300;400;500;600;700&display=swap" rel="stylesheet">
    <style>
        /* Base Styles */
        :root {
            --primary: #4285F4;
            --primary-dark: #3367D6;
            --primary-light: #8AB4F8;
            --secondary: #34A853;
            --secondary-dark: #2E8B47;
            --accent: #FBBC05;
            --accent-dark: #F29900;
            --light: #F8F9FA;
            --dark: #202124;
            --gray: #5F6368;
            --gray-light: #E8EAED;
            --transition: all 0.3s ease;
            --shadow: 0 5px 15px rgba(0, 0, 0, 0.08);
            --shadow-hover: 0 15px 30px rgba(0, 0, 0, 0.15);
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
            font-family: 'Poppins', sans-serif;
            line-height: 1.6;
            color: var(--dark);
            background-color: white;
            overflow-x: hidden;
        }

        .container {
            width: 90%;
            max-width: 1200px;
            margin: 0 auto;
            padding: 0 15px;
        }

        section {
            padding: 100px 0;
        }

        .btn {
            display: inline-flex;
            align-items: center;
            justify-content: center;
            padding: 14px 32px;
            background: var(--primary);
            color: white;
            border: none;
            border-radius: 8px;
            font-size: 1rem;
            font-weight: 600;
            cursor: pointer;
            transition: var(--transition);
            text-decoration: none;
            text-align: center;
            position: relative;
            overflow: hidden;
            z-index: 1;
        }

        .btn::before {
            content: '';
            position: absolute;
            top: 0;
            left: -100%;
            width: 100%;
            height: 100%;
            background: linear-gradient(90deg, transparent, rgba(255,255,255,0.2), transparent);
            transition: left 0.7s ease;
            z-index: -1;
        }

        .btn:hover::before {
            left: 100%;
        }

        .btn:hover {
            background: var(--primary-dark);
            transform: translateY(-3px);
            box-shadow: 0 10px 20px rgba(66, 133, 244, 0.3);
        }

        .btn-outline {
            background: transparent;
            border: 2px solid white;
            color: white;
        }

        .btn-outline:hover {
            background: white;
            color: var(--primary);
        }

        .btn-secondary {
            background: var(--secondary);
        }

        .btn-secondary:hover {
            background: var(--secondary-dark);
            box-shadow: 0 10px 20px rgba(52, 168, 83, 0.3);
        }

        .btn-accent {
            background: var(--accent);
            color: var(--dark);
        }

        .btn-accent:hover {
            background: var(--accent-dark);
            box-shadow: 0 10px 20px rgba(251, 188, 5, 0.3);
        }

        .section-title {
            text-align: center;
            margin-bottom: 60px;
        }

        .section-title h2 {
            font-size: 2.5rem;
            color: var(--dark);
            margin-bottom: 15px;
            position: relative;
            display: inline-block;
        }

        .section-title h2::after {
            content: '';
            position: absolute;
            bottom: -10px;
            left: 50%;
            transform: translateX(-50%);
            width: 80px;
            height: 4px;
            background: var(--primary);
            border-radius: 2px;
        }

        .section-title p {
            color: var(--gray);
            font-size: 1.1rem;
            max-width: 600px;
            margin: 0 auto;
        }

        /* Header Styles */
        header {
            background: white;
            box-shadow: 0 2px 20px rgba(0, 0, 0, 0.1);
            position: fixed;
            width: 100%;
            top: 0;
            z-index: 1000;
            transition: var(--transition);
        }

        header.scrolled {
            padding: 5px 0;
            box-shadow: 0 5px 20px rgba(0, 0, 0, 0.1);
        }

        .navbar {
            display: flex;
            justify-content: space-between;
            align-items: center;
            padding: 20px 0;
            transition: var(--transition);
        }

        header.scrolled .navbar {
            padding: 10px 0;
        }

        .logo {
            font-size: 1.8rem;
            font-weight: 700;
            color: var(--primary);
            text-decoration: none;
            display: flex;
            align-items: center;
        }

        .logo i {
            margin-right: 8px;
            font-size: 1.5rem;
        }

        .nav-links {
            display: flex;
            list-style: none;
        }

        .nav-links li {
            margin-left: 30px;
        }

        .nav-links a {
            text-decoration: none;
            color: var(--dark);
            font-weight: 500;
            transition: var(--transition);
            position: relative;
        }

        .nav-links a::after {
            content: '';
            position: absolute;
            bottom: -5px;
            left: 0;
            width: 0;
            height: 2px;
            background: var(--primary);
            transition: var(--transition);
        }

        .nav-links a:hover::after {
            width: 100%;
        }

        .nav-links a:hover {
            color: var(--primary);
        }

        .hamburger {
            display: none;
            cursor: pointer;
            font-size: 1.5rem;
        }

        /* Hero Section */
        .hero {
            background: linear-gradient(135deg, #4285F4, #3367D6);
            color: white;
            padding: 180px 0 120px;
            text-align: center;
            position: relative;
            overflow: hidden;
        }

        .hero::before {
            content: '';
            position: absolute;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            background: url('data:image/svg+xml,<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 1000 1000" opacity="0.05"><polygon fill="white" points="0,1000 1000,0 1000,1000"/></svg>');
            background-size: cover;
        }

        .hero-content {
            max-width: 900px;
            margin: 0 auto;
            position: relative;
            z-index: 1;
        }

        .hero h1 {
            font-size: 3.2rem;
            margin-bottom: 20px;
            line-height: 1.2;
            animation: fadeInUp 1s ease;
        }

        .hero p {
            font-size: 1.3rem;
            margin-bottom: 40px;
            opacity: 0.9;
            animation: fadeInUp 1s ease 0.2s both;
        }

        .hero-btns {
            display: flex;
            justify-content: center;
            gap: 20px;
            animation: fadeInUp 1s ease 0.4s both;
        }

        /* Services Section */
        .services {
            background: var(--light);
            position: relative;
        }

        .services::before {
            content: '';
            position: absolute;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            background: url('data:image/svg+xml,<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 1000 1000" opacity="0.03"><circle fill="%234285F4" cx="200" cy="200" r="150"/><circle fill="%2334A853" cx="800" cy="300" r="100"/><circle fill="%23FBBC05" cx="300" cy="700" r="120"/></svg>');
            background-size: cover;
        }

        .services-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(400px, 1fr));
            gap: 40px;
            margin-top: 50px;
            position: relative;
            z-index: 1;
        }

        .service-card {
            background: white;
            border-radius: 15px;
            padding: 50px 40px;
            box-shadow: var(--shadow);
            transition: var(--transition);
            text-align: center;
            position: relative;
            overflow: hidden;
            z-index: 1;
        }

        .service-card::before {
            content: '';
            position: absolute;
            top: 0;
            left: 0;
            width: 100%;
            height: 5px;
            background: var(--primary);
        }

        .service-card:nth-child(2)::before {
            background: var(--secondary);
        }

        .service-card::after {
            content: '';
            position: absolute;
            bottom: 0;
            right: 0;
            width: 100px;
            height: 100px;
            background: rgba(66, 133, 244, 0.05);
            border-radius: 50%;
            transform: translate(30%, 30%);
            z-index: -1;
        }

        .service-card:nth-child(2)::after {
            background: rgba(52, 168, 83, 0.05);
        }

        .service-card:hover {
            transform: translateY(-15px);
            box-shadow: var(--shadow-hover);
        }

        .service-icon {
            width: 90px;
            height: 90px;
            background: rgba(66, 133, 244, 0.1);
            border-radius: 50%;
            display: flex;
            align-items: center;
            justify-content: center;
            margin: 0 auto 30px;
            transition: var(--transition);
        }

        .service-card:hover .service-icon {
            transform: scale(1.1) rotate(5deg);
        }

        .service-card:nth-child(2) .service-icon {
            background: rgba(52, 168, 83, 0.1);
        }

        .service-icon i {
            font-size: 2.5rem;
            color: var(--primary);
        }

        .service-card:nth-child(2) .service-icon i {
            color: var(--secondary);
        }

        .service-card h3 {
            font-size: 1.8rem;
            margin-bottom: 20px;
            color: var(--dark);
        }

        .service-card p {
            color: var(--gray);
            margin-bottom: 30px;
            line-height: 1.7;
        }

        /* Stats Section */
        .stats {
            background: linear-gradient(135deg, var(--primary), var(--primary-dark));
            color: white;
            text-align: center;
            padding: 80px 0;
        }

        .stats-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(200px, 1fr));
            gap: 40px;
        }

        .stat-item {
            padding: 20px;
        }

        .stat-number {
            font-size: 3rem;
            font-weight: 700;
            margin-bottom: 10px;
            display: block;
        }

        .stat-text {
            font-size: 1.1rem;
            opacity: 0.9;
        }

        /* Process Section */
        .process {
            background: white;
        }

        .process-steps {
            display: flex;
            justify-content: space-between;
            position: relative;
            max-width: 900px;
            margin: 0 auto;
        }

        .process-steps::before {
            content: '';
            position: absolute;
            top: 40px;
            left: 0;
            width: 100%;
            height: 3px;
            background: var(--gray-light);
            z-index: 1;
        }

        .process-step {
            text-align: center;
            position: relative;
            z-index: 2;
            flex: 1;
        }

        .step-number {
            width: 80px;
            height: 80px;
            background: var(--primary);
            color: white;
            border-radius: 50%;
            display: flex;
            align-items: center;
            justify-content: center;
            font-size: 1.8rem;
            font-weight: 700;
            margin: 0 auto 20px;
            position: relative;
            transition: var(--transition);
        }

        .process-step:hover .step-number {
            transform: scale(1.1);
        }

        .process-step:nth-child(2) .step-number {
            background: var(--secondary);
        }

        .process-step:nth-child(3) .step-number {
            background: var(--accent);
        }

        .process-step:nth-child(4) .step-number {
            background: var(--primary-dark);
        }

        .step-content h3 {
            font-size: 1.3rem;
            margin-bottom: 10px;
            color: var(--dark);
        }

        .step-content p {
            color: var(--gray);
            font-size: 0.95rem;
        }

        /* CTA Section */
        .cta {
            background: linear-gradient(135deg, var(--secondary), var(--secondary-dark));
            color: white;
            text-align: center;
            padding: 100px 0;
            position: relative;
            overflow: hidden;
        }

        .cta::before {
            content: '';
            position: absolute;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            background: url('data:image/svg+xml,<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 1000 1000" opacity="0.05"><polygon fill="white" points="0,0 1000,1000 0,1000"/></svg>');
            background-size: cover;
        }

        .cta-content {
            max-width: 800px;
            margin: 0 auto;
            position: relative;
            z-index: 1;
        }

        .cta h2 {
            font-size: 2.8rem;
            margin-bottom: 20px;
        }

        .cta p {
            font-size: 1.3rem;
            max-width: 700px;
            margin: 0 auto 40px;
            opacity: 0.9;
        }

        /* Contact Section */
        .contact {
            background: var(--light);
            position: relative;
        }

        .contact-container {
            display: grid;
            grid-template-columns: 1fr 1fr;
            gap: 60px;
            align-items: center;
        }

        .contact-info h2 {
            font-size: 2.3rem;
            margin-bottom: 20px;
            color: var(--dark);
        }

        .contact-info p {
            color: var(--gray);
            margin-bottom: 30px;
            font-size: 1.1rem;
        }

        .contact-details {
            margin-top: 40px;
        }

        .contact-item {
            display: flex;
            align-items: center;
            margin-bottom: 20px;
        }

        .contact-item i {
            width: 50px;
            height: 50px;
            background: rgba(66, 133, 244, 0.1);
            border-radius: 50%;
            display: flex;
            align-items: center;
            justify-content: center;
            margin-right: 20px;
            color: var(--primary);
            font-size: 1.2rem;
            transition: var(--transition);
        }

        .contact-item:hover i {
            background: var(--primary);
            color: white;
            transform: scale(1.1);
        }

        .contact-form {
            background: white;
            padding: 50px;
            border-radius: 15px;
            box-shadow: var(--shadow);
            transition: var(--transition);
        }

        .contact-form:hover {
            box-shadow: var(--shadow-hover);
        }

        .form-group {
            margin-bottom: 25px;
        }

        .form-group label {
            display: block;
            margin-bottom: 10px;
            font-weight: 500;
            color: var(--dark);
        }

        .form-control {
            width: 100%;
            padding: 15px 20px;
            border: 1px solid var(--gray-light);
            border-radius: 8px;
            font-size: 1rem;
            transition: var(--transition);
            font-family: 'Poppins', sans-serif;
        }

        .form-control:focus {
            border-color: var(--primary);
            outline: none;
            box-shadow: 0 0 0 3px rgba(66, 133, 244, 0.2);
        }

        /* Footer */
        footer {
            background: var(--dark);
            color: white;
            padding: 60px 0 20px;
        }

        .footer-content {
            display: grid;
            grid-template-columns: 2fr 1fr 1fr;
            gap: 50px;
            margin-bottom: 40px;
        }

        .footer-column h3 {
            font-size: 1.3rem;
            margin-bottom: 25px;
            position: relative;
            padding-bottom: 10px;
        }

        .footer-column h3::after {
            content: '';
            position: absolute;
            bottom: 0;
            left: 0;
            width: 40px;
            height: 3px;
            background: var(--primary);
        }

        .footer-about p {
            margin-bottom: 20px;
            opacity: 0.8;
        }

        .footer-links {
            list-style: none;
        }

        .footer-links li {
            margin-bottom: 12px;
        }

        .footer-links a {
            color: white;
            text-decoration: none;
            opacity: 0.8;
            transition: var(--transition);
            display: flex;
            align-items: center;
        }

        .footer-links a i {
            margin-right: 8px;
            font-size: 0.8rem;
        }

        .footer-links a:hover {
            opacity: 1;
            padding-left: 5px;
        }

        .social-links {
            display: flex;
            gap: 15px;
            margin-top: 20px;
        }

        .social-links a {
            display: flex;
            align-items: center;
            justify-content: center;
            width: 40px;
            height: 40px;
            background: rgba(255, 255, 255, 0.1);
            border-radius: 50%;
            color: white;
            transition: var(--transition);
        }

        .social-links a:hover {
            background: var(--primary);
            transform: translateY(-5px);
        }

        .footer-bottom {
            text-align: center;
            padding-top: 30px;
            border-top: 1px solid rgba(255, 255, 255, 0.1);
            font-size: 0.9rem;
            opacity: 0.7;
        }

        /* Animations */
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

        @keyframes pulse {
            0% {
                transform: scale(1);
            }
            50% {
                transform: scale(1.05);
            }
            100% {
                transform: scale(1);
            }
        }

        .pulse {
            animation: pulse 2s infinite;
        }

        /* Responsive Styles */
        @media (max-width: 992px) {
            .hero h1 {
                font-size: 2.6rem;
            }
            
            .contact-container {
                grid-template-columns: 1fr;
                gap: 50px;
            }
            
            .footer-content {
                grid-template-columns: 1fr 1fr;
            }
            
            .process-steps {
                flex-direction: column;
                gap: 40px;
            }
            
            .process-steps::before {
                display: none;
            }
        }

        @media (max-width: 768px) {
            .navbar {
                padding: 15px 0;
            }
            
            .nav-links {
                position: fixed;
                top: 80px;
                left: -100%;
                width: 100%;
                flex-direction: column;
                background: white;
                text-align: center;
                box-shadow: 0 10px 10px rgba(0, 0, 0, 0.1);
                transition: var(--transition);
                padding: 30px 0;
            }
            
            .nav-links.active {
                left: 0;
            }
            
            .nav-links li {
                margin: 15px 0;
            }
            
            .hamburger {
                display: block;
            }
            
            .hero {
                padding: 140px 0 80px;
            }
            
            .hero h1 {
                font-size: 2.2rem;
            }
            
            .hero-btns {
                flex-direction: column;
                align-items: center;
            }
            
            .btn {
                width: 100%;
                max-width: 280px;
            }
            
            .services-grid {
                grid-template-columns: 1fr;
            }
            
            .section-title h2 {
                font-size: 2rem;
            }
            
            .footer-content {
                grid-template-columns: 1fr;
                gap: 40px;
            }
        }

        @media (max-width: 576px) {
            .hero h1 {
                font-size: 1.9rem;
            }
            
            .cta h2 {
                font-size: 2rem;
            }
            
            .contact-form {
                padding: 30px 25px;
            }
            
            .service-card {
                padding: 40px 25px;
            }
        }
    </style>
</head>
<body>
    <!-- Header -->
    <header id="header">
        <div class="container">
            <nav class="navbar">
                <a href="#" class="logo"><i class="fas fa-map-marked-alt"></i>Lovitranix</a>
                <ul class="nav-links">
                    <li><a href="#home">Home</a></li>
                    <li><a href="#services">Services</a></li>
                    <li><a href="#process">How It Works</a></li>
                    <li><a href="#contact">Contact</a></li>
                </ul>
                <a href="#contact" class="btn">CONTACT US!</a>
                <div class="hamburger">
                    <i class="fas fa-bars"></i>
                </div>
            </nav>
        </div>
    </header>

    <!-- Hero Section -->
    <section class="hero" id="home">
        <div class="container">
            <div class="hero-content">
                <h1>HELPING BUSINESSES GET ON GOOGLE SEARCH & MAPS</h1>
                <p>Increase your online visibility and reach more customers with our professional Google Business Profile services</p>
                <div class="hero-btns">
                    <a href="#services" class="btn btn-outline">Our Services</a>
                    <a href="#contact" class="btn btn-accent">Get Started Today</a>
                </div>
            </div>
        </div>
    </section>

    <!-- Services Section -->
    <section class="services" id="services">
        <div class="container">
            <div class="section-title">
                <h2>Our Services</h2>
                <p>We offer comprehensive solutions to get your business discovered on Google</p>
            </div>
            <div class="services-grid">
                <div class="service-card">
                    <div class="service-icon">
                        <i class="fas fa-map-marker-alt"></i>
                    </div>
                    <h3>Get Your Business On Google</h3>
                    <p>Put Your Business On The Map! We Help You List Your Company On Google Search And Google Maps So Customers Can Easily Find And Contact You Online. Get Verified And Grow Your Visibility Today.</p>
                    <a href="#contact" class="btn">LEARN MORE</a>
                </div>
                <div class="service-card">
                    <div class="service-icon">
                        <i class="fas fa-chart-line"></i>
                    </div>
                    <h3>Optimize Your Google Business Profile</h3>
                    <p>Boost Your Google Business Profile For Maximum Reach. We Enhance Your Listing With The Right Keywords, Photos, And Updates To Attract More Customers And Improve Your Local Search Ranking.</p>
                    <a href="#contact" class="btn btn-secondary">LEARN MORE!</a>
                </div>
            </div>
        </div>
    </section>

    <!-- Stats Section -->
    <section class="stats">
        <div class="container">
            <div class="stats-grid">
                <div class="stat-item">
                    <span class="stat-number" data-count="500">0</span>
                    <span class="stat-text">Businesses Listed</span>
                </div>
                <div class="stat-item">
                    <span class="stat-number" data-count="98">0</span>
                    <span class="stat-text">Success Rate</span>
                </div>
                <div class="stat-item">
                    <span class="stat-number" data-count="1200">0</span>
                    <span class="stat-text">Customers Reached</span>
                </div>
                <div class="stat-item">
                    <span class="stat-number" data-count="24">0</span>
                    <span class="stat-text">Hours Support</span>
                </div>
            </div>
        </div>
    </section>

    <!-- Process Section -->
    <section class="process" id="process">
        <div class="container">
            <div class="section-title">
                <h2>How It Works</h2>
                <p>Our simple 4-step process to get your business on Google</p>
            </div>
            <div class="process-steps">
                <div class="process-step">
                    <div class="step-number">1</div>
                    <div class="step-content">
                        <h3>Consultation</h3>
                        <p>We discuss your business goals and requirements</p>
                    </div>
                </div>
                <div class="process-step">
                    <div class="step-number">2</div>
                    <div class="step-content">
                        <h3>Setup</h3>
                        <p>We create and verify your Google Business Profile</p>
                    </div>
                </div>
                <div class="process-step">
                    <div class="step-number">3</div>
                    <div class="step-content">
                        <h3>Optimization</h3>
                        <p>We optimize your profile with keywords and images</p>
                    </div>
                </div>
                <div class="process-step">
                    <div class="step-number">4</div>
                    <div class="step-content">
                        <h3>Results</h3>
                        <p>You start appearing in more searches and get more customers</p>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- CTA Section -->
    <section class="cta">
        <div class="container">
            <div class="cta-content">
                <h2>Ready to Boost Your Online Presence?</h2>
                <p>Don't miss out on potential customers searching for your business on Google. Let us help you get listed and optimized today!</p>
                <a href="#contact" class="btn btn-accent pulse">GET STARTED NOW</a>
            </div>
        </div>
    </section>

    <!-- Contact Section -->
    <section class="contact" id="contact">
        <div class="container">
            <div class="contact-container">
                <div class="contact-info">
                    <h2>Get In Touch</h2>
                    <p>Contact us today to learn how we can help your business get discovered on Google Search and Maps. Our team is ready to answer your questions and get you started.</p>
                    
                    
                
                <!-- Updated Form with Formspree -->
                <div class="contact-form">
                    <form id="contactForm" action="https://formspree.io/f/xyznndad" method="POST">
                        <div class="form-group">
                            <label for="name">Your Name</label>
                            <input type="text" id="name" name="name" class="form-control" placeholder="Enter your name" required>
                        </div>
                        <div class="form-group">
                            <label for="email">Email Address</label>
                            <input type="email" id="email" name="email" class="form-control" placeholder="Enter your email" required>
                        </div>
                        <div class="form-group">
                            <label for="business">Business Name</label>
                            <input type="text" id="business" name="business" class="form-control" placeholder="Enter your business name">
                        </div>
                        <div class="form-group">
                            <label for="phone">Phone Number</label>
                            <input type="tel" id="phone" name="phone" class="form-control" placeholder="Enter your phone number">
                        </div>
                        <div class="form-group">
                            <label for="message">How Can We Help?</label>
                            <textarea id="message" name="message" class="form-control" rows="4" placeholder="Tell us about your business and goals"></textarea>
                        </div>
                        <button type="submit" class="btn" style="width: 100%;">SEND MESSAGE</button>
                    </form>
                </div>
            </div>
        </div>
    </section>

    <!-- Footer -->
    <footer>
        <div class="container">
            <div class="footer-content">
                <div class="footer-column footer-about">
                    <h3>About Lovitranix</h3>
                    <p>We specialize in helping businesses establish and optimize their presence on Google Search and Maps, increasing visibility and driving growth.</p>
                    
                </div>
                <div class="footer-column">
                    <h3>Quick Links</h3>
                    <ul class="footer-links">
                        <li><a href="#home"><i class="fas fa-chevron-right"></i>Home</a></li>
                        <li><a href="#services"><i class="fas fa-chevron-right"></i>Services</a></li>
                        <li><a href="#process"><i class="fas fa-chevron-right"></i>How It Works</a></li>
                        <li><a href="#contact"><i class="fas fa-chevron-right"></i>Contact</a></li>
                    </ul>
                </div>
                <div class="footer-column">
                    <h3>Services</h3>
                    <ul class="footer-links">
                        <li><a href="#"><i class="fas fa-chevron-right"></i>Google Business Listing</a></li>
                        <li><a href="#"><i class="fas fa-chevron-right"></i>Profile Optimization</a></li>
                        <li><a href="#"><i class="fas fa-chevron-right"></i>Local SEO</a></li>
                        <li><a href="#"><i class="fas fa-chevron-right"></i>Google Reviews Management</a></li>
                    </ul>
                </div>
            </div>
            <div class="footer-bottom">
                <p>Copyright - 2025 | Lovitranix</p>
            </div>
        </div>
    </footer>

    <script>
        // Mobile Navigation Toggle
        const hamburger = document.querySelector('.hamburger');
        const navLinks = document.querySelector('.nav-links');

        hamburger.addEventListener('click', () => {
            navLinks.classList.toggle('active');
        });

        // Close mobile menu when clicking on a link
        document.querySelectorAll('.nav-links a').forEach(link => {
            link.addEventListener('click', () => {
                navLinks.classList.remove('active');
            });
        });

        // Header scroll effect
        window.addEventListener('scroll', () => {
            const header = document.getElementById('header');
            if (window.scrollY > 50) {
                header.classList.add('scrolled');
            } else {
                header.classList.remove('scrolled');
            }
        });

        // Smooth scrolling for anchor links
        document.querySelectorAll('a[href^="#"]').forEach(anchor => {
            anchor.addEventListener('click', function(e) {
                e.preventDefault();
                
                const targetId = this.getAttribute('href');
                if(targetId === '#') return;
                
                const targetElement = document.querySelector(targetId);
                if(targetElement) {
                    window.scrollTo({
                        top: targetElement.offsetTop - 80,
                        behavior: 'smooth'
                    });
                }
            });
        });

        // Enhanced form submission with loading state
        document.getElementById('contactForm').addEventListener('submit', function(e) {
            e.preventDefault();
            
            const submitBtn = this.querySelector('button[type="submit"]');
            const originalText = submitBtn.textContent;
            
            // Show loading state
            submitBtn.textContent = 'SENDING...';
            submitBtn.disabled = true;
            
            // Prepare form data for Formspree
            const formData = new FormData(this);
            
            // Submit to Formspree using Fetch API
            fetch(this.action, {
                method: 'POST',
                body: formData,
                headers: {
                    'Accept': 'application/json'
                }
            })
            .then(response => {
                if (response.ok) {
                    // Success
                    alert('Thank you for your message! We will contact you soon.');
                    this.reset();
                } else {
                    // Error
                    response.json().then(data => {
                        if (data.errors) {
                            alert('Error: ' + data.errors.map(error => error.message).join(', '));
                        } else {
                            alert('Oops! There was a problem submitting your form. Please try again.');
                        }
                    });
                }
            })
            .catch(error => {
                alert('Oops! There was a problem submitting your form. Please try again.');
                console.error('Form submission error:', error);
            })
            .finally(() => {
                // Reset button state
                submitBtn.textContent = originalText;
                submitBtn.disabled = false;
            });
        });

        // Animated counter for stats
        const counters = document.querySelectorAll('.stat-number');
        const speed = 200;

        const animateCounter = () => {
            counters.forEach(counter => {
                const target = +counter.getAttribute('data-count');
                const count = +counter.innerText;
                
                if (count < target) {
                    counter.innerText = Math.ceil(count + (target / speed));
                    setTimeout(animateCounter, 1);
                } else {
                    counter.innerText = target;
                }
            });
        };

        // Start counter when stats section is in viewport
        const statsSection = document.querySelector('.stats');
        const observer = new IntersectionObserver((entries) => {
            entries.forEach(entry => {
                if (entry.isIntersecting) {
                    animateCounter();
                    observer.unobserve(entry.target);
                }
            });
        }, { threshold: 0.5 });

        observer.observe(statsSection);

        // Add animation to elements when they come into view
        const animateOnScroll = () => {
            const elements = document.querySelectorAll('.service-card, .process-step, .contact-form');
            
            elements.forEach(element => {
                const elementPosition = element.getBoundingClientRect().top;
                const screenPosition = window.innerHeight / 1.2;
                
                if (elementPosition < screenPosition) {
                    element.style.opacity = '1';
                    element.style.transform = 'translateY(0)';
                }
            });
        };

        // Set initial state for animated elements
        document.querySelectorAll('.service-card, .process-step, .contact-form').forEach(element => {
            element.style.opacity = '0';
            element.style.transform = 'translateY(30px)';
            element.style.transition = 'opacity 0.5s ease, transform 0.5s ease';
        });

        window.addEventListener('scroll', animateOnScroll);
        // Trigger once on load in case elements are already in view
        window.addEventListener('load', animateOnScroll);
    </script>
</body>
</html>
