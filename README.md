<!DOCTYPE html>
<html lang="fr">

<head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>Mon Portfolio</title>

    <link rel ="stylesheet" href="./Style/style.css"/>
</head>

<body>
<!DOCTYPE html>
<html lang="fr">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>AMINE KHALIT - Portfolio Scientifique</title>
    <style>
        @keyframes scrollText {
            0% { transform: translateX(100%); }
            100% { transform: translateX(-100%); }
        }
        
        @keyframes blink {
            0%, 100% { opacity: 1; }
            50% { opacity: 0; }
        }
        
        @keyframes particlePulse {
            0% { transform: scale(0.8); opacity: 0; }
            50% { transform: scale(1.2); opacity: 1; }
            100% { transform: scale(0.8); opacity: 0; }
        }
        
        @keyframes quantumSpin {
            from { transform: rotate(0deg); }
            to { transform: rotate(360deg); }
        }
        
        @keyframes float {
            0%, 100% { transform: translateY(0); }
            50% { transform: translateY(-10px); }
        }
        
        .quantum-dot {
            position: absolute;
            width: 4px;
            height: 4px;
            border-radius: 50%;
            background: #64f0ff;
            animation: particlePulse 3s infinite ease-in-out;
            box-shadow: 0 0 8px #64f0ff;
        }
        
        body {
            margin: 0;
            font-family: 'Segoe UI', system-ui, sans-serif;
            overflow-x: hidden;
        }
    </style>
