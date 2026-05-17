<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>GS Sai Kamal - AI/ML Portfolio</title>
    
    <script src="https://cdn.tailwindcss.com"></script>
    
    <script src="https://unpkg.com/lucide@latest/dist/umd/lucide.js"></script>
    <style>
        /* Custom styles for the portfolio theme */
        :root {
            --primary-red: #E9454E; /* Bright Red Accent */
            --dark-background: #121212; /* Very dark background */
            --dark-card: #202020; /* Slightly lighter card background */
            --text-light: #f3f4f6; /* Light gray text */
            --text-muted: #9ca3af; /* Muted gray text */
        }
        body {
            font-family: 'Inter', sans-serif;
            background-color: var(--dark-background);
            color: var(--text-light);
            /* Smooth scrolling for navigation */
            scroll-behavior: smooth;
        }

        /* Specific style for the dark background image section */
        .hero-image-container {
            position: relative;
            background-color: var(--dark-background); 
            border-radius: 12px;
            overflow: hidden;
            /* Using a linear gradient to add a subtle dark overlay for effect */
            background-image: linear-gradient(to bottom, rgba(18, 18, 18, 0.4), rgba(18, 18, 18, 0.7));
            background-size: cover;
            background-position: center;
        }
        /* Style for the actual image inside the hero container */
        .hero-image-container img {
            position: absolute;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            /* Removed object-fit: contain here to let inline classes take control */
            mix-blend-mode: luminosity; /* Blends the image with the background for the dark/red effect */
            opacity: 0.9; 
        }


        /* Red accent line for section titles */
        .accent-line::before {
            content: '';
            display: block;
            width: 32px;
            height: 3px;
            background-color: var(--primary-red);
            margin-bottom: 0.5rem;
        }

        /* Custom button styling */
        .btn-primary {
            background-color: var(--primary-red);
            color: white;
            padding: 0.75rem 1.5rem;
            border-radius: 8px;
            font-weight: 600;
            transition: background-color 0.3s;
        }
        .btn-primary:hover {
            background-color: #c93a40; /* Darker red on hover */
        }
        
        /* Skills badges */
        .skill-badge {
            background-color: var(--dark-card);
            border: 1px solid var(--primary-red);
            color: var(--text-light);
            padding: 0.5rem 1rem;
            border-radius: 6px;
            font-size: 0.875rem;
            font-weight: 500;
            transition: transform 0.2s;
        }
        .skill-badge:hover {
            transform: translateY(-2px);
            box-shadow: 0 4px 6px rgba(233, 69, 78, 0.2);
        }
    </style>
