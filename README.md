<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Ramakrishna Kodali - Senior Quality Engineer</title>
    <script src="https://cdn.tailwindcss.com"></script>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    <link href="https://fonts.googleapis.com/css2?family=Inter:wght@300;400;500;600;700;800&display=swap" rel="stylesheet">
    <link href="https://fonts.googleapis.com/css2?family=Playfair+Display:wght@400;700;900&display=swap" rel="stylesheet">
    <style>
        /* Professional Color Variables */
        :root {
            --primary-blue: #2563eb;
            --secondary-blue: #1e40af;
            --accent-gold: #f59e0b;
            --neutral-gray: #64748b;
            --light-gray: #f1f5f9;
            --dark-gray: #1e293b;
            --success-green: #10b981;
            --gradient-primary: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
            --gradient-secondary: linear-gradient(135deg, #2563eb 0%, #1e40af 100%);
            --gradient-accent: linear-gradient(135deg, #f59e0b 0%, #d97706 100%);
        }

        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        body {
            font-family: 'Inter', sans-serif;
            background: linear-gradient(135deg, #f8fafc 0%, #e2e8f0 100%);
            color: var(--dark-gray);
            scroll-behavior: smooth;
            line-height: 1.6;
        }

        /* Subtle Professional Background */
        .professional-background {
            position: fixed;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            z-index: -1;
            background: 
                radial-gradient(circle at 20% 20%, rgba(37, 99, 235, 0.03) 0%, transparent 50%),
                radial-gradient(circle at 80% 80%, rgba(245, 158, 11, 0.03) 0%, transparent 50%),
                linear-gradient(135deg, #f8fafc 0%, #e2e8f0 100%);
            animation: subtleShift 30s ease-in-out infinite;
        }

        @keyframes subtleShift {
            0%, 100% { background-position: 0% 0%, 100% 100%, 0% 0%; }
            50% { background-position: 100% 100%, 0% 0%, 100% 100%; }
        }

        /* Floating Professional Elements */
        .floating-elements {
            position: fixed;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            pointer-events: none;
            z-index: 1;
            opacity: 0.6;
        }

        .professional-particle {
            position: absolute;
            width: 2px;
            height: 2px;
            background: var(--primary-blue);
            border-radius: 50%;
            animation: professionalFloat 25s infinite linear;
            opacity: 0.4;
        }

        .professional-particle:nth-child(1) { left: 15%; animation-delay: 0s; }
        .professional-particle:nth-child(2) { left: 35%; animation-delay: 5s; }
        .professional-particle:nth-child(3) { left: 55%; animation-delay: 10s; }
        .professional-particle:nth-child(4) { left: 75%; animation-delay: 15s; }
        .professional-particle:nth-child(5) { left: 85%; animation-delay: 20s; }

        @keyframes professionalFloat {
            0% { transform: translateY(100vh) rotate(0deg); opacity: 0; }
            10% { opacity: 0.4; }
            90% { opacity: 0.4; }
            100% { transform: translateY(-100px) rotate(360deg); opacity: 0; }
        }

        /* Premium Glassmorphism */
        .glass-premium {
            background: rgba(255, 255, 255, 0.9);
            backdrop-filter: blur(20px) saturate(120%);
            border-radius: 24px;
            border: 1px solid rgba(255, 255, 255, 0.3);
            box-shadow: 
                0 20px 60px rgba(0, 0, 0, 0.08),
                0 8px 24px rgba(0, 0, 0, 0.04),
                inset 0 1px 0 rgba(255, 255, 255, 0.7);
            position: relative;
            overflow: hidden;
        }

        .glass-premium::before {
            content: '';
            position: absolute;
            top: 0;
            left: -100%;
            width: 100%;
            height: 100%;
            background: linear-gradient(90deg, transparent, rgba(37, 99, 235, 0.08), transparent);
            animation: premiumShimmer 4s infinite;
        }

        @keyframes premiumShimmer {
            0% { left: -100%; }
            100% { left: 100%; }
        }

        /* Professional Header */
        .professional-header {
            background: rgba(255, 255, 255, 0.95);
            backdrop-filter: blur(20px);
            border-bottom: 1px solid rgba(37, 99, 235, 0.1);
            box-shadow: 0 4px 24px rgba(0, 0, 0, 0.06);
            transition: all 0.3s ease;
        }

        .professional-header.scrolled {
            background: rgba(255, 255, 255, 0.98);
            box-shadow: 0 8px 40px rgba(0, 0, 0, 0.12);
        }

        .nav-link {
            position: relative;
            color: var(--neutral-gray);
            font-weight: 500;
            transition: all 0.3s ease;
            padding: 8px 16px;
            border-radius: 8px;
        }

        .nav-link:hover {
            color: var(--primary-blue);
            background: rgba(37, 99, 235, 0.05);
        }

        .nav-link::after {
            content: '';
            position: absolute;
            bottom: -2px;
            left: 50%;
            width: 0;
            height: 2px;
            background: var(--gradient-secondary);
            transform: translateX(-50%);
            transition: width 0.3s ease;
        }

        .nav-link:hover::after {
            width: 60%;
        }

        /* Hero Section Enhancement */
        .hero-container {
            min-height: 100vh;
            display: flex;
            align-items: center;
            justify-content: center;
            position: relative;
            padding: 80px 0;
        }

        .hero-content {
            text-align: center;
            animation: heroEntrance 1.2s ease-out forwards;
            opacity: 0;
            transform: translateY(40px);
        }

        @keyframes heroEntrance {
            to {
                opacity: 1;
                transform: translateY(0);
            }
        }

        .hero-title {
            font-family: 'Playfair Display', serif;
            font-size: clamp(2.5rem, 6vw, 4.5rem);
            font-weight: 700;
            background: var(--gradient-primary);
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
            background-clip: text;
            margin-bottom: 1.5rem;
            animation: titleReveal 1.5s ease-out 0.3s both;
        }

        @keyframes titleReveal {
            from {
                opacity: 0;
                transform: translateY(30px);
                background-position: 100% 0;
            }
            to {
                opacity: 1;
                transform: translateY(0);
                background-position: 0% 0;
            }
        }

        .hero-subtitle {
            font-size: clamp(1.2rem, 3vw, 1.8rem);
            color: var(--primary-blue);
            font-weight: 600;
            margin-bottom: 2rem;
            animation: subtitleReveal 1.5s ease-out 0.6s both;
        }

        @keyframes subtitleReveal {
            from {
                opacity: 0;
                transform: translateY(20px);
            }
            to {
                opacity: 1;
                transform: translateY(0);
            }
        }

        /* Professional CTA Button */
        .professional-cta {
            background: var(--gradient-secondary);
            color: white;
            padding: 16px 40px;
            font-size: 1.1rem;
            font-weight: 600;
            border-radius: 12px;
            border: none;
            cursor: pointer;
            position: relative;
            overflow: hidden;
            transition: all 0.3s cubic-bezier(0.4, 0, 0.2, 1);
            box-shadow: 
                0 8px 32px rgba(37, 99, 235, 0.3),
                0 4px 16px rgba(0, 0, 0, 0.1);
            animation: ctaReveal 1.5s ease-out 0.9s both;
        }

        .professional-cta::before {
            content: '';
            position: absolute;
            top: 0;
            left: -100%;
            width: 100%;
            height: 100%;
            background: linear-gradient(90deg, transparent, rgba(255, 255, 255, 0.2), transparent);
            transition: left 0.5s ease;
        }

        .professional-cta:hover::before {
            left: 100%;
        }

        .professional-cta:hover {
            transform: translateY(-3px) scale(1.02);
            box-shadow: 
                0 12px 48px rgba(37, 99, 235, 0.4),
                0 8px 24px rgba(0, 0, 0, 0.15);
        }

        @keyframes ctaReveal {
            from {
                opacity: 0;
                transform: translateY(20px);
            }
            to {
                opacity: 1;
                transform: translateY(0);
            }
        }

        /* Professional Cards */
        .professional-card {
            background: rgba(255, 255, 255, 0.9);
            backdrop-filter: blur(20px);
            border-radius: 20px;
            border: 1px solid rgba(255, 255, 255, 0.5);
            padding: 2rem;
            box-shadow: 
                0 16px 48px rgba(0, 0, 0, 0.06),
                0 8px 24px rgba(0, 0, 0, 0.04);
            transition: all 0.4s cubic-bezier(0.4, 0, 0.2, 1);
            position: relative;
            overflow: hidden;
        }

        .professional-card::before {
            content: '';
            position: absolute;
            top: 0;
            left: 0;
            right: 0;
            height: 4px;
            background: var(--gradient-primary);
            transform: scaleX(0);
            transition: transform 0.3s ease;
        }

        .professional-card:hover::before {
            transform: scaleX(1);
        }

        .professional-card:hover {
            transform: translateY(-8px);
            box-shadow: 
                0 24px 64px rgba(0, 0, 0, 0.1),
                0 12px 32px rgba(0, 0, 0, 0.06);
        }

        /* Timeline Enhancement */
        .professional-timeline {
            position: relative;
            padding: 4rem 0;
        }

        .timeline-line {
            position: absolute;
            left: 50%;
            transform: translateX(-50%);
            width: 4px;
            height: 100%;
            background: var(--gradient-primary);
            border-radius: 2px;
            box-shadow: 0 0 20px rgba(37, 99, 235, 0.3);
        }

        .timeline-item {
            position: relative;
            margin: 3rem 0;
            opacity: 0;
            transform: translateX(-50px);
            transition: all 0.8s cubic-bezier(0.4, 0, 0.2, 1);
        }

        .timeline-item.visible {
            opacity: 1;
            transform: translateX(0);
        }

        .timeline-item:nth-child(even) {
            transform: translateX(50px);
        }

        .timeline-item:nth-child(even).visible {
            transform: translateX(0);
        }

        .timeline-marker {
            position: absolute;
            top: 30px;
            left: 50%;
            transform: translateX(-50%);
            width: 20px;
            height: 20px;
            background: var(--gradient-secondary);
            border-radius: 50%;
            border: 4px solid white;
            box-shadow: 
                0 0 20px rgba(37, 99, 235, 0.4),
                0 4px 16px rgba(0, 0, 0, 0.1);
            z-index: 10;
            transition: all 0.3s ease;
        }

        .timeline-item:hover .timeline-marker {
            transform: translateX(-50%) scale(1.3);
            box-shadow: 
                0 0 30px rgba(37, 99, 235, 0.6),
                0 8px 24px rgba(0, 0, 0, 0.15);
        }

        /* Tools Grid */
        .tools-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(200px, 1fr));
            gap: 2rem;
            margin: 2rem 0;
        }

        .tool-card {
            background: rgba(255, 255, 255, 0.9);
            backdrop-filter: blur(15px);
            border-radius: 16px;
            padding: 2rem;
            text-align: center;
            border: 1px solid rgba(255, 255, 255, 0.5);
            box-shadow: 0 8px 32px rgba(0, 0, 0, 0.06);
            transition: all 0.4s cubic-bezier(0.4, 0, 0.2, 1);
            position: relative;
            overflow: hidden;
        }

        .tool-card::before {
            content: '';
            position: absolute;
            top: 0;
            left: 0;
            right: 0;
            bottom: 0;
            background: radial-gradient(circle at center, rgba(37, 99, 235, 0.05) 0%, transparent 70%);
            opacity: 0;
            transition: opacity 0.3s ease;
        }

        .tool-card:hover::before {
            opacity: 1;
        }

        .tool-card:hover {
            transform: translateY(-5px) scale(1.02);
            box-shadow: 0 16px 48px rgba(0, 0, 0, 0.1);
        }

        .tool-icon {
            font-size: 3rem;
            background: var(--gradient-primary);
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
            background-clip: text;
            margin-bottom: 1rem;
            transition: all 0.3s ease;
        }

        .tool-card:hover .tool-icon {
            transform: scale(1.1);
        }

        .tool-category {
            background: var(--gradient-accent);
            color: white;
            padding: 6px 16px;
            border-radius: 20px;
            font-size: 0.75rem;
            font-weight: 600;
            margin-bottom: 1rem;
            display: inline-block;
            box-shadow: 0 4px 16px rgba(245, 158, 11, 0.3);
        }

        /* Skills Enhancement */
        .skills-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(160px, 1fr));
            gap: 1rem;
            margin: 2rem 0;
        }

        .skill-badge {
            background: rgba(255, 255, 255, 0.9);
            border: 2px solid transparent;
            border-radius: 25px;
            padding: 12px 20px;
            text-align: center;
            font-weight: 600;
            color: var(--dark-gray);
            transition: all 0.3s cubic-bezier(0.4, 0, 0.2, 1);
            position: relative;
            overflow: hidden;
        }

        .skill-badge::before {
            content: '';
            position: absolute;
            top: 0;
            left: -100%;
            width: 100%;
            height: 100%;
            background: linear-gradient(90deg, transparent, rgba(37, 99, 235, 0.1), transparent);
            transition: left 0.5s ease;
        }

        .skill-badge:hover::before {
            left: 100%;
        }

        .skill-badge:hover {
            transform: translateY(-2px);
            border-color: var(--primary-blue);
            box-shadow: 0 8px 24px rgba(37, 99, 235, 0.2);
            color: var(--primary-blue);
        }

        /* Section Titles */
        .section-title {
            font-family: 'Playfair Display', serif;
            font-size: clamp(2rem, 5vw, 3rem);
            font-weight: 700;
            text-align: center;
            margin-bottom: 3rem;
            background: var(--gradient-primary);
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
            background-clip: text;
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
            background: var(--gradient-accent);
            border-radius: 2px;
        }

        /* Contact Enhancement */
        .contact-card {
            background: rgba(255, 255, 255, 0.9);
            backdrop-filter: blur(20px);
            border: 1px solid rgba(255, 255, 255, 0.5);
            border-radius: 16px;
            padding: 20px 30px;
            transition: all 0.3s cubic-bezier(0.4, 0, 0.2, 1);
            box-shadow: 0 8px 32px rgba(0, 0, 0, 0.06);
        }

        .contact-card:hover {
            transform: translateY(-3px);
            box-shadow: 0 16px 48px rgba(0, 0, 0, 0.1);
            border-color: var(--primary-blue);
        }

        /* Mobile Responsiveness */
        @media (max-width: 768px) {
            .tools-grid {
                grid-template-columns: repeat(auto-fit, minmax(150px, 1fr));
                gap: 1rem;
            }
            
            .timeline-line {
                left: 30px;
            }
            
            .timeline-item {
                margin-left: 60px;
                transform: translateX(-30px);
            }
            
            .timeline-item:nth-child(even) {
                transform: translateX(-30px);
            }
            
            .timeline-item.visible,
            .timeline-item:nth-child(even).visible {
                transform: translateX(0);
            }
            
            .timeline-marker {
                left: 30px;
            }
            
            .skills-grid {
                grid-template-columns: repeat(auto-fit, minmax(120px, 1fr));
            }
        }

        /* Scroll to Top */
        .scroll-to-top {
            position: fixed;
            bottom: 30px;
            right: 30px;
            background: var(--gradient-secondary);
            color: white;
            width: 50px;
            height: 50px;
            border-radius: 50%;
            display: none;
            align-items: center;
            justify-content: center;
            cursor: pointer;
            z-index: 1000;
            transition: all 0.3s cubic-bezier(0.4, 0, 0.2, 1);
            box-shadow: 0 8px 32px rgba(37, 99, 235, 0.3);
        }
        
        .scroll-to-top.show {
            display: flex;
        }
        
        .scroll-to-top:hover {
            transform: translateY(-3px) scale(1.1);
            box-shadow: 0 12px 40px rgba(37, 99, 235, 0.4);
        }

        /* Animation Classes */
        .fade-in-up {
            opacity: 0;
            transform: translateY(30px);
            transition: all 0.8s cubic-bezier(0.4, 0, 0.2, 1);
        }

        .fade-in-up.visible {
            opacity: 1;
            transform: translateY(0);
        }

        .stagger-1 { transition-delay: 0.1s; }
        .stagger-2 { transition-delay: 0.2s; }
        .stagger-3 { transition-delay: 0.3s; }
    </style>
