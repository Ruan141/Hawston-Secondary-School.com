<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title> Hawston Secondary School - Excellence in Education</title>
    <style>
        /* Global Styles */
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: 'Arial', sans-serif;
        }
        
        body {
            line-height: 1.6;
            color: #333;
            background-color: #f9f9f9;
        }
        
        .container {
            width: 90%;
            max-width: 1200px;
            margin: 0 auto;
            padding: 0 15px;
        }
        
        /* Header Styles */
        header {
            background-color: #2c3e50;
            color: white;
            padding: 20px 0;
            box-shadow: 0 2px 5px rgba(0,0,0,0.1);
        }
        
        .header-container {
            display: flex;
            justify-content: space-between;
            align-items: center;
        }
        
        .logo {
            display: flex;
            align-items: center;
        }
        
        .logo img {
            height: 60px;
            margin-right: 15px;
        }
        
        .logo-text h1 {
            font-size: 24px;
            margin-bottom: 5px;
        }
        
        .logo-text p {
            font-size: 14px;
            opacity: 0.8;
        }
        
        /* Navigation */
        nav ul {
            display: flex;
            list-style: none;
        }
        
        nav ul li {
            margin-left: 20px;
        }
        
        nav ul li a {
            color: white;
            text-decoration: none;
            font-weight: bold;
            transition: color 0.3s;
        }
        
        nav ul li a:hover {
            color: #3498db;
        }
        
        /* Hero Section */
        .hero {
            background-image: linear-gradient(rgba(0,0,0,0.6), rgba(0,0,0,0.6)), url('school-building.jpg');
            background-size: cover;
            background-position: center;
            color: white;
            text-align: center;
            padding: 100px 20px;
        }
        
        .hero h2 {
            font-size: 36px;
            margin-bottom: 20px;
        }
        
        .hero p {
            font-size: 18px;
            max-width: 700px;
            margin: 0 auto 30px;
        }
        
        .btn {
            display: inline-block;
            background-color: #3498db;
            color: white;
            padding: 12px 30px;
            border-radius: 5px;
            text-decoration: none;
            font-weight: bold;
            transition: background-color 0.3s;
        }
        
        .btn:hover {
            background-color: #2980b9;
        }
        
        /* Main Content */
        .main-content {
            padding: 50px 0;
        }
        
        .section-title {
            text-align: center;
            margin-bottom: 40px;
        }
        
        .section-title h2 {
            font-size: 32px;
            color: #2c3e50;
            position: relative;
            display: inline-block;
            padding-bottom: 10px;
        }
        
        .section-title h2::after {
            content: '';
            position: absolute;
            bottom: 0;
            left: 50%;
            transform: translateX(-50%);
            width: 80px;
            height: 3px;
            background-color: #3498db;
        }
        
        /* Features */
        .features {
            display: flex;
            flex-wrap: wrap;
            justify-content: space-between;
            margin-bottom: 50px;
        }
        
        .feature {
            flex-basis: 30%;
            background: white;
            padding: 25px;
            margin-bottom: 30px;
            border-radius: 5px;
            box-shadow: 0 3px 10px rgba(0,0,0,0.1);
            text-align: center;
        }
        
        .feature i {
            font-size: 40px;
            color: #3498db;
            margin-bottom: 15px;
        }
        
        .feature h3 {
            margin-bottom: 15px;
            color: #2c3e50;
        }
        
        /* News Section */
        .news {
            background-color: #ecf0f1;
            padding: 50px 0;
        }
        
        .news-container {
            display: flex;
            flex-wrap: wrap;
            justify-content: space-between;
        }
        
        .news-item {
            flex-basis: 48%;
            background: white;
            margin-bottom: 25px;
            border-radius: 5px;
            overflow: hidden;
            box-shadow: 0 3px 10px rgba(0,0,0,0.1);
        }
        
        .news-image {
            height: 200px;
            overflow: hidden;
        }
        
        .news-image img {
            width: 100%;
            height: 100%;
            object-fit: cover;
            transition: transform 0.5s;
        }
        
        .news-item:hover .news-image img {
            transform: scale(1.05);
        }
        
        .news-content {
            padding: 20px;
        }
        
        .news-date {
            color: #7f8c8d;
            font-size: 14px;
            margin-bottom: 10px;
        }
        
        .news-content h3 {
            margin-bottom: 10px;
            color: #2c3e50;
        }
        
        /* Footer */
        footer {
            background-color: #2c3e50;
            color: white;
            padding: 50px 0 20px;
        }
        
        .footer-container {
            display: flex;
            flex-wrap: wrap;
            justify-content: space-between;
        }
        
        .footer-section {
            flex-basis: 30%;
            margin-bottom: 30px;
        }
        
        .footer-section h3 {
            font-size: 20px;
            margin-bottom: 20px;
            position: relative;
            padding-bottom: 10px;
        }
        
        .footer-section h3::after {
            content: '';
            position: absolute;
            bottom: 0;
            left: 0;
            width: 50px;
            height: 2px;
            background-color: #3498db;
        }
        
        .footer-section p, .footer-section a {
            opacity: 0.8;
            margin-bottom: 10px;
            display: block;
            color: white;
            text-decoration: none;
        }
        
        .footer-section a:hover {
            opacity: 1;
            color: #3498db;
        }
        
        .social-icons a {
            display: inline-block;
            margin-right: 15px;
            font-size: 20px;
        }
        
        .copyright {
            text-align: center;
            padding-top: 20px;
            border-top: 1px solid rgba(255,255,255,0.1);
            margin-top: 20px;
        }
        
        /* Responsive Design */
        @media (max-width: 768px) {
            .header-container {
                flex-direction: column;
                text-align: center;
            }
            
            nav ul {
                margin-top: 20px;
                justify-content: center;
            }
            
            .feature {
                flex-basis: 100%;
            }
            
            .news-item {
                flex-basis: 100%;
            }
            
            .footer-section {
                flex-basis: 100%;
                text-align: center;
            }
            
            .footer-section h3::after {
                left: 50%;
                transform: translateX(-50%);
            }
        }
    </style>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/5.15.3/css/all.min.css">
