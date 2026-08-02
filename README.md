<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Aya Youssfi | AI & Digital Trust Engineer</title>
    <link href="https://fonts.googleapis.com/css2?family=Fira+Code:wght@300;400;600;700&display=swap" rel="stylesheet">
    <style>
        /* =========================================
           CSS: STYLES & ANIMATIONS CYBERPUNK
           ========================================= */
        :root {
            --bg-color: #0d1117;
            --neon-cyan: #00ffcc;
            --neon-blue: #0a84ff;
            --text-main: #e6edf3;
            --text-muted: #8b949e;
            --card-bg: rgba(13, 17, 23, 0.75);
            --border-glow: 0 0 10px rgba(0, 255, 204, 0.3), inset 0 0 10px rgba(0, 255, 204, 0.1);
        }

        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        body {
            background-color: var(--bg-color);
            color: var(--text-main);
            font-family: 'Fira Code', monospace;
            overflow-x: hidden;
            line-height: 1.6;
        }

        /* Arrière-plan Matrix Canvas */
        canvas {
            position: fixed;
            top: 0;
            left: 0;
            width: 100vw;
            height: 100vh;
            z-index: -1;
            opacity: 0.15;
        }

        .container {
            max-width: 1200px;
            margin: 0 auto;
            padding: 2rem;
            position: relative;
            z-index: 1;
        }

        /* Header / Terminal Glitch Effect */
        header {
            text-align: center;
            margin-bottom: 4rem;
            padding: 4rem 0;
            border-bottom: 1px solid var(--neon-cyan);
            box-shadow: 0 10px 30px -10px rgba(0, 255, 204, 0.2);
        }

        h1 {
            font-size: 3.5rem;
            color: var(--neon-cyan);
            text-shadow: 0 0 15px rgba(0, 255, 204, 0.5);
            margin-bottom: 1rem;
            letter-spacing: -2px;
        }

        .typing-container {
            font-size: 1.2rem;
            color: var(--text-muted);
            min-height: 30px;
        }

        .cursor {
            display: inline-block;
            width: 10px;
            height: 20px;
            background-color: var(--neon-cyan);
            animation: blink 1s step-end infinite;
            vertical-align: text-bottom;
        }

        @keyframes blink {
            50% { opacity: 0; }
        }

        /* Section Titres */
        h2 {
            font-size: 2rem;
            color: #fff;
            margin-bottom: 2rem;
            display: flex;
            align-items: center;
            gap: 15px;
        }

        h2::before {
            content: "[";
            color: var(--neon-cyan);
        }
        h2::after {
            content: "]";
            color: var(--neon-cyan);
        }

        /* Grille des Projets */
        .grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(350px, 1fr));
            gap: 2rem;
            margin-bottom: 4rem;
        }

        /* Cartes (Glassmorphism + Neon Border) */
        .card {
            background: var(--card-bg);
            border: 1px solid rgba(0, 255, 204, 0.2);
            backdrop-filter: blur(10px);
            padding: 2rem;
            border-radius: 8px;
            transition: all 0.3s ease;
            position: relative;
            overflow: hidden;
        }

        .card::before {
            content: '';
            position: absolute;
            top: 0;
            left: -100%;
            width: 100%;
            height: 2px;
            background: linear-gradient(90deg, transparent, var(--neon-cyan));
            transition: 0.5s;
        }

        .card:hover {
            box-shadow: var(--border-glow);
            border-color: var(--neon-cyan);
            transform: translateY(-5px);
        }

        .card:hover::before {
            left: 100%;
        }

        .card h3 {
            color: var(--neon-cyan);
            margin-bottom: 1rem;
            font-size: 1.4rem;
        }

        .card hr {
            border: none;
            height: 1px;
            background: rgba(255, 255, 255, 0.1);
            margin: 1rem 0;
        }

        .tags {
            display: flex;
            flex-wrap: wrap;
            gap: 10px;
            margin-top: 1.5rem;
        }

        .tag {
            font-size: 0.8rem;
            background: rgba(0, 255, 204, 0.1);
            color: var(--neon-cyan);
            padding: 5px 10px;
            border-radius: 4px;
            border: 1px solid rgba(0, 255, 204, 0.3);
        }

        /* Bouton Contact */
        .contact-btn {
            display: inline-block;
            margin-top: 3rem;
            padding: 15px 30px;
            font-family: 'Fira Code', monospace;
            font-size: 1.2rem;
            color: var(--bg-color);
            background-color: var(--neon-cyan);
            text-decoration: none;
            font-weight: bold;
            border-radius: 4px;
            transition: 0.3s;
            box-shadow: 0 0 15px rgba(0, 255, 204, 0.4);
        }

        .contact-btn:hover {
            background-color: transparent;
            color: var(--neon-cyan);
            border: 2px solid var(--neon-cyan);
            box-shadow: 0 0 30px rgba(0, 255, 204, 0.6);
        }

        /* Footer */
        footer {
            text-align: center;
            padding: 2rem;
            margin-top: 4rem;
            color: var(--text-muted);
            border-top: 1px dashed rgba(255, 255, 255, 0.1);
        }

        /* Code Block Style */
        .code-block {
            background: #090c10;
            padding: 1.5rem;
            border-radius: 8px;
            border-left: 3px solid var(--neon-cyan);
            margin-bottom: 4rem;
            overflow-x: auto;
            color: #a5d6ff;
        }
        .code-keyword { color: #ff7b72; }
        .code-string { color: #a5d6ff; }
        .code-comment { color: #8b949e; font-style: italic; }
    </style>
</head>
<body>

    <!-- Canvas pour l'effet Matrix JS -->
    <canvas id="matrix"></canvas>

    <div class="container">
        <!-- HEADER -->
        <header>
            <h1>> AYA_YOUSSFI</h1>
            <div class="typing-container">
                <span id="typing-text"></span><span class="cursor"></span>
            </div>
            <a href="mailto:aya.youssfi@usmba.ac.ma" class="contact-btn">INITIATE_CONTACT()</a>
        </header>

        <!-- SYSTEM OVERVIEW CODE -->
        <section>
            <h2>SYS.OVERVIEW</h2>
            <div class="code-block">
<pre><code><span class="code-keyword">class</span> DigitalTrustEngineer:
    <span class="code-keyword">def</span> __init__(self):
        self.role = <span class="code-string">"AI & Digital Trust Engineering Student"</span>
        self.location = <span class="code-string">"ENSA Fès, Morocco"</span>
        self.mission = <span class="code-string">"Turning black-box AI into secure, auditable, and trusted systems."</span>
        
    <span class="code-keyword">def</span> core_stack(self):
        <span class="code-keyword">return</span> [<span class="code-string">"Python"</span>, <span class="code-string">"PyTorch"</span>, <span class="code-string">"FastAPI"</span>, <span class="code-string">"Kafka"</span>, <span class="code-string">"SHAP"</span>]
        
    <span class="code-comment"># Seeking Internships in AI Risk Advisory or AI Governance</span></code></pre>
            </div>
        </section>

        <!-- DEPLOYMENTS GRID -->
        <section>
            <h2>DEPLOYMENTS</h2>
            <div class="grid">
                <!-- Project 1 -->
                <div class="card">
                    <h3>🛡️ NetGuard IDS</h3>
                    <p><i>Auditable Intrusion Detection</i></p>
                    <hr>
                    <p>Trained on the BETH Dataset (8M+ AWS honeypot kernel events). Isolation Forest flags anomalies, XGBoost classifies them, and SHAP produces human-readable justifications.</p>
                    <div class="tags">
                        <span class="tag">Kafka</span>
                        <span class="tag">XGBoost</span>
                        <span class="tag">SHAP (XAI)</span>
                        <span class="tag">MITRE ATT&CK</span>
                    </div>
                </div>

                <!-- Project 2 -->
                <div class="card">
                    <h3>⚡ Jailbreak Detection</h3>
                    <p><i>Real-Time AI Risk Control</i></p>
                    <hr>
                    <p>A DistilBERT classifier streamed over Apache Pulsar to intercept adversarial prompts before they reach production LLMs in sub-100ms.</p>
                    <div class="tags">
                        <span class="tag">PyTorch</span>
                        <span class="tag">Apache Pulsar</span>
                        <span class="tag">DistilBERT</span>
                    </div>
                </div>

                <!-- Project 3 -->
                <div class="card">
                    <h3>💳 Cluster-Aware XAI</h3>
                    <p><i>Segmented Fraud Detection</i></p>
                    <hr>
                    <p>Segmented 30k clients using HDBSCAN, deploying dedicated Gradient Boosting models per cluster. Imbalance handled with SMOTE.</p>
                    <div class="tags">
                        <span class="tag">HDBSCAN</span>
                        <span class="tag">SMOTE</span>
                        <span class="tag">Flask REST API</span>
                    </div>
                </div>

                <!-- Project 4 -->
                <div class="card">
                    <h3>🏭 GuardianAI Proxy</h3>
                    <p><i>Defense-in-Depth for LLMs</i></p>
                    <hr>
                    <p>FastAPI security proxy utilizing 3 independent middleware layers (auth, prompt filtering, response auditing) to ensure strict LLM compliance.</p>
                    <div class="tags">
                        <span class="tag">FastAPI</span>
                        <span class="tag">LangChain</span>
                        <span class="tag">Pytest</span>
                    </div>
                </div>
            </div>
        </section>

        <!-- FOOTER -->
        <footer>
            <p>"Trust in AI isn't a feature you add at the end — it's a control you design in from the start."</p>
            <p style="margin-top: 10px; font-size: 0.9em;">© 2026 Aya Youssfi. All systems operational.</p>
        </footer>
    </div>

    <!-- =========================================
         JAVASCRIPT: INTERACTIVITÉ & EFFETS
         ========================================= -->
    <script>
        // 1. TYPING EFFECT
        const textArray = [
            "AI & Digital Trust Engineer...",
            "Securing the Future of AI...",
            "Turning Black Boxes into Glass Boxes...",
            "Explainable AI (XAI) & Model Governance..."
        ];
        let textIndex = 0;
        let charIndex = 0;
        const typingElement = document.getElementById("typing-text");

        function type() {
            if (charIndex < textArray[textIndex].length) {
                typingElement.textContent += textArray[textIndex].charAt(charIndex);
                charIndex++;
                setTimeout(type, 80);
            } else {
                setTimeout(erase, 2000);
            }
        }

        function erase() {
            if (charIndex > 0) {
                typingElement.textContent = textArray[textIndex].substring(0, charIndex - 1);
                charIndex--;
                setTimeout(erase, 40);
            } else {
                textIndex = (textIndex + 1) % textArray.length;
                setTimeout(type, 500);
            }
        }

        // Start typing effect
        document.addEventListener("DOMContentLoaded", function() {
            setTimeout(type, 1000);
        });

        // 2. MATRIX RAIN EFFECT (CANVAS)
        const canvas = document.getElementById('matrix');
        const ctx = canvas.getContext('2d');

        canvas.width = window.innerWidth;
        canvas.height = window.innerHeight;

        const letters = 'ABCDEFGHIJKLMNOPQRSTUVWXYZ0123456789@#$%^&*()';
        const fontSize = 14;
        const columns = canvas.width / fontSize;
        const drops = [];

        for (let x = 0; x < columns; x++) {
            drops[x] = 1;
        }

        function drawMatrix() {
            ctx.fillStyle = 'rgba(13, 17, 23, 0.05)';
            ctx.fillRect(0, 0, canvas.width, canvas.height);

            ctx.fillStyle = '#00ffcc'; // Neon Cyan
            ctx.font = fontSize + 'px monospace';

            for (let i = 0; i < drops.length; i++) {
                const text = letters.charAt(Math.floor(Math.random() * letters.length));
                ctx.fillText(text, i * fontSize, drops[i] * fontSize);

                if (drops[i] * fontSize > canvas.height && Math.random() > 0.975) {
                    drops[i] = 0;
                }
                drops[i]++;
            }
        }

        setInterval(drawMatrix, 33);

        // Adjust canvas on resize
        window.addEventListener('resize', () => {
            canvas.width = window.innerWidth;
            canvas.height = window.innerHeight;
        });
    </script>
</body>
</html>
