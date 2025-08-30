<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Ayush Yadav R2 - 120 Days Transformation Journey</title>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    <link href="https://fonts.googleapis.com/css2?family=Poppins:wght@300;400;500;600;700&family=Montserrat:wght@700;800;900&display=swap" rel="stylesheet">
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: 'Poppins', 'Segoe UI', sans-serif;
        }
        
        :root {
            --primary: #2563EB;
            --secondary: #1E40AF;
            --accent: #F59E0B;
            --dark: #0F172A;
            --light: #F1F5F9;
            --gradient: linear-gradient(135deg, var(--primary), var(--secondary));
        }
        
        body {
            background-color: var(--dark);
            color: var(--light);
            line-height: 1.6;
            overflow-x: hidden;
        }
        
        .container {
            max-width: 1200px;
            margin: 0 auto;
            padding: 20px;
        }
        
        header {
            display: flex;
            justify-content: space-between;
            align-items: center;
            padding: 20px 0;
            border-bottom: 1px solid rgba(255, 255, 255, 0.1);
        }
        
        .logo-container {
            display: flex;
            align-items: center;
            gap: 15px;
        }
        
        .logo {
            width: 60px;
            height: 60px;
            display: flex;
            align-items: center;
            justify-content: center;
            border-radius: 12px;
            background: var(--gradient);
            color: white;
            font-weight: bold;
            font-size: 22px;
            box-shadow: 0 4px 15px rgba(37, 99, 235, 0.3);
        }
        
        .logo-text {
            display: flex;
            flex-direction: column;
        }
        
        .logo-text .main {
            font-size: 1.8rem;
            font-weight: 700;
            background: var(--gradient);
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
        }
        
        .logo-text .sub {
            font-size: 0.9rem;
            opacity: 0.8;
            letter-spacing: 2px;
        }
        
        nav ul {
            display: flex;
            list-style: none;
            gap: 30px;
        }
        
        nav a {
            color: white;
            text-decoration: none;
            font-weight: 500;
            transition: color 0.3s ease;
            position: relative;
        }
        
        nav a:hover {
            color: var(--primary);
        }
        
        nav a::after {
            content: '';
            position: absolute;
            bottom: -5px;
            left: 0;
            width: 0;
            height: 2px;
            background: var(--primary);
            transition: width 0.3s ease;
        }
        
        nav a:hover::after {
            width: 100%;
        }
        
        .hero {
            display: flex;
            flex-direction: column;
            align-items: center;
            text-align: center;
            padding: 80px 0 50px;
        }
        
        .hero h1 {
            font-size: 3.5rem;
            margin-bottom: 20px;
            font-family: 'Montserrat', sans-serif;
            background: linear-gradient(to right, var(--primary), var(--accent));
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
        }
        
        .hero p {
            font-size: 1.2rem;
            max-width: 700px;
            margin-bottom: 40px;
            opacity: 0.9;
        }
        
        .cta-buttons {
            display: flex;
            gap: 20px;
            margin-bottom: 50px;
            flex-wrap: wrap;
            justify-content: center;
        }
        
        .btn {
            padding: 15px 30px;
            border-radius: 50px;
            text-decoration: none;
            font-weight: 600;
            display: flex;
            align-items: center;
            gap: 10px;
            transition: all 0.3s ease;
        }
        
        .btn-primary {
            background: var(--gradient);
            color: white;
            box-shadow: 0 4px 15px rgba(37, 99, 235, 0.3);
        }
        
        .btn-primary:hover {
            transform: translateY(-3px);
            box-shadow: 0 8px 25px rgba(37, 99, 235, 0.5);
        }
        
        .btn-secondary {
            background: rgba(255, 255, 255, 0.1);
            backdrop-filter: blur(10px);
            color: white;
            border: 1px solid rgba(255, 255, 255, 0.2);
        }
        
        .btn-secondary:hover {
            background: rgba(255, 255, 255, 0.2);
            transform: translateY(-3px);
        }
        
        .social-links {
            display: flex;
            gap: 15px;
            flex-wrap: wrap;
            justify-content: center;
        }
        
        .social-icon {
            width: 50px;
            height: 50px;
            border-radius: 50%;
            display: flex;
            align-items: center;
            justify-content: center;
            background: rgba(255, 255, 255, 0.1);
            color: white;
            font-size: 1.2rem;
            transition: all 0.3s ease;
        }
        
        .social-icon:hover {
            transform: translateY(-5px);
            background: var(--gradient);
        }
        
        .section-title {
            text-align: center;
            margin: 60px 0 40px;
            font-size: 2.2rem;
            position: relative;
            padding-bottom: 15px;
            font-family: 'Montserrat', sans-serif;
        }
        
        .section-title::after {
            content: '';
            position: absolute;
            bottom: 0;
            left: 50%;
            transform: translateX(-50%);
            width: 80px;
            height: 4px;
            background: var(--gradient);
            border-radius: 2px;
        }
        
        .features {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 25px;
            margin-bottom: 60px;
        }
        
        .feature-card {
            background: rgba(255, 255, 255, 0.05);
            border-radius: 15px;
            padding: 30px;
            text-align: center;
            transition: transform 0.3s ease, box-shadow 0.3s ease;
            box-shadow: 0 5px 15px rgba(0, 0, 0, 0.1);
            backdrop-filter: blur(10px);
            border: 1px solid rgba(255, 255, 255, 0.1);
        }
        
        .feature-card:hover {
            transform: translateY(-10px);
            box-shadow: 0 15px 30px rgba(0, 0, 0, 0.2);
        }
        
        .feature-icon {
            width: 70px;
            height: 70px;
            border-radius: 50%;
            display: flex;
            align-items: center;
            justify-content: center;
            margin: 0 auto 20px;
            background: var(--gradient);
            font-size: 1.8rem;
        }
        
        .feature-card h3 {
            font-size: 1.4rem;
            margin-bottom: 15px;
            color: var(--accent);
        }
        
        .about-section {
            background: rgba(255, 255, 255, 0.05);
            border-radius: 15px;
            padding: 40px;
            margin-bottom: 60px;
            box-shadow: 0 5px 15px rgba(0, 0, 0, 0.1);
            backdrop-filter: blur(10px);
            border: 1px solid rgba(255, 255, 255, 0.1);
        }
        
        .about-section h2 {
            color: var(--accent);
            margin-bottom: 20px;
            text-align: center;
        }
        
        .about-section p {
            margin-bottom: 15px;
            line-height: 1.8;
        }
        
        .videos-container {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(320px, 1fr));
            gap: 25px;
            margin-bottom: 60px;
        }
        
        .video-card {
            background: rgba(255, 255, 255, 0.05);
            border-radius: 15px;
            overflow: hidden;
            transition: transform 0.3s ease, box-shadow 0.3s ease;
            box-shadow: 0 5px 15px rgba(0, 0, 0, 0.1);
            backdrop-filter: blur(10px);
            border: 1px solid rgba(255, 255, 255, 0.1);
        }
        
        .video-card:hover {
            transform: translateY(-10px);
            box-shadow: 0 15px 30px rgba(0, 0, 0, 0.2);
        }
        
        .video-thumb {
            width: 100%;
            height: 180px;
            background: #1a1a2e;
            display: flex;
            align-items: center;
            justify-content: center;
            font-size: 50px;
            color: var(--primary);
            position: relative;
            overflow: hidden;
        }
        
        .video-thumb::before {
            content: '';
            position: absolute;
            width: 100%;
            height: 100%;
            background: linear-gradient(45deg, rgba(37, 99, 235, 0.2), rgba(59, 130, 246, 0.2));
        }
        
        .video-info {
            padding: 20px;
        }
        
        .video-title {
            font-size: 1.2rem;
            margin-bottom: 10px;
            font-weight: 600;
        }
        
        .watch-btn {
            display: inline-flex;
            align-items: center;
            gap: 8px;
            padding: 8px 18px;
            background: var(--primary);
            color: white;
            border-radius: 5px;
            text-decoration: none;
            font-weight: 500;
            transition: background 0.3s ease;
        }
        
        .watch-btn:hover {
            background: var(--secondary);
        }
        
        .contact-section {
            background: rgba(255, 255, 255, 0.05);
            border-radius: 15px;
            padding: 40px;
            text-align: center;
            margin-bottom: 60px;
            box-shadow: 0 5px 15px rgba(0, 0, 0, 0.1);
            backdrop-filter: blur(10px);
            border: 1px solid rgba(255, 255, 255, 0.1);
        }
        
        .contact-title {
            font-size: 1.8rem;
            margin-bottom: 20px;
        }
        
        .contact-email {
            display: inline-flex;
            align-items: center;
            gap: 10px;
            padding: 15px 30px;
            background: rgba(255, 255, 255, 0.1);
            border-radius: 50px;
            font-size: 1.2rem;
            text-decoration: none;
            color: white;
            transition: all 0.3s ease;
            border: 1px solid rgba(255, 255, 255, 0.2);
        }
        
        .contact-email:hover {
            background: rgba(255, 255, 255, 0.2);
            transform: scale(1.05);
        }
        
        .contact-buttons {
            display: flex;
            gap: 15px;
            justify-content: center;
            flex-wrap: wrap;
            margin-top: 20px;
        }
        
        .contact-btn {
            display: inline-flex;
            align-items: center;
            gap: 8px;
            padding: 12px 25px;
            background: var(--primary);
            color: white;
            border-radius: 50px;
            text-decoration: none;
            font-weight: 500;
            transition: all 0.3s ease;
        }
        
        .contact-btn:hover {
            background: var(--secondary);
            transform: translateY(-3px);
        }
        
        footer {
            text-align: center;
            padding: 30px;
            border-top: 1px solid rgba(255, 255, 255, 0.1);
            margin-top: 30px;
            font-size: 0.9rem;
            opacity: 0.7;
        }
        
        @media (max-width: 768px) {
            header {
                flex-direction: column;
                gap: 20px;
            }
            
            nav ul {
                gap: 15px;
                flex-wrap: wrap;
                justify-content: center;
            }
            
            .hero h1 {
                font-size: 2.5rem;
            }
            
            .cta-buttons {
                flex-direction: column;
            }
            
            .features, .videos-container {
                grid-template-columns: 1fr;
            }
            
            .contact-buttons {
                flex-direction: column;
                align-items: center;
            }
        }
    </style>