</head>
<body>
    <!-- Header Section -->
    <header>
        <div class="container header-container">
            <div class="logo">
                <img src="school-logo.png" alt=" High School Logo">
                <div class="logo-text">
                    <h1>Hawston Secondary School</h1>
                    <p>Excellence in Education Since 1985</p>
                </div>
            </div>
            <nav>
                <ul>
                    <li><a href="#">Home</a></li>
                    <li><a href="#">About Us</a></li>
                    <li><a href="#">Academics</a></li>
                    <li><a href="#">Admissions</a></li>
                    <li><a href="#">Contact</a></li>
                </ul>
            </nav>
        </div>
    </header>

    <!-- Hero Section -->
    <section class="hero">
        <div class="container">
            <h2>Shaping Future Leaders</h2>
            <p>At Hawston Secondary School, we provide a nurturing environment that fosters academic excellence, character development, and lifelong learning.</p>
            <a href="#" class="btn">Learn More</a>
        </div>
    </section>

    <!-- Main Content -->
    <section class="main-content">
        <div class="container">
            <div class="section-title">
                <h2>Why Choose Hawston Secondary?</h2>
            </div>
            
            <div class="features">
                <div class="feature">
                    <i class="fas fa-graduation-cap"></i>
                    <h3>Academic Excellence</h3>
                    <p>Our students consistently achieve top results in national examinations with a 98% college acceptance rate.</p>
                </div>
                
                <div class="feature">
                    <i class="fas fa-users"></i>
                    <h3>Experienced Faculty</h3>
                    <p>Learn from passionate educators with an average of 15 years teaching experience in their fields.</p>
                </div>
                
                <div class="feature">
                    <i class="fas fa-futbol"></i>
                    <h3>Extracurricular Programs</h3>
                    <p>Over 30 clubs and sports teams to help students develop their talents and interests.</p>
                </div>
            </div>
        </div>
    </section>

    <!-- News Section -->
    <section class="news">
        <div class="container">
            <div class="section-title">
                <h2>Latest News & Events</h2>
            </div>
            
            <div class="news-container">
                <div class="news-item">
                    <div class="news-image">
                        <img src="science-fair.jpg" alt="Science Fair">
                    </div>
                    <div class="news-content">
                        <div class="news-date">June 15, 2023</div>
                        <h3>Annual Science Fair Winners Announced</h3>
                        <p>Congratulations to our students for their innovative projects at this year's science fair.</p>
                        <a href="#">Read More</a>
                    </div>
                </div>
                
                <div class="news-item">
                    <div class="news-image">
                        <img src="graduation.jpg" alt="Graduation">
                    </div>
                    <div class="news-content">
                        <div class="news-date">May 28, 2023</div>
                        <h3>Class of 2023 Graduation Ceremony</h3>
                        <p>We celebrated the achievements of 142 graduates at our annual commencement ceremony.</p>
                        <a href="#">Read More</a>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- Footer -->
    <footer>
        <div class="container">
            <div class="footer-container">
                <div class="footer-section">
                    <h3>Contact Us</h3>
                    <p><i class="fas fa-map-marker-alt"></i> 123 Education Ave, Springfield</p>
                    <p><i class="fas fa-phone"></i> (555) 123-4567</p>
                    <p><i class="fas fa-envelope"></i> info@greenwood.edu</p>
                </div>
                
                <div class="footer-section">
                    <h3>Quick Links</h3>
                    <a href="#">School Calendar</a>
                    <a href="#">Parent Portal</a>
                    <a href="#">Lunch Menu</a>
                    <a href="#">Employment</a>
                </div>
                
                <div class="footer-section">
                    <h3>Follow Us</h3>
                    <div class="social-icons">
                        <a href="#"><i class="fab fa-facebook"></i></a>
                        <a href="#"><i class="fab fa-twitter"></i></a>
                        <a href="#"><i class="fab fa-instagram"></i></a>
                        <a href="#"><i class="fab fa-youtube"></i></a>
                    </div>
                </div>
            </div>
            
            <div class="copyright">
                <p>&copy; 2025 Hawston Secondary School. All Rights Reserved.</p>
            </div>
        </div>
    </footer>
</body>
</html>