</head>
<body>
    <!-- Professional Background -->
    <div class="professional-background"></div>

    <!-- Floating Elements -->
    <div class="floating-elements">
        <div class="professional-particle"></div>
        <div class="professional-particle"></div>
        <div class="professional-particle"></div>
        <div class="professional-particle"></div>
        <div class="professional-particle"></div>
    </div>

    <!-- Header & Navigation -->
    <header class="professional-header sticky top-0 z-50" id="header">
        <nav class="container mx-auto px-6 py-4 flex justify-between items-center">
            <a href="#" class="text-2xl font-bold" style="background: var(--gradient-primary); -webkit-background-clip: text; -webkit-text-fill-color: transparent;">RAMA KRISHNA</a>
            <div class="hidden md:flex space-x-2">
                <a href="#about" class="nav-link">About</a>
                <a href="#experience" class="nav-link">Experience</a>
                <a href="#projects" class="nav-link">Projects</a>
                <a href="#tools" class="nav-link">Tools</a>
                <a href="#skills" class="nav-link">Skills</a>
                <a href="#contact" class="nav-link">Contact</a>
            </div>
            <button id="mobile-menu-button" class="md:hidden p-2 rounded-lg hover:bg-gray-100">
                <i class="fas fa-bars text-xl"></i>
            </button>
        </nav>
        <!-- Mobile Menu -->
        <div id="mobile-menu" class="hidden md:hidden bg-white/95 backdrop-blur-sm border-t">
            <div class="container mx-auto px-6 py-4 space-y-2">
                <a href="#about" class="block nav-link">About</a>
                <a href="#experience" class="block nav-link">Experience</a>
                <a href="#projects" class="block nav-link">Projects</a>
                <a href="#tools" class="block nav-link">Tools</a>
                <a href="#skills" class="block nav-link">Skills</a>
                <a href="#contact" class="block nav-link">Contact</a>
            </div>
        </div>
    </header>

    <!-- Hero Section -->
    <main>
        <section id="hero" class="hero-container">
            <div class="container mx-auto px-6">
                <div class="glass-premium max-w-5xl mx-auto p-12 hero-content">
                    <h1 class="hero-title">Ramakrishna Kodali</h1>
                    <p class="hero-subtitle">Senior Quality Assurance Engineer</p>
                    <p class="max-w-3xl mx-auto text-neutral-gray mb-8 text-lg leading-relaxed">
                        A dedicated QA Engineer with over 4+ years of experience, passionate about ensuring product excellence through meticulous automated and manual testing, performance analysis, and effective team collaboration.
                    </p>
                    <button class="professional-cta" onclick="document.getElementById('contact').scrollIntoView({behavior: 'smooth'})">
                        <i class="fas fa-paper-plane mr-2"></i>
                        Connect With Me
                    </button>
                </div>
            </div>
        </section>

        <!-- About Section -->
        <section id="about" class="py-20">
            <div class="container mx-auto px-6">
                <div class="glass-premium max-w-4xl mx-auto p-12 fade-in-up">
                    <h2 class="section-title">About Me</h2>
                    <div class="text-center text-lg text-neutral-gray leading-relaxed space-y-6">
                        <p>
                            I am a results-oriented Quality Assurance Engineer with a proven track record in both manual and automation testing. My experience spans across API and web services testing, and I have a strong command of Selenium with Java.
                        </p>
                        <p>
                            I thrive in Agile and Scrum environments, contributing to all stages of the software development and testing lifecycles. From creating detailed test plans and cases to analyzing results and reporting defects, I am committed to enhancing product quality and reliability.
                        </p>
                    </div>
                </div>
            </div>
        </section>

        <!-- Experience Section -->
        <section id="experience" class="py-20">
            <div class="container mx-auto px-6">
                <h2 class="section-title fade-in-up">Professional Experience</h2>
                <div class="relative professional-timeline max-w-4xl mx-auto">
                    <div class="timeline-line"></div>
                    
                    <!-- Timeline Item 1 -->
                    <div class="timeline-item">
                        <div class="timeline-marker"></div>
                        <div class="professional-card ml-16">
                            <h3 class="text-xl font-bold text-dark-gray mb-2">QA Engineer</h3>
                            <p class="text-primary-blue font-semibold text-lg mb-2">Tata Consultancy Services LTD</p>
                            <p class="text-neutral-gray mb-3">May 2023 - Present | Hyderabad</p>
                            <p class="text-neutral-gray">Supported the software engineering team with a strong emphasis on development and testing excellence. Oversaw the end-to-end software testing process and promoted knowledge sharing.</p>
                        </div>
                    </div>
                    
                    <!-- Timeline Item 2 -->
                    <div class="timeline-item">
                        <div class="timeline-marker"></div>
                        <div class="professional-card mr-16">
                            <h3 class="text-xl font-bold text-dark-gray mb-2">QA Engineer</h3>
                            <p class="text-primary-blue font-semibold text-lg mb-2">Carelon Global Solutions India LLP</p>
                            <p class="text-neutral-gray mb-3">Sep 2020 - Apr 2023 | Hyderabad</p>
                            <p class="text-neutral-gray">Guided the software testing team in adopting and refining testing methodologies. Contributed to both manual and automation testing, engaging in the full software development lifecycle.</p>
                        </div>
                    </div>
                </div>
            </div>
        </section>

        <!-- Projects Section -->
        <section id="projects" class="py-20">
            <div class="container mx-auto px-6">
                <h2 class="section-title fade-in-up">Key Projects</h2>
                <div class="grid md:grid-cols-2 lg:grid-cols-3 gap-8">
		    <!-- Project Card 1 -->
                    <div class="professional-card fade-in-up stagger-1">
                        <h3 class="text-xl font-bold text-dark-gray mb-3">Automation solutions</h3>
                        <p class="text-primary-blue font-semibold mb-3">Client: PwC</p>
                        <p class="text-neutral-gray mb-4">Worked on functional and automation testing for web application.Handled integrated functional testing and automated scripts from scratch.</p>
                        <div class="flex flex-wrap gap-2">
                            <span class="skill-badge text-sm">Karate Framework</span>
                            <span class="skill-badge text-sm">MongoDB</span>
			    <span class="skill-badge text-sm">Azure Devops</span>
                        </div>
                    </div>



                    <!-- Project Card 2 -->
                    <div class="professional-card fade-in-up stagger-1">
                        <h3 class="text-xl font-bold text-dark-gray mb-3">Learn Platform</h3>
                        <p class="text-primary-blue font-semibold mb-3">Client: PwC</p>
                        <p class="text-neutral-gray mb-4">Worked on functional and automation testing for an E-Learning platform. Handled integrated functional testing and automated scripts from scratch.</p>
                        <div class="flex flex-wrap gap-2">
                            <span class="skill-badge text-sm">Karate Framework</span>
                            <span class="skill-badge text-sm">MongoDB</span>
                            <span class="skill-badge text-sm">Mobile Testing</span>
			    <span class="skill-badge text-sm">Azure Devops</span>
                        </div>
                    </div>
                    
                    <!-- Project Card 3 -->
                    <div class="professional-card fade-in-up stagger-2">
                        <h3 class="text-xl font-bold text-dark-gray mb-3">CDX</h3>
                        <p class="text-primary-blue font-semibold mb-3">Client: GE Health Care</p>
                        <p class="text-neutral-gray mb-4">Performed functional and automation testing for user stories on a weekly sprint basis. Created regression test cases and worked on the end-to-end bug life cycle.</p>
                        <div class="flex flex-wrap gap-2">
                            <span class="skill-badge text-sm">Rally</span>
                            <span class="skill-badge text-sm">Functionize</span>
                            <span class="skill-badge text-sm">API Testing</span>
                        </div>
                    </div>
                    
                    <!-- Project Card 4 -->
                    <div class="professional-card fade-in-up stagger-3">
                        <h3 class="text-xl font-bold text-dark-gray mb-3">Claims Intake & Workflow</h3>
                        <p class="text-primary-blue font-semibold mb-3">Client: Elevance Health</p>
                        <p class="text-neutral-gray mb-4">Performed manual testing in all phases (System, Integration) and automation regression testing. Developed and implemented automated test scripts.</p>
                        <div class="flex flex-wrap gap-2">
                            <span class="skill-badge text-sm">Pega</span>
                            <span class="skill-badge text-sm">Selenium</span>
                            <span class="skill-badge text-sm">JIRA</span>
                        </div>
                    </div>
                </div>
            </div>
        </section>

        <!-- Tools Section -->
        <section id="tools" class="py-20">
            <div class="container mx-auto px-6">
                <h2 class="section-title fade-in-up">Tools & Technologies</h2>
                
                <!-- Testing Tools -->
                <div class="mb-12 fade-in-up">
                    <h3 class="text-2xl font-bold text-center mb-8 text-primary-blue">Testing & Automation</h3>
                    <div class="tools-grid">
                        <div class="tool-card">
                            <div class="tool-category">Automation</div>
                            <i class="fab fa-python tool-icon"></i>
                            <div class="font-semibold text-dark-gray">Selenium</div>
                        </div>
                        <div class="tool-card">
                            <div class="tool-category">API Testing</div>
                            <i class="fas fa-code tool-icon"></i>
                            <div class="font-semibold text-dark-gray">Karate DSL</div>
                        </div>
                        <div class="tool-card">
                            <div class="tool-category">AI Testing</div>
                            <i class="fas fa-robot tool-icon"></i>
                            <div class="font-semibold text-dark-gray">Functionize</div>
                        </div>
                        <div class="tool-card">
                            <div class="tool-category">Mobile Testing</div>
                            <i class="fas fa-mobile-alt tool-icon"></i>
                            <div class="font-semibold text-dark-gray">Mobile Testing</div>
                        </div>
                        <div class="tool-card">
                            <div class="tool-category">Performance</div>
                            <i class="fas fa-tachometer-alt tool-icon"></i>
                            <div class="font-semibold text-dark-gray">Performance Testing</div>
                        </div>
                        <div class="tool-card">
                            <div class="tool-category">Automation</div>
                            <i class="fas fa-cogs tool-icon"></i>
                            <div class="font-semibold text-dark-gray">Simplify3X</div>
                        </div>
                    </div>
                </div>

                <!-- Project Management -->
                <div class="mb-12 fade-in-up">
                    <h3 class="text-2xl font-bold text-center mb-8 text-primary-blue">Project Management</h3>
                    <div class="tools-grid">
                        <div class="tool-card">
                            <div class="tool-category">Issue Tracking</div>
                            <i class="fab fa-atlassian tool-icon"></i>
                            <div class="font-semibold text-dark-gray">JIRA</div>
                        </div>
                        <div class="tool-card">
                            <div class="tool-category">DevOps</div>
                            <i class="fab fa-microsoft tool-icon"></i>
                            <div class="font-semibold text-dark-gray">Azure DevOps</div>
                        </div>
                        <div class="tool-card">
                            <div class="tool-category">Agile</div>
                            <i class="fas fa-chart-line tool-icon"></i>
                            <div class="font-semibold text-dark-gray">Rally</div>
                        </div>
                        <div class="tool-card">
                            <div class="tool-category">BPM</div>
                            <i class="fas fa-sitemap tool-icon"></i>
                            <div class="font-semibold text-dark-gray">Pega</div>
                        </div>
                    </div>
                </div>

                <!-- Databases & Languages -->
                <div class="fade-in-up">
                    <h3 class="text-2xl font-bold text-center mb-8 text-primary-blue">Databases & Languages</h3>
                    <div class="tools-grid">
                        <div class="tool-card">
                            <div class="tool-category">Database</div>
                            <i class="fas fa-leaf tool-icon"></i>
                            <div class="font-semibold text-dark-gray">MongoDB</div>
                        </div>
                        <div class="tool-card">
                            <div class="tool-category">Language</div>
                            <i class="fab fa-java tool-icon"></i>
                            <div class="font-semibold text-dark-gray">Java</div>
                        </div>
                        <div class="tool-card">
                            <div class="tool-category">Database</div>
                            <i class="fas fa-database tool-icon"></i>
                            <div class="font-semibold text-dark-gray">SQL</div>
                        </div>
                    </div>
                </div>
            </div>
        </section>

        <!-- Skills Section -->
        <section id="skills" class="py-20">
            <div class="container mx-auto px-6">
                <h2 class="section-title fade-in-up">Skills & Competencies</h2>
                <div class="max-w-5xl mx-auto">
                    <div class="mb-12 fade-in-up">
                        <h3 class="text-2xl font-bold text-center mb-8 text-primary-blue">Technical Skills</h3>
                        <div class="skills-grid">
                            <div class="skill-badge">Manual Testing</div>
                            <div class="skill-badge">Automation Testing</div>
                            <div class="skill-badge">API Testing</div>
                            <div class="skill-badge">Performance Testing</div>
                            <div class="skill-badge">Mobile Testing</div>
                            <div class="skill-badge">Regression Testing</div>
                            <div class="skill-badge">Test Planning</div>
                            <div class="skill-badge">Bug Tracking</div>
                        </div>
                    </div>
                    <div class="fade-in-up">
                        <h3 class="text-2xl font-bold text-center mb-8 text-primary-blue">Soft Skills & Methodologies</h3>
                        <div class="skills-grid">
                            <div class="skill-badge">Communication</div>
                            <div class="skill-badge">Leadership</div>
                            <div class="skill-badge">Teamwork</div>
                            <div class="skill-badge">Problem Solving</div>
                            <div class="skill-badge">Agile Testing</div>
                            <div class="skill-badge">Scrum</div>
                            <div class="skill-badge">SDLC</div>
                            <div class="skill-badge">STLC</div>
                        </div>
                    </div>
                </div>
            </div>
        </section>

        <!-- Education Section -->
        <section id="education" class="py-20">
            <div class="container mx-auto px-6">
                <h2 class="section-title fade-in-up">Education</h2>
                <div class="glass-premium max-w-3xl mx-auto p-12 text-center fade-in-up">
                    <h3 class="text-2xl font-bold text-dark-gray mb-3">Bachelor of Technology (B.Tech, ECE)</h3>
                    <p class="text-primary-blue text-xl font-semibold mb-2">Koneru Lakshmaiah University</p>
                    <p class="text-neutral-gray">Jul 2016 - May 2020</p>
		    <p class="text-neutral-gray">CGPA - 7.83</p>
                </div>
            </div>
        </section>

        <!-- Contact Section -->
        <section id="contact" class="py-20">
            <div class="container mx-auto px-6">
                <h2 class="section-title fade-in-up">Let's Connect</h2>
                <div class="glass-premium max-w-4xl mx-auto p-12 text-center fade-in-up">
                    <p class="max-w-2xl mx-auto mb-8 text-lg text-neutral-gray">
                        I'm currently seeking new opportunities and would love to hear from you. Whether you have a question or just want to say hi, feel free to reach out.
                    </p>
                    <div class="flex flex-col md:flex-row justify-center items-center space-y-4 md:space-y-0 md:space-x-6">
                        <a href="mailto:ramakrishnakodali1998@gmail.com" class="contact-card flex items-center gap-3">
                            <i class="fas fa-envelope text-primary-blue text-xl"></i>
                            <span class="text-dark-gray font-medium">ramakrishnakodali98@gmail.com</span>
                        </a>
                        <a href="https://www.linkedin.com/in/ramakrishnakodali/" class="contact-card flex items-center gap-3">
                            <i class="fab fa-linkedin text-primary-blue text-xl"></i>
                            <span class="text-dark-gray font-medium">LinkedIn</span>
                        </a>
                        <span class="contact-card flex items-center gap-3">
                            <i class="fas fa-phone text-success-green text-xl"></i>
                            <span class="text-dark-gray font-medium">+91 9493171709</span>
                        </span>
                    </div>
                </div>
            </div>
        </section>
    </main>

    <!-- Footer -->
    <footer class="py-8">
        <div class="container mx-auto px-6 text-center">
            <div class="glass-premium p-6">
                <p class="text-neutral-gray">&copy; 2025 Ramakrishna Kodali. All Rights Reserved.</p>
            </div>
        </div>
    </footer>

    <!-- Scroll to Top Button -->
    <div id="scroll-to-top" class="scroll-to-top">
        <i class="fas fa-arrow-up"></i>
    </div>

    <script>
        // Header scroll effect
        const header = document.getElementById('header');
        window.addEventListener('scroll', () => {
            if (window.scrollY > 100) {
                header.classList.add('scrolled');
            } else {
                header.classList.remove('scrolled');
            }
        });

        // Mobile menu toggle
        const mobileMenuButton = document.getElementById('mobile-menu-button');
        const mobileMenu = document.getElementById('mobile-menu');
        mobileMenuButton.addEventListener('click', () => {
            mobileMenu.classList.toggle('hidden');
        });

        // Smooth scrolling
        document.querySelectorAll('a[href^="#"]').forEach(anchor => {
            anchor.addEventListener('click', function (e) {
                if (this.getAttribute('href') !== '#') {
                    e.preventDefault();
                    if (!mobileMenu.classList.contains('hidden')) {
                        mobileMenu.classList.add('hidden');
                    }
                    document.querySelector(this.getAttribute('href')).scrollIntoView({
                        behavior: 'smooth'
                    });
                }
            });
        });

        // Scroll to top button
        const scrollToTopBtn = document.getElementById('scroll-to-top');
        window.addEventListener('scroll', () => {
            if (window.pageYOffset > 300) {
                scrollToTopBtn.classList.add('show');
            } else {
                scrollToTopBtn.classList.remove('show');
            }
        });
        scrollToTopBtn.addEventListener('click', () => {
            window.scrollTo({ top: 0, behavior: 'smooth' });
        });

        // Intersection Observer for animations
        const observerOptions = {
            threshold: 0.1,
            rootMargin: '0px 0px -50px 0px'
        };

        const observer = new IntersectionObserver((entries) => {
            entries.forEach(entry => {
                if (entry.isIntersecting) {
                    entry.target.classList.add('visible');
                }
            });
        }, observerOptions);

        // Observe all animated elements
        document.querySelectorAll('.fade-in-up, .timeline-item').forEach(el => {
            observer.observe(el);
        });

        // Parallax effect for background
        window.addEventListener('scroll', () => {
            const scrolled = window.pageYOffset;
            const parallax = document.querySelector('.professional-background');
            const speed = scrolled * 0.5;
            parallax.style.transform = `translateY(${speed}px)`;
        });
    </script>
</body>
</html>
