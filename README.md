<!DOCTYPE html>
<html lang="en" class="scroll-smooth">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Abdellah Bouabdli | Software Engineering Student</title>
    <!-- Fonts -->
    <link rel="preconnect" href="https://fonts.googleapis.com">
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
    <link href="https://fonts.googleapis.com/css2?family=Fira+Code:wght@400;500;600&family=Inter:wght@400;500;600;700;800&display=swap" rel="stylesheet">
    <!-- FontAwesome -->
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    <!-- Tailwind CSS -->
    <script src="https://cdn.tailwindcss.com"></script>
    <script>
        tailwind.config = {
            theme: {
                extend: {
                    colors: {
                        navy: '#0a192f',
                        lightNavy: '#112240',
                        lightestNavy: '#233554',
                        teal: '#64ffda',
                        slate: '#8892b0',
                        lightSlate: '#a8b2d1',
                        lightestSlate: '#ccd6f6',
                        white: '#e6f1ff',
                    },
                    fontFamily: {
                        sans: ['Inter', 'sans-serif'],
                        mono: ['Fira Code', 'monospace'],
                    }
                }
            }
        }
    </script>
    <style>
        /* Custom scrollbar for a polished look */
        ::-webkit-scrollbar {
            width: 8px;
        }
        ::-webkit-scrollbar-track {
            background: #0a192f;
        }
        ::-webkit-scrollbar-thumb {
            background: #233554;
            border-radius: 4px;
        }
        ::-webkit-scrollbar-thumb:hover {
            background: #8892b0;
        }
        
        body {
            background-color: #0a192f;
            color: #8892b0;
        }
        
        /* Section heading line */
        .numbered-heading::after {
            content: "";
            display: block;
            position: relative;
            top: -5px;
            width: 300px;
            height: 1px;
            margin-left: 20px;
            background-color: #233554;
        }
        @media (max-width: 768px) {
            .numbered-heading::after {
                width: 100%;
            }
        }
    </style>