</head>
<body>
    <!-- En-tête cyber-scientifique avec système de particules interactives -->
    <header style="display: flex; flex-direction: column; align-items: center; justify-content: center; text-align: center; padding: 80px 20px; background: linear-gradient(rgba(10, 25, 47, 0.9), rgba(33, 150, 243, 0.7)), url('https://images.unsplash.com/photo-1639762681057-408e52192e55?ixlib=rb-4.0.3&auto=format&fit=crop&w=1950&q=80') center/cover no-repeat; color: white; position: relative; overflow: hidden; height: 100vh;">

        <!-- Système de particules quantiques (canvas interactif) -->
        <canvas id="quantumParticles" style="position: absolute; top: 0; left: 0; width: 100%; height: 100%; z-index: 0; pointer-events: none;"></canvas>
        
        <!-- Effet d'intrication quantique (particules connectées) -->
        <svg id="quantumConnections" style="position: absolute; top: 0; left: 0; width: 100%; height: 100%; z-index: 1; pointer-events: none;"></svg>
        
        <!-- Points quantiques lumineux -->
        <div id="quantumDots" style="position: absolute; top: 0; left: 0; width: 100%; height: 100%; z-index: 1; pointer-events: none;"></div>
        
        <!-- Titre avec effet de diffraction lumineuse -->
        <h1 style="font-size: clamp(2.5rem, 5vw, 3.5rem); margin: 0; z-index: 2; 
            background: linear-gradient(90deg, #64f0ff, #2196f3, #3d5afe);
            -webkit-background-clip: text;
            background-clip: text;
            color: transparent;
            text-shadow: 0 0 12px rgba(100, 240, 255, 0.4);
            position: relative;
            animation: float 4s ease-in-out infinite;">
            AMINE KHALIT
            <!-- Effet de particules émanant du texte -->
            <div class="particle-emitter" style="position: absolute; top: 50%; left: 0; width: 100%; height: 2px; background: transparent; z-index: -1;"></div>
        </h1>
        
        <!-- Sous-titre avec effet terminal -->
        <p style="font-size: clamp(1rem, 2vw, 1.3rem); margin: 15px 0 25px; z-index: 2; font-family: 'Courier New', monospace; position: relative;">
            <span id="typingEffect" style="border-right: 2px solid #64f0ff; animation: blink 0.7s infinite;"></span>
        </p>
        
        <!-- Badge d'état quantique -->
        <div style="margin-top: 25px; z-index: 2; padding: 12px 24px; border-radius: 24px; 
            background: rgba(33, 150, 243, 0.15); border: 1px solid rgba(100, 240, 255, 0.4);
            box-shadow: 0 0 15px rgba(100, 240, 255, 0.2);
            position: relative;
            overflow: hidden;
            backdrop-filter: blur(5px);">
            <code style="color: #64f0ff; font-size: clamp(0.9rem, 1.5vw, 1.1rem);">public class Scientist implements Researcher, Developer {}</code>
            <!-- Particules en orbite autour du badge -->
            <div class="orbiting-particles" style="position: absolute; top: 0; left: 0; width: 100%; height: 100%;"></div>
        </div>
        
        <!-- Réseau de connaissances animé -->
        <div class="knowledge-network" style="position: absolute; bottom: 30px; width: 80%; height: 60px; z-index: 2;">
            <svg viewBox="0 0 800 60" style="width: 100%; height: 100%;">
                <path id="pulseWave" stroke="rgba(100, 240, 255, 0.7)" stroke-width="2" fill="none" 
                      stroke-dasharray="10 5" style="filter: drop-shadow(0 0 5px rgba(100, 240, 255, 0.5));"></path>
            </svg>
        </div>

        <!-- Tags scientifiques animés -->
        <div class="animated-text" style="position: absolute; bottom: 100px; width: 90%; z-index: 1; overflow: hidden;">
            <div style="display: inline-block; animation: scrollText 20s linear infinite; white-space: nowrap;">
                <span style="display: inline-block; margin: 0 15px; color: rgba(100, 240, 255, 0.8);">[Machine Learning]</span>
                <span style="display: inline-block; margin: 0 15px; color: rgba(100, 240, 255, 0.8);">[Théorie des Graphes]</span>
                <span style="display: inline-block; margin: 0 15px; color: rgba(100, 240, 255, 0.8);">[Algorithmes Quantiques]</span>
                <span style="display: inline-block; margin: 0 15px; color: rgba(100, 240, 255, 0.8);">[Topologie Algébrique]</span>
                <span style="display: inline-block; margin: 0 15px; color: rgba(100, 240, 255, 0.8);">[Neural Networks]</span>
                <span style="display: inline-block; margin: 0 15px; color: rgba(100, 240, 255, 0.8);">[Optimisation Combinatoire]</span>
            </div>
        </div>
    </header>

    <script>
        document.addEventListener('DOMContentLoaded', function() {
            initQuantumParticles();
            initTypingEffect();
            initPulseNetwork();
            createQuantumDots();
            initOrbitingParticles();
        });
        
        // Système de particules quantiques
        function initQuantumParticles() {
            const canvas = document.getElementById('quantumParticles');
            const ctx = canvas.getContext('2d');
            canvas.width = window.innerWidth;
            canvas.height = window.innerHeight;
            
            const particles = [];
            const particleCount = Math.floor(window.innerWidth / 10);
            
            for (let i = 0; i < particleCount; i++) {
                particles.push({
                    x: Math.random() * canvas.width,
                    y: Math.random() * canvas.height,
                    size: Math.random() * 2 + 1,
                    speedX: Math.random() * 0.5 - 0.25,
                    speedY: Math.random() * 0.5 - 0.25,
                    color: `rgba(100, 240, 255, ${Math.random() * 0.5 + 0.1})`
                });
            }
            
            function animateParticles() {
                ctx.clearRect(0, 0, canvas.width, canvas.height);
                
                for (let i = 0; i < particles.length; i++) {
                    const p = particles[i];
                    
                    ctx.beginPath();
                    ctx.arc(p.x, p.y, p.size, 0, Math.PI * 2);
                    ctx.fillStyle = p.color;
                    ctx.fill();
                    
                    p.x += p.speedX;
                    p.y += p.speedY;
                    
                    if (p.x < 0 || p.x > canvas.width) p.speedX *= -1;
                    if (p.y < 0 || p.y > canvas.height) p.speedY *= -1;
                }
                
                requestAnimationFrame(animateParticles);
            }
            
            animateParticles();
            
            window.addEventListener('resize', function() {
                canvas.width = window.innerWidth;
                canvas.height = window.innerHeight;
            });
        }
        
        // Effet de frappe au clavier
        function initTypingEffect() {
            const textElement = document.getElementById('typingEffect');
            const phrases = [
                "Mathématiques Discrètes • Informatique Théorique",
                "Complexité Algorithmique • Intelligence Artificielle",
                "∀x ∈ {Science, Code} • Passion(x) ∧ Research(x)"
            ];
            let phraseIndex = 0;
            let charIndex = 0;
            let isDeleting = false;
            let typingSpeed = 100;
            
            function type() {
                const currentPhrase = phrases[phraseIndex];
                
                if (isDeleting) {
                    textElement.textContent = currentPhrase.substring(0, charIndex - 1);
                    charIndex--;
                    typingSpeed = 50;
                } else {
                    textElement.textContent = currentPhrase.substring(0, charIndex + 1);
                    charIndex++;
                    typingSpeed = 100;
                }
                
                if (!isDeleting && charIndex === currentPhrase.length) {
                    isDeleting = true;
                    typingSpeed = 1500;
                } else if (isDeleting && charIndex === 0) {
                    isDeleting = false;
                    phraseIndex = (phraseIndex + 1) % phrases.length;
                    typingSpeed = 500;
                }
                
                setTimeout(type, typingSpeed);
            }
            
            setTimeout(type, 1000);
        }
        
        // Réseau pulsant
        function initPulseNetwork() {
            const pulseWave = document.getElementById('pulseWave');
            const points = [];
            const width = 800;
            const height = 60;
            
            for (let x = 0; x <= width; x += 20) {
                points.push({
                    x: x,
                    y: height / 2 + Math.sin(x / 50) * 20
                });
            }
            
            let offset = 0;
            
            function animateWave() {
                let pathData = `M ${points[0].x} ${points[0].y + Math.sin(offset) * 5}`;
                
                for (let i = 1; i < points.length; i++) {
                    pathData += ` L ${points[i].x} ${points[i].y + Math.sin(offset + i * 0.2) * 5}`;
                }
                
                pulseWave.setAttribute('d', pathData);
                offset += 0.05;
                
                requestAnimationFrame(animateWave);
            }
            
            animateWave();
        }
        
        // Points quantiques aléatoires
        function createQuantumDots() {
            const container = document.getElementById('quantumDots');
            const dotCount = 30;
            
            for (let i = 0; i < dotCount; i++) {
                const dot = document.createElement('div');
                dot.className = 'quantum-dot';
                dot.style.left = `${Math.random() * 100}%`;
                dot.style.top = `${Math.random() * 100}%`;
                dot.style.animationDelay = `${Math.random() * 3}s`;
                container.appendChild(dot);
            }
        }
        
        // Particules en orbite
        function initOrbitingParticles() {
            const badges = document.querySelectorAll('.orbiting-particles');
            
            badges.forEach(badge => {
                const particleCount = 8;
                const radius = 40;
                
                for (let i = 0; i < particleCount; i++) {
                    const particle = document.createElement('div');
                    particle.style.position = 'absolute';
                    particle.style.width = '6px';
                    particle.style.height = '6px';
                    particle.style.borderRadius = '50%';
                    particle.style.background = 'rgba(100, 240, 255, 0.7)';
                    particle.style.boxShadow = '0 0 8px #64f0ff';
                    
                    const angle = (i * (2 * Math.PI / particleCount));
                    const x = 50 + radius * Math.cos(angle);
                    const y = 50 + radius * Math.sin(angle);
                    
                    particle.style.left = `calc(${x}% - 3px)`;
                    particle.style.top = `calc(${y}% - 3px)`;
                    particle.style.animation = `quantumSpin ${10 + i}s linear infinite`;
                    
                    badge.appendChild(particle);
                }
            });
        }
    </script>
</body>
</html>

<!-- Animation CSS pour le texte déroulant -->
<style>
@keyframes scrollText {
    0% { transform: translateX(100%); }
    100% { transform: translateX(-100%); }
}
</style>


    <style>
        @keyframes scrollText {
            0% {
                transform: translateX(100%);
            }
            100% {
                transform: translateX(-100%);
            }
        }
    </style>
</header>




    <!-- Sidebar Ouverture et fermeture-->
    <aside id="sidebar" style="position: fixed; top: 0; left: 0; height: 100%; width: 300px; background: linear-gradient(135deg, #343a40, #212529); color: white; padding: 20px; box-shadow: 3px 0 10px rgba(0, 0, 0, 0.3); z-index: 1000; display: flex; flex-direction: column; align-items: center; transition: transform 0.3s;">
        <div style="text-align: center; margin-bottom: 30px;">
            <img src="./Images/Photo.png" alt="Photo de profil" style="width: 100px; height: 100px; border-radius: 50%; border: 3px solid #f8f9fa; margin-bottom: 10px;">
            <h2 style="font-size: 1.5rem; margin: 0; color: #f8f9fa;">KHALIT AMINE </h2>
            <p style="font-size: 0.9rem; color: #adb5bd;">Étudiant en Mathématiques-Informatique</p>
        </div>
        <nav style="width: 100%;">
            <ul style="list-style: none; padding: 0; margin: 0; width: 100%;">
                <li style="margin-bottom: 15px;">
                    <a href="#about" style="text-decoration: none; color: #f8f9fa; font-size: 1.1rem; display: flex; align-items: center; padding: 10px; border-radius: 5px; transition: background-color 0.3s;">
                        <span style="margin-right: 10px; font-size: 1.2rem;">🏠</span> Accueil
                    </a>
                </li>
                <li style="margin-bottom: 15px;">
                    <a href="#Parcours" style="text-decoration: none; color: #f8f9fa; font-size: 1.1rem; display: flex; align-items: center; padding: 10px; border-radius: 5px; transition: background-color 0.3s;">
                        <span style="margin-right: 10px; font-size: 1.2rem;">📚</span> Parcours
                    </a>
                </li>
                <li style="margin-bottom: 15px;">
                    <a href="#skills" style="text-decoration: none; color: #f8f9fa; font-size: 1.1rem; display: flex; align-items: center; padding: 10px; border-radius: 5px; transition: background-color 0.3s;">
                        <span style="margin-right: 10px; font-size: 1.2rem;">💻</span> Compétences
                    </a>
                </li>
                <li style="margin-bottom: 15px;">
                    <a href="#Certifications" style="text-decoration: none; color: #f8f9fa; font-size: 1.1rem; display: flex; align-items: center; padding: 10px; border-radius: 5px; transition: background-color 0.3s;">
                        <span style="margin-right: 10px; font-size: 1.2rem;">🏆</span> Certifications
                    </a>
                </li>
                <li style="margin-bottom: 15px;">
                    <a href="#contact" style="text-decoration: none; color: #f8f9fa; font-size: 1.1rem; display: flex; align-items: center; padding: 10px; border-radius: 5px; transition: background-color 0.3s;">
                        <span style="margin-right: 10px; font-size: 1.2rem;">✉️</span> Contact
                    </a>
                </li>
            </ul>
        </nav>
        <div style="margin-top: auto; text-align: center; color: #adb5bd; font-size: 0.9rem;">
            <p>© 2025 AMINE KHALIT IBRAHIM</p>
            <p>Tous droits réservés</p>
        </div>
    </aside>

    

    <!-- Section À propos -->
    <section id="about">
        <h2>À propos de moi</h2>
        <div style="text-align: center; max-width: 800px; margin: 0 auto;">
            <p>
                Je suis un étudiant passionné par les mathématiques et l'informatique,
                avec une solide formation en algorithmique et en programmation.
                Mon objectif est de mettre mes compétences au service de projets innovants et stimulants.
            </p> 
            <p>
                Fort d'une solide formation en Bases de données(SQL), en algorithmique et en programmation (Python,
                Java, R, C)
                acquise lors de mes études en Licence Mathématiques et Informatique,
                je maîtrise également les bases du développement web (HTML, CSS, JavaScript). Mes certifications
                récentes en
                Introduction to Python, Python Intermediate, Java Intermediate, et Introduction to Java (Sololearn)
                attestent de mon engagement à approfondir ces compétences.


            </p>
        </div>
    </section>

    <!-- Section Parcours -->
    <section id="Parcours">
        <h2>Parcours</h2>
        <div style="text-align: center; max-width: 800px; margin: 0 auto;">
            <p>Mon parcours académique reflète une progression constante dans le domaine des mathématiques et de l'informatique :</p>
            <ul>
            <li>Licence en Mathématiques et Applications à l'<strong>Université de Paris Cité</strong> (2024 - 2025)</li>
            <li>Licence en Mathématiques et Informatique à l'<strong>Université de Toulouse</strong> (2023 - 2024)</li>
            <li>Certificat Universitaire à l'<strong>Université de Lille</strong> (2022 - 2023)</li>
            </ul>
            <p>En parallèle, j'ai enrichi mes compétences grâce à diverses certifications :</p>
            <ul>
            <li>Certifications en programmation sur <strong>Sololearn</strong> et <strong>Kaggle</strong> :
                <ul>
                <li><em>Python</em> (Introduction, niveau intermédiaire)</li>
                <li><em>Java</em> (Introduction, niveau intermédiaire)</li>
                </ul>
            </li>
            <li>Séminaire en leadership et gestion de projet organisé par le <strong>CANTIC Center</strong></li>
            </ul>
        </div>
        </section>

    <!-- Section Compétences -->
    <section id="skills">
        <h2>Mes Compétences</h2>
        <div class="skills-container" style="display: flex; justify-content: space-around; gap: 20px; flex-wrap: wrap; max-width: 1200px; margin: 0 auto;">
            <div class="skill-card" style="text-align: center; flex: 1; min-width: 200px;">
                <div class="skill-icon" style="font-size: 2rem;">💻</div>
                <h3>Développement Web</h3>
                <p>HTML, CSS, JavaScript</p>
            </div>
            <div class="skill-card" style="text-align: center; flex: 1; min-width: 200px;">
                <div class="skill-icon" style="font-size: 2rem;">📊</div>
                <h3>Data Science</h3>
                <p>Octave, Python, Pandas, NumPy, Matplotlib</p>
            </div>
            <div class="skill-card" style="text-align: center; flex: 1; min-width: 200px;">
                <div class="skill-icon" style="font-size: 2rem;">🔢</div>
                <h3>Mathématiques</h3>
                <p>Algèbre, Analyse, Probabilités, Statistiques</p>
            </div>
            <div class="skill-card" style="text-align: center; flex: 1; min-width: 200px;">
                <div class="skill-icon" style="font-size: 2rem;">🗄️</div>
                <h3>Bases de données</h3>
                <p>SQL, MySQL, Adminer</p>
            </div>
        </div>
    </section>

    <!-- Section Certifications -->
    <section id="Certifications">
        <h2>Mes Certifications</h2>
        <div class="certifications-grid" style="display: flex; justify-content: space-around; gap: 20px; flex-wrap: wrap; max-width: 1200px; margin: 0 auto;">
            <div class="certification-card" style="text-align: center; flex: 1; min-width: 200px;">
                <iframe src="./Images/Python_Intermediate.pdf" style="width: 100%; height: 400px; border: none;"></iframe>
                <h3>Python Intermediate</h3>
                <p>Certification obtenue sur Sololearn</p>
            </div>
            <div class="certification-card" style="text-align: center; flex: 1; min-width: 200px;">
                <iframe src="./Images/Java Intermediate.pdf" style="width: 100%; height: 400px; border: none;"></iframe>
                <h3>Java Intermediate</h3>
                <p>Certification obtenue sur Sololearn</p>
            </div>
            <div class="certification-card" style="text-align: center; flex: 1; min-width: 200px;">
                <iframe src="./Images/CANTIC_certificat de participation.pdf" style="width: 100%; height: 400px; border: none;"></iframe>
                <h3>Leadership et Gestion de Projet</h3>
                <p>Séminaire organisé par le CANTIC Center</p>
            </div>
            <div class="certification-card" style="text-align: center; flex: 1; min-width: 200px;">
                <iframe src="./Images/Coding Foundations.pdf" style="width: 100%; height: 400px; border: none;"></iframe>
                <h3>Coding Foundations</h3>
                <p>Certification obtenue sur Sololearn</p>
            </div>
        </div>
    </section>
    
    <!-- Section Contact -->
    <section id="contact" style="text-align: center;">
        <h2>Contactez-moi</h2>
        <form class="contact-form" action="mailto:khalit-ibrahim.amine@etu.u-paris.fr?subject=Contact%20Form&body=Nom:%20[Nom]%0AEmail:%20[Email]%0AMessage:%20[Message]" method="post" enctype="text/plain" onsubmit="return confirm('Votre message a été envoyé avec succès !')" style="max-width: 600px; margin: 0 auto; text-align: left;">
            <div class="form-group" style="margin-bottom: 15px;">
                <label for="name" style="display: block; font-weight: bold;">Nom</label>
                <input type="text" id="name" name="name" placeholder="Votre nom" required style="width: 100%; padding: 10px; border: 1px solid #ccc; border-radius: 5px;" />
            </div>
            <div class="form-group" style="margin-bottom: 15px;">
                <label for="email" style="display: block; font-weight: bold;">Email</label>
                <input type="email" id="email" name="email" placeholder="Votre email" required style="width: 100%; padding: 10px; border: 1px solid #ccc; border-radius: 5px;" />
            </div>
            <div class="form-group" style="margin-bottom: 15px;">
                <label for="message" style="display: block; font-weight: bold;">Message</label>
                <textarea id="message" name="message" rows="5" placeholder="Votre message" required style="width: 100%; padding: 10px; border: 1px solid #ccc; border-radius: 5px;"></textarea>
            </div>
                <div style="text-align: right;">
                    <button type="submit" class="submit-btn" style="background-color: #007BFF; color: white; padding: 10px 20px; border: none; border-radius: 5px; cursor: pointer;">Envoyer</button>
                </div>
            </form>
        </form>
    </section>


    <!-- Section Réseaux Sociaux -->
    <footer style="text-align: center; padding: 20px; background-color: #f8f9fa; margin-top: 20px;">
        <h3>Retrouvez-moi sur</h3>
        <div style="display: flex; justify-content: center; gap: 20px; margin-top: 10px;">
            <a href="https://www.linkedin.com/in/amine-khalit-ibrahim" target="_blank" style="text-decoration: none; color: #0077B5; font-size: 1.5rem;">
                <img src="https://cdn-icons-png.flaticon.com/512/174/174857.png" alt="LinkedIn" style="width: 40px; height: 40px; vertical-align: middle;"> LinkedIn
            </a>
            <a href="mailto:khalit-ibrahim.amine@etu.u-paris.fr" style="text-decoration: none; color: #D44638; font-size: 1.5rem;">
                <img src="https://cdn-icons-png.flaticon.com/512/732/732200.png" alt="Email" style="width: 40px; height: 40px; vertical-align: middle;"> Email
            </a>
            <a href="https://wa.me/33748276867" target="_blank" style="text-decoration: none; color: #25D366; font-size: 1.5rem;">
                <img src="https://cdn-icons-png.flaticon.com/512/733/733585.png" alt="WhatsApp" style="width: 40px; height: 40px; vertical-align: middle;"> WhatsApp
            </a>
        </div>
    </footer>

    <script src="./Script/script.js"></script>
</body>

</html>
