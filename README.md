
        }

        body {
            background-color: var(--bg-color); /* Fallback */
            /* Subtle diagonal line pattern for a textured, "old money" feel */
            background-image: repeating-linear-gradient(
                45deg,
                transparent,
                transparent 15px,
                rgba(10, 35, 66, 0.03) 15px, /* Using a hint of the primary navy color for the lines */
                rgba(10, 35, 66, 0.03) 17px
            );
            color: var(--text-color);
            font-family: 'Lato', sans-serif;
        }

        h1, h2, h3, h4, h5, h6 {
            font-family: 'Lora', serif;
        }
        
        .section-title {
            border-bottom: 3px solid var(--secondary-color);
            padding-bottom: 0.5rem;
            margin-bottom: 2rem;
            color: var(--primary-color);
        }

        html {
            scroll-behavior: smooth;
        }

        /* Animations */
        .fade-in-section {
            opacity: 0;
            transform: translateY(20px);
            transition: opacity 0.8s ease-out, transform 0.8s ease-out;
        }

        .fade-in-section.is-visible {
            opacity: 1;
            transform: translateY(0);
        }
        
        .nav-link {
            position: relative;
            transition: color 0.3s ease;
        }

        .nav-link::after {
            content: '';
            position: absolute;
            width: 0;
            height: 2px;
            bottom: -4px;
            left: 50%;
            background-color: var(--secondary-color);
            transition: all 0.3s ease-in-out;
        }

        .nav-link:hover {
            color: var(--primary-color);
        }

        .nav-link:hover::after {
            width: 100%;
            left: 0;
        }

    </style>