</head>
<body>
    <div class="container">
        <header>
            <div class="logo-container">
                <div class="logo">AY</div>
                <div class="logo-text">
                    <span class="main">AyushYadav R2</span>
                    <span class="sub">120 DAYS TRANSFORMATION</span>
                </div>
            </div>
            
            <nav>
                <ul>
                    <li><a href="#about">About</a></li>
                    <li><a href="#features">Features</a></li>
                    <li><a href="#videos">Videos</a></li>
                    <li><a href="#contact">Contact</a></li>
                </ul>
            </nav>
        </header>
        
        <section class="hero">
            <h1>Transform Your Life in 120 Days</h1>
            <p>Welcome to Ayush Yadav R2's 120 Days Self-Life Transformation Series. Get daily motivation, mindset building tips, and powerful thoughts that will push you closer to your goals.</p>
            
            <div class="cta-buttons">
                <a href="https://youtube.com/@ayushyadav-r2?si=JmwCoDSOr724spT8" class="btn btn-primary" target="_blank">
                    <i class="fab fa-youtube"></i> YouTube Channel
                </a>
                <a href="#videos" class="btn btn-secondary">
                    <i class="fas fa-play-circle"></i> Watch Videos
                </a>
            </div>
            
            <div class="social-links">
                <a href="https://youtube.com/@ayushyadav-r2?si=JmwCoDSOr724spT8" class="social-icon" target="_blank">
                    <i class="fab fa-youtube"></i>
                </a>
                <a href="https://www.instagram.com/ayushyadavr2?igsh=MTlzYm9pYmRid3hjbw==" class="social-icon" target="_blank">
                    <i class="fab fa-instagram"></i>
                </a>
                <a href="mailto:ayushyadav47633@gmail.com" class="social-icon">
                    <i class="fas fa-envelope"></i>
                </a>
            </div>
        </section>
        
        <section id="about" class="about-section">
            <h2>Welcome to Ayush Yadav R2 App</h2>
            <p>This app is your companion for the 120 Days Self-Life Transformation Series created by Ayush Yadav. Every day you'll get motivation, mindset building tips, skill development hacks, and powerful thoughts that will push you closer to your goals.</p>
            
            <p>🌟 What you get inside:</p>
            <p>🎥 Direct access to daily YouTube Shorts</p>
            <p>📚 Mindset, productivity & self-growth lessons</p>
            <p>💪 Health & fitness motivation</p>
            <p>📈 Skill development ideas for students & creators</p>
            <p>🔔 Never miss a video – instant reminders</p>
            
            <p>This app is for those who want to stop wasting time and build a sharp mind, healthy body, and a successful future.</p>
            
            <p>👉 Follow the journey now and see the transformation in your own life.</p>
            
            <p>Made with ❤️ by Ayush Yadav (R2).</p>
        </section>
        
        <h2 class="section-title" id="features">What You Get Inside</h2>
        
        <div class="features">
            <div class="feature-card">
                <div class="feature-icon">
                    <i class="fas fa-film"></i>
                </div>
                <h3>Daily YouTube Shorts</h3>
                <p>Direct access to daily motivation and transformation content in short, digestible videos.</p>
            </div>
            
            <div class="feature-card">
                <div class="feature-icon">
                    <i class="fas fa-brain"></i>
                </div>
                <h3>Mindset Lessons</h3>
                <p>Powerful mindset building tips and productivity hacks to reprogram your thinking.</p>
            </div>
            
            <div class="feature-card">
                <div class="feature-icon">
                    <i class="fas fa-dumbbell"></i>
                </div>
                <h3>Fitness Motivation</h3>
                <p>Health & fitness guidance to transform your body and boost your energy levels.</p>
            </div>
            
            <div class="feature-card">
                <div class="feature-icon">
                    <i class="fas fa-laptop-code"></i>
                </div>
                <h3>Skill Development</h3>
                <p>Learn valuable skills for personal and professional growth as a student or creator.</p>
            </div>
        </div>
        
        <h2 class="section-title" id="videos">Popular Videos</h2>
        
        <div class="videos-container">
            <div class="video-card">
                <div class="video-thumb">
                    <i class="fas fa-play-circle"></i>
                </div>
                <div class="video-info">
                    <h3 class="video-title">How to Do Mental Reprogramming</h3>
                    <a href="#" class="watch-btn">
                        <i class="fas fa-play"></i> Watch Now
                    </a>
                </div>
            </div>
            
            <div class="video-card">
                <div class="video-thumb">
                    <i class="fas fa-play-circle"></i>
                </div>
                <div class="video-info">
                    <h3 class="video-title">Building Self-Discipline</h3>
                    <a href="#" class="watch-btn">
                        <i class="fas fa-play"></i> Watch Now
                    </a>
                </div>
            </div>
            
            <div class="video-card">
                <div class="video-thumb">
                    <i class="fas fa-play-circle"></i>
                </div>
                <div class="video-info">
                    <h3 class="video-title">Time Management Secrets</h3>
                    <a href="#" class="watch-btn">
                        <i class="fas fa-play"></i> Watch Now
                    </a>
                </div>
            </div>
        </div>
        
        <section id="contact" class="contact-section">
            <h2 class="contact-title">Get in Touch</h2>
            <a href="mailto:ayushyadav47633@gmail.com" class="contact-email">
                <i class="fas fa-envelope"></i> ayushyadav47633@gmail.com
            </a>
            
            <div class="contact-buttons">
                <a href="https://www.instagram.com/ayushyadavr2?igsh=MTlzYm9pYmRid3hjbw==" class="contact-btn" target="_blank">
                    <i class="fab fa-instagram"></i> Instagram
                </a>
                <a href="https://youtube.com/@ayushyadav-r2?si=JmwCoDSOr724spT8" class="contact-btn" target="_blank">
                    <i class="fab fa-youtube"></i> YouTube
                </a>
                <a href="mailto:ayushyadav47633@gmail.com" class="contact-btn">
                    <i class="fas fa-envelope"></i> Email
                </a>
            </div>
        </section>
    </div>
    
    <footer>
        <p>Made with ❤️ by Ayush Yadav (R2) | © 2023 AyushYadav R2. All Rights Reserved.</p>
    </footer>

    <script>
        // Simple animation for page elements
        document.addEventListener('DOMContentLoaded', function() {
            const elements = document.querySelectorAll('.feature-card, .video-card, .btn, .social-icon');
            
            elements.forEach(element => {
                element.style.opacity = 0;
                element.style.transform = 'translateY(20px)';
            });
            
            setTimeout(() => {
                elements.forEach((element, index) => {
                    setTimeout(() => {
                        element.style.transition = 'opacity 0.5s ease, transform 0.5s ease';
                        element.style.opacity = 1;
                        element.style.transform = 'translateY(0)';
                    }, 100 * index);
                });
            }, 300);
        });
    </script>
</body>
</html>