</head>
<body class="antialiased selection:bg-teal selection:text-navy flex flex-col min-h-screen">

    <!-- Navigation -->
    <header class="fixed w-full top-0 z-50 bg-navy/90 backdrop-blur-sm shadow-sm transition-all duration-300 py-4 px-6 md:px-12 flex justify-between items-center">
        <a href="#" class="text-teal font-mono text-xl font-bold tracking-tighter">AB<span class="text-lightestSlate">.</span></a>
        <nav class="hidden md:flex items-center gap-8 font-mono text-sm">
            <a href="#about" class="text-lightSlate hover:text-teal transition-colors"><span class="text-teal">01.</span> About</a>
            <a href="#experience" class="text-lightSlate hover:text-teal transition-colors"><span class="text-teal">02.</span> Experience</a>
            <a href="#projects" class="text-lightSlate hover:text-teal transition-colors"><span class="text-teal">03.</span> Projects</a>
            <a href="#contact" class="text-lightSlate hover:text-teal transition-colors"><span class="text-teal">04.</span> Contact</a>
            <a href="mailto:abdalabouabdeli@gmail.com" class="text-teal border border-teal rounded px-4 py-2 hover:bg-teal/10 transition-colors ml-4">Resume</a>
        </nav>
        <!-- Mobile Menu Button (Visual Only for this artifact) -->
        <button class="md:hidden text-teal text-2xl">
            <i class="fa-solid fa-bars"></i>
        </button>
    </header>

    <!-- Main Content -->
    <main class="flex-grow px-6 md:px-24 lg:px-48 max-w-7xl mx-auto w-full">

        <!-- Hero Section -->
        <section id="hero" class="min-h-screen flex flex-col justify-center items-start pt-20">
            <p class="text-teal font-mono mb-5">Hi, my name is</p>
            <h1 class="text-4xl md:text-6xl lg:text-7xl font-bold text-lightestSlate mb-4 tracking-tight">Abdellah Bouabdli.</h1>
            <h2 class="text-3xl md:text-5xl lg:text-6xl font-bold text-slate mb-6 tracking-tight">I build enterprise-grade systems.</h2>
            
            <p class="max-w-2xl text-lg md:text-xl text-slate mb-10 leading-relaxed">
                I'm a <span class="text-teal">Software Engineering Student</span> & Full Stack Developer focused on designing clean, scalable, production-grade applications. I work across the stack — from complex data models and APIs to polished interfaces — with a strong product engineering mindset. 
                Currently exploring <span class="text-lightestSlate">AI & Machine Learning</span>.
            </p>
            
            <div class="flex flex-wrap gap-4 items-center">
                <a href="#projects" class="border border-teal text-teal px-7 py-4 rounded hover:bg-teal/10 transition-all font-mono text-sm">
                    Check out my work!
                </a>
                <a href="https://github.com/AbdellahBouabdli" target="_blank" class="text-lightSlate hover:text-teal p-3 text-2xl transition-colors">
                    <i class="fa-brands fa-github"></i>
                </a>
                <a href="https://linkedin.com/in/abdellah-bouabdli" target="_blank" class="text-lightSlate hover:text-teal p-3 text-2xl transition-colors">
                    <i class="fa-brands fa-linkedin"></i>
                </a>
            </div>
            
            <div class="mt-12 flex items-center gap-2 text-sm font-mono text-lightSlate">
                <i class="fa-solid fa-location-dot text-teal"></i> Based in Morocco
            </div>
        </section>

        <!-- About Section -->
        <section id="about" class="py-24 max-w-4xl">
            <h2 class="numbered-heading flex items-center text-2xl md:text-3xl font-bold text-lightestSlate mb-10 whitespace-nowrap">
                <span class="text-teal font-mono text-xl md:text-2xl mr-3">01.</span> About Me
            </h2>
            
            <div class="grid grid-cols-1 md:grid-cols-2 gap-12">
                <div>
                    <p class="mb-4 leading-relaxed">
                        Hello! My name is Abdellah and I enjoy creating things that live on the internet and run seamlessly on servers. My interest in software engineering started when I realized that writing clean lines of code could solve complex, real-world problems.
                    </p>
                    <p class="mb-4 leading-relaxed">
                        Today, I'm focused on mastering <span class="text-teal">Full Stack Development</span> and diving deep into <span class="text-teal">Artificial Intelligence & Machine Learning</span>. I have a strong foundation in building clean architectures, utilizing MVC patterns, and employing UML-driven design to ensure maintainability.
                    </p>
                    <p class="leading-relaxed">
                        Whether it's designing RESTful APIs, configuring relational databases, or crafting responsive user interfaces, I approach every challenge with a <span class="text-lightestSlate">Product Engineering Mindset</span>.
                    </p>
                </div>
                
                <div class="bg-lightNavy p-6 rounded-lg border border-lightestNavy">
                    <h3 class="text-lightestSlate font-semibold mb-4 flex items-center gap-2">
                        <i class="fa-solid fa-bullseye text-teal"></i> Current Focus
                    </h3>
                    <ul class="space-y-3 font-mono text-sm">
                        <li class="flex items-start gap-2">
                            <i class="fa-solid fa-caret-right text-teal mt-1"></i>
                            <span>Advanced Machine Learning & Deep Learning</span>
                        </li>
                        <li class="flex items-start gap-2">
                            <i class="fa-solid fa-caret-right text-teal mt-1"></i>
                            <span>System Design & Scalable Architecture</span>
                        </li>
                        <li class="flex items-start gap-2">
                            <i class="fa-solid fa-caret-right text-teal mt-1"></i>
                            <span>Cloud-Native Development (AWS)</span>
                        </li>
                        <li class="flex items-start gap-2">
                            <i class="fa-solid fa-caret-right text-teal mt-1"></i>
                            <span>MLOps & Model Deployment</span>
                        </li>
                    </ul>
                </div>
            </div>
            
            <!-- Tech Stack -->
            <div class="mt-16">
                <h3 class="text-lightestSlate font-semibold mb-6">Languages & Technologies I've been working with:</h3>
                
                <div class="grid grid-cols-2 md:grid-cols-4 gap-4 font-mono text-sm">
                    <!-- Languages -->
                    <div class="space-y-2">
                        <div class="text-teal mb-3 font-bold border-b border-lightestNavy pb-1 inline-block">Languages</div>
                        <p><i class="fa-solid fa-caret-right text-teal text-xs mr-2"></i>PHP & Python</p>
                        <p><i class="fa-solid fa-caret-right text-teal text-xs mr-2"></i>JavaScript (ES6+) / TS</p>
                        <p><i class="fa-solid fa-caret-right text-teal text-xs mr-2"></i>Java & C++</p>
                    </div>
                    <!-- Frontend -->
                    <div class="space-y-2">
                        <div class="text-teal mb-3 font-bold border-b border-lightestNavy pb-1 inline-block">Frontend</div>
                        <p><i class="fa-solid fa-caret-right text-teal text-xs mr-2"></i>React & Vue</p>
                        <p><i class="fa-solid fa-caret-right text-teal text-xs mr-2"></i>Tailwind CSS</p>
                        <p><i class="fa-solid fa-caret-right text-teal text-xs mr-2"></i>Bootstrap</p>
                    </div>
                    <!-- Backend -->
                    <div class="space-y-2">
                        <div class="text-teal mb-3 font-bold border-b border-lightestNavy pb-1 inline-block">Backend / DB</div>
                        <p><i class="fa-solid fa-caret-right text-teal text-xs mr-2"></i>Laravel (PHP)</p>
                        <p><i class="fa-solid fa-caret-right text-teal text-xs mr-2"></i>Node.js & Express</p>
                        <p><i class="fa-solid fa-caret-right text-teal text-xs mr-2"></i>MySQL & Postgres</p>
                        <p><i class="fa-solid fa-caret-right text-teal text-xs mr-2"></i>MongoDB</p>
                    </div>
                    <!-- Tools -->
                    <div class="space-y-2">
                        <div class="text-teal mb-3 font-bold border-b border-lightestNavy pb-1 inline-block">DevOps & Tools</div>
                        <p><i class="fa-solid fa-caret-right text-teal text-xs mr-2"></i>Git & GitHub</p>
                        <p><i class="fa-solid fa-caret-right text-teal text-xs mr-2"></i>Docker</p>
                        <p><i class="fa-solid fa-caret-right text-teal text-xs mr-2"></i>AWS & Linux</p>
                    </div>
                </div>
            </div>
        </section>

        <!-- Experience Section -->
        <section id="experience" class="py-24 max-w-3xl">
            <h2 class="numbered-heading flex items-center text-2xl md:text-3xl font-bold text-lightestSlate mb-10 whitespace-nowrap">
                <span class="text-teal font-mono text-xl md:text-2xl mr-3">02.</span> Experience
            </h2>
            
            <div class="flex flex-col md:flex-row gap-8">
                <!-- Timeline/Tabs style left bar -->
                <div class="flex md:flex-col overflow-x-auto md:w-48 border-b md:border-b-0 md:border-l border-lightestNavy no-scrollbar">
                    <button class="px-5 py-3 border-b-2 md:border-b-0 md:border-l-2 border-teal text-teal bg-lightNavy/50 text-left font-mono text-sm whitespace-nowrap transition-all">
                        Independent / Academic
                    </button>
                </div>
                
                <!-- Content -->
                <div class="w-full">
                    <h3 class="text-xl font-medium text-lightestSlate mb-1">
                        Software Engineering Intern
                    </h3>
                    <p class="text-lightSlate font-mono text-sm mb-5">2024 — Present</p>
                    
                    <ul class="space-y-4 text-slate leading-relaxed">
                        <li class="flex items-start gap-3">
                            <i class="fa-solid fa-caret-right text-teal mt-1.5 text-sm"></i>
                            <span>Designing and building full stack applications and AI-integrated tools while pursuing a software engineering degree, focusing on production-quality code.</span>
                        </li>
                        <li class="flex items-start gap-3">
                            <i class="fa-solid fa-caret-right text-teal mt-1.5 text-sm"></i>
                            <span>Architected a Laravel MVC school management system with full RBAC, utilizing UML use-case, class, and sequence diagrams.</span>
                        </li>
                        <li class="flex items-start gap-3">
                            <i class="fa-solid fa-caret-right text-teal mt-1.5 text-sm"></i>
                            <span>Built and optimized relational schemas, migrations, and Eloquent models for robust data management.</span>
                        </li>
                        <li class="flex items-start gap-3">
                            <i class="fa-solid fa-caret-right text-teal mt-1.5 text-sm"></i>
                            <span>Integrated AI/ML capabilities into full stack applications ensuring seamless API contracts.</span>
                        </li>
                    </ul>
                </div>
            </div>
        </section>

        <!-- Projects Section -->
        <section id="projects" class="py-24">
            <h2 class="numbered-heading flex items-center text-2xl md:text-3xl font-bold text-lightestSlate mb-12 whitespace-nowrap">
                <span class="text-teal font-mono text-xl md:text-2xl mr-3">03.</span> Featured Projects
            </h2>
            
            <div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-6">
                <!-- Project 1 -->
                <div class="bg-lightNavy rounded-lg p-7 hover:-translate-y-2 transition-all duration-300 hover:shadow-2xl hover:shadow-teal/10 flex flex-col h-full group">
                    <div class="flex justify-between items-center mb-6">
                        <i class="fa-regular fa-folder text-teal text-4xl group-hover:text-white transition-colors"></i>
                        <div class="flex gap-4">
                            <a href="https://github.com/AbdellahBouabdli" class="text-lightSlate hover:text-teal transition-colors text-xl"><i class="fa-brands fa-github"></i></a>
                        </div>
                    </div>
                    <h3 class="text-lightestSlate text-xl font-bold mb-3 group-hover:text-teal transition-colors">Système de Gestion Scolaire</h3>
                    <p class="text-slate text-sm mb-6 flex-grow leading-relaxed">
                        Enterprise-grade school management platform built with a clean MVC architecture. Models the full educational lifecycle featuring RBAC (Admin/Prof/Student), grading, scheduling, and digital report generation. Designed completely from UML models.
                    </p>
                    <ul class="flex flex-wrap gap-x-3 gap-y-2 text-xs font-mono text-lightSlate mt-auto">
                        <li>Laravel</li>
                        <li>PHP</li>
                        <li>MySQL</li>
                        <li>Bootstrap</li>
                    </ul>
                </div>

                <!-- Project 2 -->
                <div class="bg-lightNavy rounded-lg p-7 hover:-translate-y-2 transition-all duration-300 hover:shadow-2xl hover:shadow-teal/10 flex flex-col h-full group">
                    <div class="flex justify-between items-center mb-6">
                        <i class="fa-regular fa-folder text-teal text-4xl group-hover:text-white transition-colors"></i>
                        <div class="flex gap-4">
                            <a href="https://github.com/AbdellahBouabdli" class="text-lightSlate hover:text-teal transition-colors text-xl"><i class="fa-brands fa-github"></i></a>
                        </div>
                    </div>
                    <h3 class="text-lightestSlate text-xl font-bold mb-3 group-hover:text-teal transition-colors">AI-Powered Productivity Engine</h3>
                    <p class="text-slate text-sm mb-6 flex-grow leading-relaxed">
                        A full stack application integrating LLM capabilities to automate summarization, classification, and intelligent search over user content. Features async processing, caching, and a responsive frontend.
                    </p>
                    <ul class="flex flex-wrap gap-x-3 gap-y-2 text-xs font-mono text-lightSlate mt-auto">
                        <li>React</li>
                        <li>Node.js</li>
                        <li>Python</li>
                        <li>LLMs</li>
                    </ul>
                </div>

                <!-- Project 3 -->
                <div class="bg-lightNavy rounded-lg p-7 hover:-translate-y-2 transition-all duration-300 hover:shadow-2xl hover:shadow-teal/10 flex flex-col h-full group">
                    <div class="flex justify-between items-center mb-6">
                        <i class="fa-regular fa-folder text-teal text-4xl group-hover:text-white transition-colors"></i>
                        <div class="flex gap-4">
                            <a href="https://github.com/AbdellahBouabdli" class="text-lightSlate hover:text-teal transition-colors text-xl"><i class="fa-brands fa-github"></i></a>
                            <a href="#" class="text-lightSlate hover:text-teal transition-colors text-xl"><i class="fa-solid fa-arrow-up-right-from-square"></i></a>
                        </div>
                    </div>
                    <h3 class="text-lightestSlate text-xl font-bold mb-3 group-hover:text-teal transition-colors">Full Stack Web Platform</h3>
                    <p class="text-slate text-sm mb-6 flex-grow leading-relaxed">
                        A modern, responsive web platform demonstrating end-to-end engineering practices. Showcases data modeling, authenticated APIs, role guards, lazy loading, and a polished component-driven UI.
                    </p>
                    <ul class="flex flex-wrap gap-x-3 gap-y-2 text-xs font-mono text-lightSlate mt-auto">
                        <li>Laravel</li>
                        <li>React</li>
                        <li>Tailwind</li>
                        <li>Docker</li>
                    </ul>
                </div>
            </div>
        </section>

        <!-- Contact / Connect Section -->
        <section id="contact" class="py-32 max-w-2xl mx-auto text-center">
            <p class="text-teal font-mono mb-4 text-sm">04. What's Next?</p>
            <h2 class="text-4xl md:text-5xl font-bold text-lightestSlate mb-6">Get In Touch</h2>
            <p class="text-slate text-lg mb-12 leading-relaxed">
                I'm always open to discussing internships, open source collaborations, research, and Full Stack or AI roles. Whether you have a question or just want to say hi, I'll try my best to get back to you!
            </p>
            <a href="mailto:abdalabouabdeli@gmail.com" class="border border-teal text-teal px-8 py-4 rounded hover:bg-teal/10 transition-all font-mono text-sm inline-block">
                Say Hello
            </a>
        </section>

    </main>

    <!-- Footer -->
    <footer class="text-center p-6 mt-auto">
        <div class="flex justify-center gap-6 mb-6 md:hidden">
            <!-- Mobile Links -->
            <a href="https://github.com/AbdellahBouabdli" class="text-lightSlate hover:text-teal transition-colors text-xl"><i class="fa-brands fa-github"></i></a>
            <a href="https://linkedin.com/in/abdellah-bouabdli" class="text-lightSlate hover:text-teal transition-colors text-xl"><i class="fa-brands fa-linkedin"></i></a>
        </div>
        <p class="text-slate font-mono text-xs mb-2">
            "Engineering is the art of turning complexity into clarity — one clean line at a time."
        </p>
        <p class="text-lightSlate font-mono text-xs hover:text-teal transition-colors cursor-pointer inline-block">
            Designed & Built by Abdellah Bouabdli
        </p>
    </footer>

    <!-- Side Social Elements (Visible on lg screens) -->
    <div class="hidden lg:flex flex-col items-center fixed bottom-0 left-10 z-10 gap-6">
        <a href="https://github.com/AbdellahBouabdli" target="_blank" class="text-lightSlate hover:text-teal hover:-translate-y-1 transition-all text-xl"><i class="fa-brands fa-github"></i></a>
        <a href="https://linkedin.com/in/abdellah-bouabdli" target="_blank" class="text-lightSlate hover:text-teal hover:-translate-y-1 transition-all text-xl"><i class="fa-brands fa-linkedin"></i></a>
        <div class="w-[1px] h-24 bg-lightSlate mt-2"></div>
    </div>
    <div class="hidden lg:flex flex-col items-center fixed bottom-0 right-10 z-10 gap-6">
        <a href="mailto:abdalabouabdeli@gmail.com" class="text-lightSlate hover:text-teal hover:-translate-y-1 transition-all font-mono text-xs" style="writing-mode: vertical-rl;">
            abdalabouabdeli@gmail.com
        </a>
        <div class="w-[1px] h-24 bg-lightSlate mt-2"></div>
    </div>

</body>
</html>