</head>
<body>

    <header class="fixed top-0 left-0 right-0 bg-opacity-95 bg-[--dark-background] backdrop-blur-sm z-50 shadow-lg">
        <nav class="container mx-auto px-4 sm:px-6 lg:px-8 py-4 flex justify-between items-center">
            
            <a href="#hero" class="text-2xl font-extrabold text-[--primary-red]">GS Sai Kamal<span class="text-white"></span></a>
            
            <div class="hidden md:flex space-x-8 text-sm font-medium">
                <a href="#hero" class="hover:text-[--primary-red] transition duration-300">HOME</a>
                <a href="https://drive.google.com/file/d/1oUg7XDwa5H2Z6zsnJan87hFyTdHHK8Do/view?usp=sharing" target="_blank" class="hover:text-[--primary-red] transition duration-300">RESUME</a>
                <a href="#about" class="hover:text-[--primary-red] transition duration-300">ABOUT ME</a>
                <a href="#contact-footer" class="hover:text-[--primary-red] transition duration-300">CONTACT</a>
            </div>

            </nav>
    </header>

    <main>
        <section id="hero" class="pt-24 pb-24 container mx-auto px-4 sm:px-6 lg:px-8">
            <div class="grid md:grid-cols-2 gap-16 items-center">
                
                <div class="space-y-6">
                    <p class="text-lg text-[--text-muted]">Hello, My Name Is</p>
                    <h1 class="text-6xl font-extrabold leading-tight">
                        <span class="text-[--primary-red]">GS SAI KAMAL</span>
                    </h1>
                    <p class="text-xl text-[--text-muted] max-w-lg">
                        An Aspiring Artificial Intelligence and Machine Learning Student, driven by a passion for creating data-driven systems and cutting-edge software solutions.
                    </p>
                    
                    <a href="mailto:gssaikamal99@gmail.com" class="btn-primary inline-block">Contact me</a>
                </div>

                <div class="hero-image-container h-96 w-full max-w-md mx-auto md:mx-0">
                    <img 
                        src="https://ik.imagekit.io/uyfhu28ch/profile_pic.jpg" 
                        alt="GS Sai Kamal Profile Photo" 
                        class="w-full h-full object-contain rounded-xl"
                    >
                </div>
            </div>
        </section>

        <section id="about" class="py-24 bg-[--dark-card]">
            <div class="container mx-auto px-4 sm:px-6 lg:px-8">
                <div class="grid md:grid-cols-2 gap-16 items-start">
                    
                    <div class="flex flex-col gap-6 w-full max-w-md mx-auto md:mx-0">
                        <div class="hero-image-container h-[450px] w-full opacity-100">
                            <img 
                                src="https://ik.imagekit.io/uyfhu28ch/Normal_pic.jpg" 
                                alt="GS Sai Kamal Working Photo" 
                                class="w-full h-full object-cover rounded-xl"
                            >
                        </div>

                        <div class="flex flex-wrap justify-center md:justify-start gap-8 mt-2">
                            <a href="https://github.com/GSSaiKamal/" target="_blank" class="flex items-center gap-3 text-[--text-muted] hover:text-[--primary-red] transition duration-300 group">
                                <i data-lucide="github" class="w-8 h-8 group-hover:scale-110 transition-transform"></i>
                                <span class="font-semibold text-lg">GitHub</span>
                            </a>

                            <a href="https://www.linkedin.com/in/gs-sai-kamal-b9a635343" target="_blank" class="flex items-center gap-3 text-[--text-muted] hover:text-[--primary-red] transition duration-300 group">
                                <i data-lucide="linkedin" class="w-8 h-8 group-hover:scale-110 transition-transform"></i>
                                <span class="font-semibold text-lg">LinkedIn</span>
                            </a>

                            <a href="mailto:gssaikamal99@gmail.com" class="flex items-center gap-3 text-[--text-muted] hover:text-[--primary-red] transition duration-300 group">
                                <i data-lucide="mail" class="w-8 h-8 group-hover:scale-110 transition-transform"></i>
                                <span class="font-semibold text-lg">Email</span>
                            </a>
                        </div>
                    </div>

                    <div class="space-y-8">
                        <div>
                            <p class="text-[--primary-red] text-sm tracking-widest accent-line">About me</p>
                            <h2 class="text-3xl font-bold mt-2">Who Am I</h2>
                        </div>
                        
                        <div class="text-[--text-muted] space-y-4">
                            <p>My name is GS Sai Kamal, and I am an aspiring AI/ML Student with a strong educational background in Computer Science and Data Science. I am driven by the intersection of data, algorithms, and technology, thriving on the challenge of turning complex problems into scalable, intelligent solutions.</p>
                            <p>My primary focus is on machine learning, where I excel at using "Python", "TensorFlow", and "Scikit-learn" to build predictive models and automated systems, such as my "Desktop Virtual Assistant" and "Video Summarization System". I am also proficient in "Java" and full-stack concepts, laying a solid foundation for robust software development.</p>
                            <p>I am a detail-oriented, quick learner committed to leveraging the latest trends in AI to deliver cutting-edge results.</p>
                        </div>

                        <div class="pt-4">
                            <h3 class="text-lg font-semibold mb-4 text-white">Skills:</h3>
                            <div class="flex flex-wrap gap-3">
                                <span class="skill-badge">Python</span>
                                <span class="skill-badge">Machine Learning</span>
                                <span class="skill-badge">TensorFlow</span>
                                <span class="skill-badge">Natural Language Processing (NLP)</span>
                                <span class="skill-badge">SQL</span>
                                <span class="skill-badge">Java</span>
                                <span class="skill-badge">HTML/CSS/JS</span>
                                <span class="skill-badge">Data Structures & Algorithms</span>
                            </div>
                        </div>

                        <a href="https://drive.google.com/file/d/1oUg7XDwa5H2Z6zsnJan87hFyTdHHK8Do/view?usp=sharing" target="_blank" class="btn-primary inline-block mt-4">View Resume </a>
                    </div>
                </div>
            </div>
        </section>

        <section id="education" class="py-24 container mx-auto px-4 sm:px-6 lg:px-8">
            <div class="mb-12 text-center">
                <p class="text-[--primary-red] text-sm tracking-widest accent-line inline-block">My Path</p>
                <h2 class="text-3xl font-bold mt-2">Education & Scores</h2>
            </div>

            <div class="grid md:grid-cols-3 gap-12 px-4">
                <div class="flex flex-col items-center">
                    <div class="relative w-[160px] h-[160px] rounded-full shadow-xl transition-all duration-300 ease-in-out hover:shadow-[0_0_25px_#E9454E] hover:scale-105 cursor-pointer"
                         style="background: conic-gradient(var(--primary-red) 0% 73.4%, var(--dark-card) 73.4% 100%);">
                        <div class="absolute top-1/2 left-1/2 transform -translate-x-1/2 -translate-y-1/2 w-[130px] h-[130px] bg-[--dark-background] rounded-full flex items-center justify-center">
                            <span class="text-3xl font-extrabold text-white">73.4%</span>
                        </div>
                    </div>
                    <h3 class="text-xl font-bold text-white mt-6">10th Grade</h3>
                    <p class="text-[--text-muted] text-sm mt-1">Secondary School Certificate</p>
                </div>

                <div class="flex flex-col items-center">
                    <div class="relative w-[160px] h-[160px] rounded-full shadow-xl transition-all duration-300 ease-in-out hover:shadow-[0_0_25px_#E9454E] hover:scale-105 cursor-pointer"
                         style="background: conic-gradient(var(--primary-red) 0% 85.8%, var(--dark-card) 85.8% 100%);">
                        <div class="absolute top-1/2 left-1/2 transform -translate-x-1/2 -translate-y-1/2 w-[130px] h-[130px] bg-[--dark-background] rounded-full flex items-center justify-center">
                            <span class="text-3xl font-extrabold text-white">85.8%</span>
                        </div>
                    </div>
                    <h3 class="text-xl font-bold text-white mt-6">Intermediate</h3>
                    <p class="text-[--text-muted] text-sm mt-1">Higher Secondary</p>
                </div>

                <div class="flex flex-col items-center">
                    <div class="relative w-[160px] h-[160px] rounded-full shadow-xl transition-all duration-300 ease-in-out hover:shadow-[0_0_25px_#E9454E] hover:scale-105 cursor-pointer"
                         style="background: conic-gradient(var(--primary-red) 0% 84.2%, var(--dark-card) 84.2% 100%);">
                        <div class="absolute top-1/2 left-1/2 transform -translate-x-1/2 -translate-y-1/2 w-[130px] h-[130px] bg-[--dark-background] rounded-full flex items-center justify-center">
                            <span class="text-3xl font-extrabold text-white">8.42</span>
                        </div>
                    </div>
                    <h3 class="text-xl font-bold text-white mt-6">B.E. Current CGPA</h3>
                    <p class="text-[--text-muted] text-sm mt-1">Bachelor of Engineering</p>
                </div>
            </div>
        </section>

        <section id="services" class="py-24 container mx-auto px-4 sm:px-6 lg:px-8 bg-[--dark-card]">
            <div class="mb-12">
                <p class="text-[--primary-red] text-sm tracking-widest accent-line">My Capabilities</p>
                <h2 class="text-3xl font-bold mt-2">What I Can Do</h2>
            </div>
            
            <div class="grid sm:grid-cols-2 lg:grid-cols-3 gap-8">
                <div class="bg-[--dark-background] p-6 rounded-xl shadow-xl space-y-3 transition duration-300 hover:shadow-2xl hover:border-b-4 hover:border-[--primary-red]">
                    <i data-lucide="brain" class="text-[--primary-red] w-8 h-8"></i>
                    <h3 class="text-xl font-semibold text-white">AI/ML Model Design</h3>
                    <p class="text-[--text-muted] text-sm">Designing, training, and optimizing Machine Learning models for classification, regression, and complex prediction tasks using scikit-learn and TensorFlow.</p>
                </div>

                <div class="bg-[--dark-background] p-6 rounded-xl shadow-xl space-y-3 transition duration-300 hover:shadow-2xl hover:border-b-4 hover:border-[--primary-red]">
                    <i data-lucide="message-square-text" class="text-[--primary-red] w-8 h-8"></i>
                    <h3 class="text-xl font-semibold text-white">Natural Language Processing</h3>
                    <p class="text-[--text-muted] text-sm">Developing applications for text summarization, sentiment analysis, and virtual assistants to enhance automation and user interaction (e.g., Desktop Assistant project).</p>
                </div>

                <div class="bg-[--dark-background] p-6 rounded-xl shadow-xl space-y-3 transition duration-300 hover:shadow-2xl hover:border-b-4 hover:border-[--primary-red]">
                    <i data-lucide="code" class="text-[--primary-red] w-8 h-8"></i>
                    <h3 class="text-xl font-semibold text-white">Software Development</h3>
                    <p class="text-[--text-muted] text-sm">Building robust and clean backend logic using Python and Java, following best practices for code efficiency and maintainability.</p>
                </div>

                <div class="bg-[--dark-background] p-6 rounded-xl shadow-xl space-y-3 transition duration-300 hover:shadow-2xl hover:border-b-4 hover:border-[--primary-red]">
                    <i data-lucide="layout-grid" class="text-[--primary-red] w-8 h-8"></i>
                    <h3 class="text-xl font-semibold text-white">Data Structures & Algorithms</h3>
                    <p class="text-[--text-muted] text-sm">Applying efficient data structures and algorithmic thinking to solve complex computational problems, ensuring high performance in all applications.</p>
                </div>

                <div class="bg-[--dark-background] p-6 rounded-xl shadow-xl space-y-3 transition duration-300 hover:shadow-2xl hover:border-b-4 hover:border-[--primary-red]">
                    <i data-lucide="database" class="text-[--primary-red] w-8 h-8"></i>
                    <h3 class="text-xl font-semibold text-white">Database Integration (SQL)</h3>
                    <p class="text-[--text-muted] text-sm">Designing and managing efficient databases (e.g., SQLite) and integrating them with web and desktop applications for secure data handling.</p>
                </div>

                <div class="bg-[--dark-background] p-6 rounded-xl shadow-xl space-y-3 transition duration-300 hover:shadow-2xl hover:border-b-4 hover:border-[--primary-red]">
                    <i data-lucide="monitor" class="text-[--primary-red] w-8 h-8"></i>
                    <h3 class="text-xl font-semibold text-white">Web Application Design</h3>
                    <p class="text-[--text-muted] text-sm">Creating intuitive and responsive user interfaces using HTML/CSS (Tailwind) and frameworks like Flask for full-stack project deployment.</p>
                </div>

                <div class="bg-[--dark-background] p-6 rounded-xl shadow-xl space-y-3 transition duration-300 hover:shadow-2xl hover:border-b-4 hover:border-[--primary-red]">
                    <i data-lucide="network" class="text-[--primary-red] w-8 h-8"></i>
                    <h3 class="text-xl font-semibold text-white">Interested in Computer Networks</h3>
                    <p class="text-[--text-muted] text-sm">Passionate about understanding network architectures, passive and cabling infrastructures, and data communication protocols for building scalable communication systems.</p>
                </div>
            </div>
        </section>

        <section class="py-24 bg-[--dark-card] text-center">
            <div class="container mx-auto px-4 sm:px-6 lg:px-8 max-w-2xl">
                <h2 class="text-4xl font-extrabold leading-snug mb-4 text-white">
                    Let's work together on your next project
                </h2>
                <p class="text-lg text-[--text-muted] mb-8">
                    Collaboration is key. Let's join forces and combine our skills to tackle your next project with a powerful synergy that guarantees success.
                </p>
                <a href="mailto:gssaikamal99@gmail.com" class="btn-primary inline-block text-lg">Contact me</a>
            </div>
        </section>

    </main>

    <footer id="contact-footer" class="py-10 bg-[--dark-background] border-t border-gray-800">
        <div class="container mx-auto px-4 sm:px-6 lg:px-8 flex flex-col md:flex-row justify-between items-center text-sm text-[--text-muted]">
            <div class="text-center md:text-left mb-4 md:mb-0">
                &copy; <span id="year"></span> GS Sai Kamal. All rights reserved.
            </div>
            
            <div class="flex space-x-6">
                <a href="https://github.com/GSSaiKamal/" target="_blank" class="hover:text-[--primary-red] transition duration-300">
                    <i data-lucide="github" class="w-5 h-5"></i>
                </a>
                <a href="https://www.linkedin.com/in/gs-sai-kamal-b9a635343" target="_blank" class="hover:text-[--primary-red] transition duration-300">
                    <i data-lucide="linkedin" class="w-5 h-5"></i>
                </a>
                <a href="mailto:gssaikamal99@gmail.com" class="hover:text-[--primary-red] transition duration-300">
                    <i data-lucide="mail" class="w-5 h-5"></i>
                </a>
            </div>
        </div>
    </footer>

    <script>
        // Initialize Lucide icons
        lucide.createIcons();

        // Set current year in the footer
        document.getElementById('year').textContent = new Date().getFullYear();
    </script>
</body>
</html>
