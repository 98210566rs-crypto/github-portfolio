<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Ravi Kumar Sharma | CS Portfolio</title>
    <style>
        :root {
            --primary: #6366f1;
            --secondary: #a855f7;
            --bg: #0f172a;
            --card: #1e293b;
            --text: #f8fafc;
            --dim: #94a3b8;
        }

        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: 'Inter', system-ui, sans-serif;
        }

        body {
            background-color: var(--bg);
            color: var(--text);
            overflow-x: hidden;
            scroll-behavior: smooth;
        }

        /* Animated Background Gradient */
        .bg-glow {
            position: fixed;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            background: radial-gradient(circle at 50% 50%, #1e1b4b 0%, #0f172a 100%);
            z-index: -1;
        }

        .container {
            max-width: 1000px;
            margin: 0 auto;
            padding: 2rem;
        }

        /* Header & Nav */
        header {
            height: 60vh;
            display: flex;
            flex-direction: column;
            justify-content: center;
            align-items: center;
            text-align: center;
            animation: fadeIn 1s ease-in;
        }

        h1 {
            font-size: 3.5rem;
            margin-bottom: 0.5rem;
            background: linear-gradient(to right, var(--primary), var(--secondary));
            -webkit-background-clip: text;
            -webkit-fill-color: transparent;
            color: transparent;
        }

        /* Section Styling */
        section {
            margin: 4rem 0;
            opacity: 0;
            transform: translateY(20px);
            transition: all 0.6s ease-out;
        }

        section.visible {
            opacity: 1;
            transform: translateY(0);
        }

        .card {
            background: var(--card);
            padding: 2rem;
            border-radius: 1rem;
            border: 1px solid rgba(255,255,255,0.1);
            box-shadow: 0 10px 30px rgba(0,0,0,0.3);
        }

        /* Skills Chips */
        .skills-container {
            display: flex;
            flex-wrap: wrap;
            gap: 10px;
            margin-top: 1rem;
        }

        .skill-chip {
            background: rgba(99, 102, 241, 0.1);
            border: 1px solid var(--primary);
            color: var(--primary);
            padding: 5px 15px;
            border-radius: 20px;
            font-size: 0.9rem;
            transition: 0.3s;
            cursor: default;
        }

        .skill-chip:hover {
            background: var(--primary);
            color: white;
        }

        /* Project Cards */
        .project-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 20px;
        }

        .project-card {
            background: #1e293b;
            border-radius: 10px;
            padding: 1.5rem;
            border-bottom: 4px solid var(--primary);
            transition: 0.3s;
        }

        .project-card:hover {
            transform: scale(1.03);
            background: #2d3748;
        }

        /* Interactive Counter Section */
        .stats {
            display: flex;
            justify-content: space-around;
            text-align: center;
            margin: 2rem 0;
        }

        .stat-item h3 { font-size: 2rem; color: var(--secondary); }

        @keyframes fadeIn {
            from { opacity: 0; }
            to { opacity: 1; }
        }

        .cta-button {
            background: var(--primary);
            color: white;
            padding: 12px 30px;
            border-radius: 30px;
            text-decoration: none;
            font-weight: 600;
            margin-top: 20px;
            display: inline-block;
            transition: 0.3s;
        }

        .cta-button:hover {
            box-shadow: 0 0 20px var(--primary);
        }
    </style>
</head>
<body>

    <div class="bg-glow"></div>

    <div class="container">
        <header>
            <h1 id="typing-text">Ravi Kumar Sharma</h1>
            <p style="color: var(--dim); font-size: 1.2rem;">Final Year B.Tech CSE Student @ Sharda University</p>
            <a href="mailto:ravi@email.com" class="cta-button">Hire Me</a>
        </header>

        <section id="about" class="card">
            <h2>About Me</h2>
            <p style="margin-top: 10px; color: var(--dim);">
                Specializing in Full-Stack Development and IoT. I bridge the gap between complex C++ algorithms and user-friendly web interfaces. Currently preparing for GATE 2026.
            </p>
            <div class="stats">
                <div class="stat-item">
                    <h3 class="counter" data-target="15">0</h3>
                    <p>Projects</p>
                </div>
                <div class="stat-item">
                    <h3 class="counter" data-target="4">0</h3>
                    <p>Year Student</p>
                </div>
            </div>
        </section>

        <section id="skills">
            <h2>Technical Stack</h2>
            <div class="skills-container">
                <span class="skill-chip">C++</span>
                <span class="skill-chip">Data Structures</span>
                <span class="skill-chip">React.js</span>
                <span class="skill-chip">Next.js</span>
                <span class="skill-chip">Firebase</span>
                <span class="skill-chip">SQL</span>
                <span class="skill-chip">IoT</span>
                <span class="skill-chip">Git</span>
            </div>
        </section>

        <section id="projects">
            <h2>Featured Projects</h2>
            <div class="project-grid">
                <div class="project-card">
                    <h3>Associate Editor</h3>
                    <p style="color:var(--dim); font-size: 0.9rem; margin: 10px 0;">Real-time collaborative tool built with Next.js and Firebase Firestore.</p>
                    <button class="skill-chip" onclick="alert('Opening Project...')">View Live</button>
                </div>
                <div class="project-card">
                    <h3>Robotics Learning Hub</h3>
                    <p style="color:var(--dim); font-size: 0.9rem; margin: 10px 0;">A platform for students to learn robotics assembly and coding.</p>
                    <button class="skill-chip" onclick="alert('Opening Docs...')">View Source</button>
                </div>
            </div>
        </section>
    </div>

    <script>
        // 1. Intersection Observer for Scroll Animations
        const observerOptions = { threshold: 0.2 };
        const observer = new IntersectionObserver((entries) => {
            entries.forEach(entry => {
                if (entry.isIntersecting) {
                    entry.target.classList.add('visible');
                    if(entry.target.id === 'about') startCounters();
                }
            });
        }, observerOptions);

        document.querySelectorAll('section').forEach(section => {
            observer.observe(section);
        });

        // 2. Animated Counters for Stats
        function startCounters() {
            const counters = document.querySelectorAll('.counter');
            counters.forEach(counter => {
                const updateCount = () => {
                    const target = +counter.getAttribute('data-target');
                    const count = +counter.innerText;
                    const speed = 200; 
                    const inc = target / speed;

                    if (count < target) {
                        counter.innerText = Math.ceil(count + inc);
                        setTimeout(updateCount, 10);
                    } else {
                        counter.innerText = target + "+";
                    }
                };
                updateCount();
            });
        }

        // 3. Simple Dynamic Greeting based on time
        window.onload = () => {
            const hour = new Date().getHours();
            const welcomeMsg = hour < 12 ? "Good Morning!" : (hour < 18 ? "Good Afternoon!" : "Good Evening!");
            console.log(`${welcomeMsg} Welcome to Ravi's Portfolio.`);
        };
    </script>
</body>
</html>
