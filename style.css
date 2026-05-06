<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Nikhil Adagatala | Portfolio</title>
    <script src="https://unpkg.com"></script>
    <style>
        :root {
            --bg: #0b0b0b;
            --card-bg: rgba(255, 255, 255, 0.05);
            --text: #ffffff;
            --accent: #0071e3;
            --glass-border: rgba(255, 255, 255, 0.1);
        }

        .light-mode {
            --bg: #f5f5f7;
            --card-bg: rgba(0, 0, 0, 0.05);
            --text: #1d1d1f;
            --glass-border: rgba(0, 0, 0, 0.1);
        }

        * { box-sizing: border-box; scroll-behavior: smooth; margin: 0; padding: 0; }
        body { 
            background: var(--bg); 
            color: var(--text); 
            font-family: -apple-system, BlinkMacSystemFont, "SF Pro Display", sans-serif;
            transition: all 0.5s ease;
        }

        /* Glassmorphism Utility */
        .glass {
            background: var(--card-bg);
            backdrop-filter: blur(15px);
            -webkit-backdrop-filter: blur(15px);
            border: 1px solid var(--glass-border);
        }

        /* Navbar */
        nav {
            display: flex;
            justify-content: space-between;
            padding: 1rem 5%;
            align-items: center;
            position: fixed;
            width: 100%;
            top: 0;
            z-index: 1000;
        }

        .nav-links { display: flex; list-style: none; gap: 2rem; }
        .nav-links a { color: var(--text); text-decoration: none; font-weight: 500; opacity: 0.7; transition: 0.3s; }
        .nav-links a:hover { opacity: 1; color: var(--accent); }

        /* Hero Section */
        .hero {
            height: 100vh;
            display: flex;
            flex-direction: column;
            align-items: center;
            justify-content: center;
            text-align: center;
            padding-top: 60px;
        }

        .profile-frame {
            width: 200px;
            height: 200px;
            border-radius: 50%;
            overflow: hidden;
            margin-bottom: 1.5rem;
            border: 4px solid var(--accent);
            box-shadow: 0 10px 30px rgba(0,0,0,0.5);
            animation: popIn 1s cubic-bezier(0.175, 0.885, 0.32, 1.275);
        }

        .profile-img { width: 100%; height: 100%; object-fit: cover; }

        @keyframes popIn { from { transform: scale(0); } to { transform: scale(1); } }

        h1 { font-size: 3rem; margin-bottom: 0.5rem; }
        .subtitle { font-size: 1.5rem; color: var(--accent); font-weight: 300; }

        .btn {
            margin-top: 2rem;
            padding: 12px 30px;
            background: var(--accent);
            color: white;
            text-decoration: none;
            border-radius: 30px;
            font-weight: 600;
            transition: 0.3s;
            display: inline-flex;
            align-items: center;
            gap: 8px;
        }
        .btn:hover { transform: scale(1.05); box-shadow: 0 5px 15px rgba(0,113,227,0.4); }

        /* Sections */
        .section { padding: 100px 10%; }
        .section-title { font-size: 2.5rem; margin-bottom: 2rem; text-align: center; }

        .grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 2rem;
        }

        .glass-card {
            padding: 2rem;
            border-radius: 20px;
            background: var(--card-bg);
            border: 1px solid var(--glass-border);
            transition: 0.3s;
        }
        .glass-card:hover { transform: translateY(-10px); }

        /* Modal */
        .modal {
            display: none;
            position: fixed;
            z-index: 2000;
            top: 0; left: 0; width: 100%; height: 100%;
            background: rgba(0,0,0,0.9);
            justify-content: center;
            align-items: center;
        }
        .modal-content { max-width: 80%; max-height: 80%; border-radius: 10px; }

        #theme-toggle { cursor: pointer; border: none; background: none; color: var(--text); }
        .hidden { display: none; }
    </style>
</head>
<body class="dark-mode">

    <nav class="glass">
        <div class="logo" style="font-weight: 800; font-size: 1.5rem;">N.A</div>
        <ul class="nav-links">
            <li><a href="#home">Home</a></li>
            <li><a href="#about">About</a></li>
            <li><a href="#projects">Projects</a></li>
            <li><a href="#certificates">Certificates</a></li>
        </ul>
        <button id="theme-toggle">
            <i data-lucide="sun" id="sun-icon" class="hidden"></i>
            <i data-lucide="moon" id="moon-icon"></i>
        </button>
    </nav>

    <section id="home" class="hero">
        <div class="profile-frame">
            <!-- Using the image you provided -->
            <img src="https://ibb.co" alt="Nikhil Adagatala" class="profile-img">
        </div>
        <h1>Nikhil Vinayak Adagatala</h1>
        <p class="subtitle" id="typing"></p>
        <!-- Download Button -->
        <a href="your-cv-link.pdf" download class="btn">
            <i data-lucide="download"></i> Download CV
        </a>
    </section>

    <section id="about" class="section">
        <h2 class="section-title">About Me</h2>
        <div class="glass-card">
            <p style="font-size: 1.2rem; line-height: 1.8;">
                I am a B.Tech Computer Science student at <strong>MIT Vishwaprayag University (MIT VPU)</strong>. 
                I specialize in C, C++, Java, and Modern Web Technologies.
            </p>
        </div>
    </section>

    <section id="certificates" class="section">
        <h2 class="section-title">Certificates</h2>
        <div class="grid">
            <div class="glass-card" onclick="openModal('https://placeholder.com', 'Certificate Title')">
                <img src="https://placeholder.com" style="width: 100%; border-radius: 10px; cursor: pointer;">
                <h3 style="margin-top: 1rem;">Course Name</h3>
            </div>
        </div>
    </section>

    <div id="certModal" class="modal" onclick="this.style.display='none'">
        <img class="modal-content" id="modalImg">
    </section>

    <script>
        // Lucide Icons
        lucide.createIcons();

        // Typing Effect
        const text = "Aspiring Software Developer | Web Developer | Programmer";
        let i = 0;
        function typeWriter() {
            if (i < text.length) {
                document.getElementById("typing").innerHTML += text.charAt(i);
                i++;
                setTimeout(typeWriter, 100);
            }
        }
        typeWriter();

        // Theme Toggle
        const btn = document.getElementById("theme-toggle");
        btn.onclick = () => {
            document.body.classList.toggle("light-mode");
            document.getElementById("sun-icon").classList.toggle("hidden");
            document.getElementById("moon-icon").classList.toggle("hidden");
        };

        // Modal
        function openModal(src) {
            document.getElementById("certModal").style.display = "flex";
            document.getElementById("modalImg").src = src;
        }
    </script>
</body>
</html>