</head>
<body class="antialiased">

    <!-- Header & Navigation -->
    <header class="bg-[var(--bg-color)] shadow-sm sticky top-0 z-50">
        <nav class="container mx-auto px-6 py-4 flex justify-between items-center">
            <a href="#" class="text-2xl font-bold" style="color: var(--primary-color);">Akhil Murali AM</a>
            <div class="hidden md:flex space-x-8">
                <a href="#about" class="nav-link text-gray-600 font-medium">About</a>
                <a href="#dream" class="nav-link text-gray-600 font-medium">My Dream</a>
                <a href="#experience" class="nav-link text-gray-600 font-medium">Experience</a>
                <a href="#projects" class="nav-link text-gray-600 font-medium">Projects</a>
                <a href="#articles" class="nav-link text-gray-600 font-medium">Articles</a>
                <a href="#skills" class="nav-link text-gray-600 font-medium">Skills</a>
                <a href="#contact" class="nav-link text-gray-600 font-medium">Contact</a>
            </div>
            <div class="md:hidden">
                <button id="menu-btn" class="text-gray-600 focus:outline-none">
                    <i class="fas fa-bars fa-lg"></i>
                </button>
            </div>
        </nav>
        <!-- Mobile Menu -->
        <div id="mobile-menu" class="hidden md:hidden">
            <a href="#about" class="block py-2 px-4 text-sm text-gray-700 hover:bg-gray-200">About</a>
            <a href="#dream" class="block py-2 px-4 text-sm text-gray-700 hover:bg-gray-200">My Dream</a>
            <a href="#experience" class="block py-2 px-4 text-sm text-gray-700 hover:bg-gray-200">Experience</a>
            <a href="#projects" class="block py-2 px-4 text-sm text-gray-700 hover:bg-gray-200">Projects</a>
            <a href="#articles" class="block py-2 px-4 text-sm text-gray-700 hover:bg-gray-200">Articles</a>
            <a href="#skills" class="block py-2 px-4 text-sm text-gray-700 hover:bg-gray-200">Skills</a>
            <a href="#contact" class="block py-2 px-4 text-sm text-gray-700 hover:bg-gray-200">Contact</a>
        </div>
    </header>

    <!-- Main Content -->
    <main class="container mx-auto px-6 py-12">

        <!-- Hero Section -->
        <section id="hero" class="text-center py-20 fade-in-section">
            <h1 class="text-6xl font-bold mb-4 uppercase" style="color: var(--primary-color);">Akhil Murali AM</h1>
            <p class="text-xl font-medium mb-6" style="color: var(--secondary-color);">MBA Graduate | Program & Marketing Associate | Professional Social Worker</p>
            <p class="max-w-3xl mx-auto text-lg text-gray-700 mb-8">
                A results-driven professional with a unique blend of business acumen from an MBA and a deep understanding of community needs from a background in social work. Passionate about leveraging data-driven strategies to drive growth, manage impactful projects, and foster strong stakeholder relationships.
            </p>
            <a href="#contact" class="text-white font-bold py-3 px-8 rounded-sm hover:opacity-90 transition-all duration-300" style="background-color: var(--primary-color);">Get In Touch</a>
        </section>

        <!-- About Section -->
        <section id="about" class="py-20 fade-in-section">
            <h2 class="text-4xl font-bold text-center section-title w-max mx-auto">About Me</h2>
            <div class="flex flex-col md:flex-row items-center gap-12 mt-12">
                <div class="md:w-1/3 text-center">
                     <img src="http://googleusercontent.com/file_content/1" alt="Akhil Murali AM" class="rounded-sm mx-auto shadow-xl w-72 h-72 object-cover">
                </div>
                <div class="md:w-2/3">
                    <p class="text-lg mb-4 text-gray-700 leading-relaxed">
                        I am a dedicated and analytical professional with a strong foundation in project management, marketing operations, and client engagement. My experience spans from leading skills development programs for underprivileged youth to conducting in-depth market research for major brands like Amul.
                    </p>
                    <p class="text-lg mb-4 text-gray-700 leading-relaxed">
                        My dual qualifications in Business Administration and Social Work provide me with a unique perspective, allowing me to balance business objectives with social impact. I am adept at managing cross-functional initiatives, executing campaigns, and delivering insights that drive both business and community value. I thrive in fast-paced, client-facing environments where I can apply my skills in strategic thinking and problem-solving.
                    </p>
                </div>
            </div>
        </section>

        <!-- My Dream Section -->
        <section id="dream" class="py-20 bg-[var(--card-bg)] rounded-sm shadow-lg p-8 md:p-12 fade-in-section">
            <h2 class="text-4xl font-bold text-center section-title w-max mx-auto">My Dream</h2>
            <div class="mt-12 text-center">
                <h3 class="text-3xl font-bold mb-4" style="color: var(--primary-color);">Sapiens Consulting</h3>
                <p class="max-w-3xl mx-auto text-lg text-gray-700 mb-8">
                    Sapiens is not merely a consulting firm; we are architects of legacy. We partner with ambitious organizations to build powerful, data-driven strategies that stand the test of time. Our approach marries deep industry knowledge with innovative foresight, turning your vision into a lasting market reality.
                </p>
                <a href="http://sapiens-consulting.lovable.app/" target="_blank" rel="noopener noreferrer" class="text-white font-bold py-3 px-8 rounded-sm hover:opacity-90 transition-all duration-300 inline-block" style="background-color: var(--secondary-color);">
                    Visit Sapiens Consulting <i class="fas fa-external-link-alt ml-2"></i>
                </a>
            </div>
        </section>

        <!-- Experience Section -->
        <section id="experience" class="py-20 fade-in-section">
            <h2 class="text-4xl font-bold text-center section-title w-max mx-auto">Professional Experience</h2>
            <div class="mt-12 bg-[var(--card-bg)] rounded-sm shadow-lg p-8 md:p-12">
                <div class="space-y-12">
                    <!-- DDU GKY Project -->
                    <div class="flex flex-col md:flex-row gap-6">
                        <div class="md:w-1/4">
                            <p class="font-semibold text-lg" style="color: var(--primary-color);">Operations Team Member</p>
                            <p class="text-gray-600 font-medium">DDU GKY Project</p>
                            <p class="text-sm text-gray-500">Jan 2023 - Jun 2024</p>
                        </div>
                        <div class="md:w-3/4 border-l-2 border-gray-200 pl-6">
                            <ul class="list-disc list-inside text-gray-700 space-y-2">
                                <li>Led a skills development program that successfully upskilled over 300 underprivileged students, securing them job placements.</li>
                                <li>Played a pivotal role in securing 50 lakh in government funding by efficiently completing project milestones.</li>
                                <li>Built and maintained strong industry partnerships, significantly enhancing referral networks for placements.</li>
                                <li>Represented the organization in CXO-level meetings, advocating for workforce development and strategic collaborations.</li>
                            </ul>
                        </div>
                    </div>
                    <!-- Learn Wise -->
                    <div class="flex flex-col md:flex-row gap-6">
                        <div class="md:w-1/4">
                            <p class="font-semibold text-lg" style="color: var(--primary-color);">Domain Faculty</p>
                            <p class="text-gray-600 font-medium">Learn Wise</p>
                            <p class="text-sm text-gray-500">Apr 2023 - Jun 2024</p>
                        </div>
                        <div class="md:w-3/4 border-l-2 border-gray-200 pl-6">
                            <ul class="list-disc list-inside text-gray-700 space-y-2">
                                <li>Conducted engaging training sessions for students and professionals on social work methodologies.</li>
                                <li>Facilitated practical workshops on real-world applications of social work principles.</li>
                                <li>Provided mentorship and guidance to learners, assessing progress to enhance their professional development.</li>
                            </ul>
                        </div>
                    </div>
                     <!-- Internships -->
                     <h3 class="text-2xl font-bold pt-8" style="color: var(--primary-color);">Internships</h3>
                     <div class="flex flex-col md:flex-row gap-6">
                        <div class="md:w-1/4">
                            <p class="font-semibold text-lg" style="color: var(--primary-color);">Marketing Intern</p>
                            <p class="text-gray-600 font-medium">GCMMF Ltd. - Amul</p>
                        </div>
                        <div class="md:w-3/4 border-l-2 border-gray-200 pl-6">
                             <p class="text-gray-700">Conducted market research and competitive analysis, performed retail audits, and assisted distributors to enhance supply chain efficiency.</p>
                        </div>
                    </div>
                     <div class="flex flex-col md:flex-row gap-6">
                        <div class="md:w-1/4">
                            <p class="font-semibold text-lg" style="color: var(--primary-color);">HR Intern</p>
                            <p class="text-gray-600 font-medium">Hill Track Construction Pvt.Ltd</p>
                        </div>
                        <div class="md:w-3/4 border-l-2 border-gray-200 pl-6">
                            <p class="text-gray-700">Assisted in daily HR activities and contributed to programs aimed at enhancing laborer satisfaction.</p>
                        </div>
                    </div>
                </div>
            </div>
        </section>
        
        <!-- Education Section -->
        <section id="education" class="py-20 fade-in-section">
            <h2 class="text-4xl font-bold text-center section-title w-max mx-auto">Education</h2>
            <div class="mt-12 grid md:grid-cols-3 gap-8">
                <div class="bg-[var(--card-bg)] p-6 rounded-sm shadow-lg text-center transition-transform transform hover:-translate-y-2 duration-300">
                    <h3 class="font-bold text-xl mb-2" style="color: var(--primary-color);">MBA</h3>
                    <p class="font-medium" style="color: var(--secondary-color);">LEAD College of Management, Palakkad</p>
                    <p class="text-gray-500 text-sm">Completed with high distinction (Sem 1: 88.5%, Sem 2: 81.5%)</p>
                </div>
                <div class="bg-[var(--card-bg)] p-6 rounded-sm shadow-lg text-center transition-transform transform hover:-translate-y-2 duration-300">
                    <h3 class="font-bold text-xl mb-2" style="color: var(--primary-color);">MSW (Master of Social Work)</h3>
                    <p class="font-medium" style="color: var(--secondary-color);">Calicut University Regional Centre, Perambra</p>
                    <p class="text-gray-500 text-sm">Graduated with A+</p>
                </div>
                <div class="bg-[var(--card-bg)] p-6 rounded-sm shadow-lg text-center transition-transform transform hover:-translate-y-2 duration-300">
                    <h3 class="font-bold text-xl mb-2" style="color: var(--primary-color);">BSc. Physics</h3>
                    <p class="font-medium" style="color: var(--secondary-color);">SARBTM Govt College, Koyilandy</p>
                    <p class="text-gray-500 text-sm">Graduated with First Class</p>
                </div>
            </div>
        </section>

        <!-- Projects Section -->
        <section id="projects" class="py-20 bg-[var(--card-bg)] rounded-sm shadow-lg p-8 md:p-12 fade-in-section">
            <h2 class="text-4xl font-bold text-center section-title w-max mx-auto">Key Projects</h2>
            <div class="mt-12 grid md:grid-cols-2 gap-10">
                <div class="border-l-4 pl-6" style="border-color: var(--secondary-color);">
                    <h3 class="font-bold text-xl mb-2" style="color: var(--primary-color);">Analysis of Dairy Products in Q-Comm Platforms</h3>
                    <p class="text-gray-700">A comprehensive market analysis project focusing on the performance and positioning of dairy products within the rapidly growing quick-commerce sector.</p>
                </div>
                <div class="border-l-4 pl-6" style="border-color: var(--secondary-color);">
                    <h3 class="font-bold text-xl mb-2" style="color: var(--primary-color);">Livelihood Impact of Environmental Changes</h3>
                    <p class="text-gray-700">A study on the effect of anthropogenic environmental changes on the livelihood of the rural poor with reference to the Vembanad wetland complex.</p>
                </div>
            </div>
        </section>

        <!-- Articles & Insights Section -->
        <section id="articles" class="py-20 fade-in-section">
            <h2 class="text-4xl font-bold text-center section-title w-max mx-auto">Articles & Insights</h2>
            <div class="mt-12 grid grid-cols-1 md:grid-cols-2 gap-10">
                <!-- Article 1 -->
                <div class="bg-[var(--card-bg)] p-8 rounded-sm shadow-lg flex flex-col">
                    <img src="https://placehold.co/600x400/0A2342/FDFDFB?text=GenAI" alt="AI Meets Imagination Article" class="rounded-sm shadow-md w-full object-cover mb-6">
                    <h3 class="font-bold text-xl mb-3" style="color: var(--primary-color);">AI Meets Imagination: The Next Frontier of Experiential Marketing</h3>
                    <blockquote class="border-l-4 pl-4 italic text-gray-600 my-4 flex-grow" style="border-color: var(--secondary-color);">
                        <p>"GenAI boosts campaign ROI by up to 30%... Experiential strategies increase customer retention by 60%..."</p>
                    </blockquote>
                    <a href="AI Meets Imagination The Next Frontier of Experiential Marketing.pdf" target="_blank" class="font-bold text-white py-2 px-5 rounded-sm inline-block mt-4 hover:opacity-90 transition-opacity duration-300 self-start" style="background-color: var(--primary-color);">Read Full Article &rarr;</a>
                </div>
                <!-- Article 2 -->
                <div class="bg-[var(--card-bg)] p-8 rounded-sm shadow-lg flex flex-col">
                    <img src="https://placehold.co/600x400/2CA58D/FFFFFF?text=Kirana+2.0" alt="Reimagining Kirana Stores Article" class="rounded-sm shadow-md w-full object-cover mb-6">
                    <h3 class="font-bold text-xl mb-3" style="color: var(--primary-color);">Reimagining Kirana Stores: From Corner Shops to Smart Retail Hubs</h3>
                    <blockquote class="border-l-4 pl-4 italic text-gray-600 my-4 flex-grow" style="border-color: var(--secondary-color);">
                        <p>"Kirana 2.0 isn’t just about digitization—it’s about experiences, ecosystems, and evolution."</p>
                    </blockquote>
                    <a href="1751697328847.pdf" target="_blank" class="font-bold text-white py-2 px-5 rounded-sm inline-block mt-4 hover:opacity-90 transition-opacity duration-300 self-start" style="background-color: var(--primary-color);">Read Full Article &rarr;</a>
                </div>
                <!-- Article 3 -->
                <div class="bg-[var(--card-bg)] p-8 rounded-sm shadow-lg flex flex-col">
                    <img src="https://placehold.co/600x400/4a5568/f7fafc?text=Logistics+Hub" alt="Reimagining Logistics in Northeast India Article" class="rounded-sm shadow-md w-full object-cover mb-6">
                    <h3 class="font-bold text-xl mb-3" style="color: var(--primary-color);">Reimagining Logistics in Northeast India: Why Assam is the Next Big Hub!</h3>
                    <blockquote class="border-l-4 pl-4 italic text-gray-600 my-4 flex-grow" style="border-color: var(--secondary-color);">
                        <p>"Assam’s unique location and growing infrastructure position it as a vital corridor for both domestic and international trade."</p>
                    </blockquote>
                    <a href="1751881727528.pdf" target="_blank" class="font-bold text-white py-2 px-5 rounded-sm inline-block mt-4 hover:opacity-90 transition-opacity duration-300 self-start" style="background-color: var(--primary-color);">Read Full Article &rarr;</a>
                </div>
                <!-- Article 4 -->
                 <div class="bg-[var(--card-bg)] p-8 rounded-sm shadow-lg flex flex-col">
                    <img src="https://placehold.co/600x400/8B5CF6/FFFFFF?text=Viral+Science" alt="Going Viral with AI Article" class="rounded-sm shadow-md w-full object-cover mb-6">
                    <h3 class="font-bold text-xl mb-3" style="color: var(--primary-color);">Going Viral with AI: The Science Behind Viral Content Creation</h3>
                    <blockquote class="border-l-4 pl-4 italic text-gray-600 my-4 flex-grow" style="border-color: var(--secondary-color);">
                        <p>"AI transforms viral success from luck to science by leveraging emotional triggers and predictive analytics."</p>
                    </blockquote>
                    <a href="1752854013974.pdf" target="_blank" class="font-bold text-white py-2 px-5 rounded-sm inline-block mt-4 hover:opacity-90 transition-opacity duration-300 self-start" style="background-color: var(--primary-color);">Read Full Article &rarr;</a>
                </div>
            </div>
        </section>

        <!-- Skills & Certifications Section -->
        <section id="skills" class="py-20 fade-in-section">
            <h2 class="text-4xl font-bold text-center section-title w-max mx-auto">Skills & Certifications</h2>
            <div class="mt-12 grid md:grid-cols-2 gap-16">
                <div>
                    <h3 class="text-2xl font-bold mb-8 text-center" style="color: var(--primary-color);">Core Competencies</h3>
                    <div class="flex flex-wrap justify-center gap-3">
                        <span class="bg-gray-200 text-gray-800 text-md font-medium px-4 py-2 rounded-sm">Leadership</span>
                        <span class="bg-gray-200 text-gray-800 text-md font-medium px-4 py-2 rounded-sm">Strategic Thinking</span>
                        <span class="bg-gray-200 text-gray-800 text-md font-medium px-4 py-2 rounded-sm">Project Management</span>
                        <span class="bg-gray-200 text-gray-800 text-md font-medium px-4 py-2 rounded-sm">Communication</span>
                        <span class="bg-gray-200 text-gray-800 text-md font-medium px-4 py-2 rounded-sm">Problem Solving</span>
                        <span class="bg-gray-200 text-gray-800 text-md font-medium px-4 py-2 rounded-sm">Team Work</span>
                        <span class="bg-gray-200 text-gray-800 text-md font-medium px-4 py-2 rounded-sm">Networking</span>
                        <span class="bg-gray-200 text-gray-800 text-md font-medium px-4 py-2 rounded-sm">Financial Management</span>
                    </div>
                </div>
                <div>
                    <h3 class="text-2xl font-bold mb-8 text-center" style="color: var(--primary-color);">Certifications</h3>
                    <div class="flex flex-wrap justify-center gap-3">
                         <span class="font-medium px-4 py-2 rounded-sm" style="background-color: #E3F2FD; color: #1E88E5;">Six Sigma Green Belt</span>
                         <span class="font-medium px-4 py-2 rounded-sm" style="background-color: #E3F2FD; color: #1E88E5;">Zoho Books</span>
                         <span class="font-medium px-4 py-2 rounded-sm" style="background-color: #E3F2FD; color: #1E88E5;">Operations Management</span>
                         <span class="font-medium px-4 py-2 rounded-sm" style="background-color: #E3F2FD; color: #1E88E5;">Product Management</span>
                    </div>
                </div>
            </div>
        </section>

        <!-- Contact Section -->
        <section id="contact" class="py-20 text-white rounded-sm fade-in-section" style="background-color: var(--primary-color);">
            <div class="text-center">
                <h2 class="text-4xl font-bold section-title w-max mx-auto !border-white">Contact Me</h2>
                <p class="text-lg mt-4 mb-8 max-w-xl mx-auto text-gray-300">I'm currently seeking new opportunities and would love to connect. Feel free to reach out via email or connect with me on LinkedIn.</p>
                <div class="flex justify-center items-center space-x-8 text-3xl">
                    <a href="mailto:akhilmuraliambscmsw@gmail.com" class="hover:text-[var(--secondary-color)] transition duration-300" title="Email">
                        <i class="fas fa-envelope"></i>
                    </a>
                    <a href="https://www.linkedin.com/in/akhil-murali-am-10810b249" target="_blank" rel="noopener noreferrer" class="hover:text-[var(--secondary-color)] transition duration-300" title="LinkedIn">
                        <i class="fab fa-linkedin"></i>
                    </a>
                    <a href="tel:+918086081545" class="hover:text-[var(--secondary-color)] transition duration-300" title="Phone">
                        <i class="fas fa-phone"></i>
                    </a>
                </div>
                 <div class="mt-10">
                    <a href="Akhil_Murali_AM_Resume.pdf" download="Akhil_Murali_AM_Resume.pdf" class="bg-white text-[var(--primary-color)] font-bold py-3 px-6 rounded-sm hover:bg-gray-200 transition duration-300">
                        <i class="fas fa-download mr-2"></i>Download Resume
                    </a>
                </div>
            </div>
        </section>

    </main>

    <!-- Footer -->
    <footer class="bg-[var(--card-bg)] text-center py-6">
        <p class="text-gray-600">&copy; 2024 Akhil Murali AM. All Rights Reserved.</p>
    </footer>

    <script>
        // Mobile menu toggle
        const menuBtn = document.getElementById('menu-btn');
        const mobileMenu = document.getElementById('mobile-menu');
        menuBtn.addEventListener('click', () => {
            mobileMenu.classList.toggle('hidden');
        });

        // Scroll Animations
        const sections = document.querySelectorAll('.fade-in-section');
        const observer = new IntersectionObserver(entries => {
            entries.forEach(entry => {
                if (entry.isIntersecting) {
                    entry.target.classList.add('is-visible');
                }
            });
        }, {
            threshold: 0.1
        });

        sections.forEach(section => {
            observer.observe(section);
        });
    </script>

</body>
</html>
