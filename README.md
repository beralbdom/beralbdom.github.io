<!DOCTYPE html>
<html lang="pt-BR">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Bernardo Albuquerque Domingues | Portfólio</title>
    <script src="https://cdn.tailwindcss.com"></script>
    <style>
        /* Using a custom font for a more modern look */
        @import url('https://fonts.googleapis.com/css2?family=Inter:wght@400;500;700&display=swap');
        
        body {
            font-family: 'Inter', sans-serif;
            margin: 0;
            overflow: hidden; /* Prevent main body scrollbars */
            color: #252525;
            background-color: #252525; /* A dark blue background */
        }

        #windyCanvas {
            position: fixed;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            z-index: 0;
        }

        /* This container will hold the content and be scrollable */
        .scroll-container {
            position: relative;
            z-index: 1;
            height: 100vh;
            overflow-y: auto;
            overflow-x: hidden;
            scroll-behavior: smooth;
        }
        
        /* Custom scrollbar for a sleeker look */
        .scroll-container::-webkit-scrollbar {
            width: 8px;
        }
        .scroll-container::-webkit-scrollbar-track {
            background: rgba(10, 10, 20, 0.5);
        }
        .scroll-container::-webkit-scrollbar-thumb {
            background-color: #4a5568;
            border-radius: 10px;
            border: 2px solid transparent;
        }

        /* Animation for sections fading in on scroll */
        .fade-in-section {
            opacity: 0;
            transform: translateY(20px);
            transition: opacity 0.6s ease-out, transform 0.6s ease-out;
        }
        .fade-in-section.is-visible {
            opacity: 1;
            transform: translateY(0);
        }
        
        /* Glassmorphism effect for content cards */
        .card {
            background: rgba(17, 24, 39, 0.75);
            backdrop-filter: blur(12px);
            -webkit-backdrop-filter: blur(12px);
            border: 1px solid rgba(255, 255, 255, 0.1);
        }
    </style>
</head>
<body>

    <canvas id="windyCanvas"></canvas>

    <!-- Scrollable container for the page content -->
    <div class="scroll-container">
        <main class="container mx-auto px-6 py-12 md:py-24">

            <!-- Header Section -->
            <section id="header" class="min-h-screen flex flex-col justify-center items-center text-center">
                <div class="max-w-3xl card rounded-xl p-8">
                    <h1 class="text-4xl md:text-6xl font-bold text-white tracking-tight" style="text-shadow: 2px 2px 4px rgba(0,0,0,0.5);">Bernardo Albuquerque Domingues</h1>
                    <p class="mt-4 text-lg md:text-xl text-cyan-300" style="text-shadow: 1px 1px 2px rgba(0,0,0,0.5);">Engenheiro Eletricista | Mestrando em Engenharia Elétrica na UFF</p>
                    <div class="mt-6 flex flex-wrap justify-center items-center gap-x-4 gap-y-2 text-sm text-gray-200">
                        <span class="flex items-center">
                            <svg class="w-4 h-4 mr-2" fill="currentColor" viewBox="0 0 20 20"><path d="M2 3a1 1 0 011-1h2.153a1 1 0 01.986.836l.74 4.435a1 1 0 01-.54 1.06l-1.518.759a11.03 11.03 0 004.28 4.28l.759-1.518a1 1 0 011.06-.54l4.435.74a1 1 0 01.836.986V17a1 1 0 01-1 1h-2C7.82 18 2 12.18 2 5V3z"></path></svg>
                            (24) 98117-7719
                        </span>
                        <span class="flex items-center">
                            <svg class="w-4 h-4 mr-2" fill="currentColor" viewBox="0 0 20 20"><path d="M2.003 5.884L10 9.882l7.997-3.998A2 2 0 0016 4H4a2 2 0 00-1.997 1.884z"></path><path d="M18 8.118l-8 4-8-4V14a2 2 0 002 2h12a2 2 0 002-2V8.118z"></path></svg>
                            beralbdom@gmail.com
                        </span>
                    </div>
                    <div class="mt-6 flex justify-center space-x-6">
                         <!-- Social links with icons -->
                        <a href="#" class="text-gray-300 hover:text-white transition-colors">LinkedIn</a>
                        <a href="#" class="text-gray-300 hover:text-white transition-colors">GitHub</a>
                        <a href="#" class="text-gray-300 hover:text-white transition-colors">Lattes</a>
                    </div>
                </div>
            </section>

            <!-- Professional Experience Section -->
            <section id="experience" class="py-16 md:py-20 fade-in-section">
                <h2 class="text-3xl font-bold text-white mb-8 text-center" style="text-shadow: 2px 2px 4px rgba(0,0,0,0.7);">Experiência Profissional</h2>
                <div class="max-w-4xl mx-auto space-y-8">
                    <div class="card rounded-lg p-6">
                        <h3 class="text-xl font-bold text-cyan-300">Empresa de Pesquisa Energética - Estágio</h3>
                        <p class="text-sm text-gray-400">Superintendência de Geração de Energia (DEE/SGR)</p>
                        <ul class="mt-4 list-disc list-inside text-gray-300 space-y-2">
                            <li>Análise de dados e séries temporais (Python, SQL, R, Excel).</li>
                            <li>Aplicação de métodos estatísticos, clusterização e modelos de regressão e classificação.</li>
                            <li>Automatização de consultas ao AEGE durante leilões de energia.</li>
                            <li>Modelagem de geração eólica a partir de dados climáticos e do sistema AMA.</li>
                            <li>Co-autoria de artigo sobre competitividade da fonte eólica em cenários de PLD.</li>
                        </ul>
                    </div>
                    <div class="card rounded-lg p-6">
                        <h3 class="text-xl font-bold text-cyan-300">Siemens Healthcare - Estágio</h3>
                        <p class="text-sm text-gray-400">Engenharia de Campo</p>
                        <ul class="mt-4 list-disc list-inside text-gray-300 space-y-2">
                            <li>Automatização de processos utilizando Python, SAP e Excel/VBA.</li>
                            <li>Acompanhamento e controle de KPIs para otimização de performance.</li>
                        </ul>
                    </div>
                </div>
            </section>

            <!-- Academic Education Section -->
            <section id="education" class="py-16 md:py-20 fade-in-section">
                <h2 class="text-3xl font-bold text-white mb-8 text-center" style="text-shadow: 2px 2px 4px rgba(0,0,0,0.7);">Formação Acadêmica</h2>
                <div class="max-w-4xl mx-auto space-y-8">
                    <div class="card rounded-lg p-6">
                        <h3 class="text-xl font-bold text-cyan-300">Mestrado em Engenharia Elétrica</h3>
                        <p class="text-gray-300">Universidade Federal Fluminense (UFF)</p>
                        <p class="text-sm text-gray-400">2024 - 2025 | Modelagem de Sistemas Elétricos</p>
                    </div>
                    <div class="card rounded-lg p-6">
                        <h3 class="text-xl font-bold text-cyan-300">Graduação em Engenharia Elétrica</h3>
                        <p class="text-gray-300">Universidade Federal Fluminense (UFF)</p>
                        <p class="text-sm text-gray-400">2017 - 2025 | Sistemas de Energia Elétrica e Renováveis</p>
                    </div>
                </div>
            </section>

            <!-- Skills Section -->
            <section id="skills" class="py-16 md:py-20 fade-in-section">
                <h2 class="text-3xl font-bold text-white mb-8 text-center" style="text-shadow: 2px 2px 4px rgba(0,0,0,0.7);">Habilidades</h2>
                <div class="max-w-5xl mx-auto grid grid-cols-2 md:grid-cols-4 gap-6 text-center">
                    <div class="card rounded-lg p-4">
                        <h4 class="font-bold text-lg text-cyan-300">Programação</h4>
                        <p class="text-gray-300 text-sm">Python, C/C++, R, VBA</p>
                    </div>
                    <div class="card rounded-lg p-4">
                        <h4 class="font-bold text-lg text-cyan-300">Análise de Dados</h4>
                        <p class="text-gray-300 text-sm">Pandas, Scikit-learn, TensorFlow, Keras</p>
                    </div>
                    <div class="card rounded-lg p-4">
                        <h4 class="font-bold text-lg text-cyan-300">Banco de Dados</h4>
                        <p class="text-gray-300 text-sm">SQL</p>
                    </div>
                    <div class="card rounded-lg p-4">
                        <h4 class="font-bold text-lg text-cyan-300">DevOps</h4>
                        <p class="text-gray-300 text-sm">Git, GitHub, Azure DevOps</p>
                    </div>
                </div>
            </section>
            
            <footer class="text-center py-8 text-gray-200 text-sm fade-in-section" style="text-shadow: 1px 1px 2px rgba(0,0,0,0.7);">
                <p>&copy; 2025 Bernardo Albuquerque Domingues. Design por Gemini.</p>
            </footer>

        </main>
    </div>

    <script>
        // --- Wind Particle Animation ---
        const canvas = document.getElementById('windyCanvas');
        const ctx = canvas.getContext('2d');
        canvas.width = window.innerWidth;
        canvas.height = window.innerHeight;
        let particlesArray;

        window.addEventListener('resize', () => {
            canvas.width = window.innerWidth;
            canvas.height = window.innerHeight;
            init();
        });

        class Particle {
            constructor(x, y) {
                this.x = x;
                this.y = y;
                this.size = .5; // Set particle size to 1px
                this.speedX = (Math.random() * 0.5) + 0.1; // Base horizontal speed
                this.angle = Math.random() * Math.PI * 2; // Starting angle for the whirl
                this.angleSpeed = Math.random() * 0.04 + 0.01; // How fast it whirls
                this.amplitude = 0; // How wide the whirl is
                this.hue = (this.x / canvas.width) * 360; // Color based on X position
            }
            update() {
                // Move horizontally
                this.x += this.speedX;
                
                // Create the vertical whirl effect using a sine wave
                this.y += Math.sin(this.angle) * this.amplitude;
                
                // Increment the angle for the next frame's sine value
                this.angle += this.angleSpeed;

                // Update hue based on new position to create the gradient effect
                this.hue = (this.x / canvas.width) * 360;

                // Reset particle when it goes off the right side of the screen
                if (this.x > canvas.width + this.size) {
                    this.x = -this.size;
                    this.y = Math.random() * canvas.height;
                }
                // Reset particle if it whirls too far off the top or bottom
                if (this.y > canvas.height + this.size || this.y < -this.size) {
                    this.x = -this.size;
                    this.y = Math.random() * canvas.height;
                }
            }
            draw() {
                // Use HSL for vibrant, position-based color
                ctx.fillStyle = `hsl(${this.hue}, 100%, 70%)`;
                ctx.beginPath();
                ctx.arc(this.x, this.y, this.size, 0, Math.PI * 2);
                ctx.fill();
            }
        }

        function init() {
            particlesArray = [];
            // Significantly increased particle density
            const numberOfParticles = (canvas.width * canvas.height) / 200;
            for (let i = 0; i < numberOfParticles; i++) {
                const x = Math.random() * canvas.width;
                const y = Math.random() * canvas.height;
                particlesArray.push(new Particle(x, y));
            }
        }

        function animate() {
            // Lower alpha value for even longer trails
            ctx.fillStyle = 'rgba(25, 25, 25, 0.02)';
            ctx.fillRect(0, 0, canvas.width, canvas.height);

            for (let i = 0; i < particlesArray.length; i++) {
                particlesArray[i].update();
                particlesArray[i].draw();
            }
            requestAnimationFrame(animate);
        }

        init();
        animate();

        // --- Scroll Animation Logic ---
        const sections = document.querySelectorAll('.fade-in-section');
        const scrollContainer = document.querySelector('.scroll-container');

        const sectionObserver = new IntersectionObserver((entries, observer) => {
            entries.forEach(entry => {
                if (entry.isIntersecting) {
                    entry.target.classList.add('is-visible');
                }
            });
        }, {
            root: scrollContainer,
            threshold: 0.1
        });

        const headerSection = document.querySelector('#header');
        if (headerSection) {
            setTimeout(() => {
                headerSection.querySelector('.card').classList.add('is-visible');
            }, 100);
        }
        
        const headerCard = document.querySelector('#header .card');
        if(headerCard) {
            headerCard.classList.add('fade-in-section');
        }

        sections.forEach(section => {
            sectionObserver.observe(section);
        });

    </script>
</body>
</html>
