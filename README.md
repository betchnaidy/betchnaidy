<!DOCTYPE html>
<html lang="pt-BR">
<head>
    <meta charset="UTF-8">
    <title>NeuroCore - README 2025</title>
    <link href="https://fonts.googleapis.com/css2?family=Orbitron:wght@400;700&family=Exo+2:wght@300;600&display=swap" rel="stylesheet">
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0/css/all.min.css">
    <style>
        :root {
            --neon-cyan: #00f3ff;
            --neon-purple: #bc13fe;
            --metalic-silver: #c0c0c0;
            --background-dark: #0a0a0f;
        }

        body {
            background: var(--background-dark);
            color: var(--metalic-silver);
            font-family: 'Exo 2', sans-serif;
            overflow-x: hidden;
        }

        /* Animação do Título */
        @keyframes glow {
            0% { text-shadow: 0 0 10px var(--neon-cyan); }
            50% { text-shadow: 0 0 20px var(--neon-purple); }
            100% { text-shadow: 0 0 10px var(--neon-cyan); }
        }

        .title {
            animation: glow 3s infinite;
            font-family: 'Orbitron', sans-serif;
        }

        /* Seções Interativas */
        .tab-content { display: none; }
        .tab-content.active {
            display: block;
            animation: slideIn 0.5s ease-out;
        }

        @keyframes slideIn {
            from { transform: translateX(100%); opacity: 0; }
            to { transform: translateX(0); opacity: 1; }
        }

        /* Gráficos Interativos (Exemplo) */
        .tech-icon:hover {
            transform: scale(1.2);
            filter: drop-shadow(0 0 15px var(--neon-cyan));
            transition: all 0.3s ease;
        }
    </style>
</head>
<body>
    <header>
        <h1 class="title">🚀 NeuroCore</h1>
        <p class="tagline">Revolucionando a Automação com IA Quântica</p>
        <div class="logo" id="animated-logo"></div>
    </header>

    <section class="video-intro">
        <video src="demo.mp4" controls></video>
    </section>

    <div class="tabs">
        <button class="tab-button" onclick="openTab('overview')">Visão Geral</button>
        <button class="tab-button" onclick="openTab('install')">Instalação</button>
    </div>

    <div id="overview" class="tab-content active">
        <h3>✨ Tecnologias</h3>
        <div class="tech-grid">
            <i class="fab fa-react tech-icon"></i>
            <i class="fab fa-python tech-icon"></i>
        </div>
    </div>

    <script>
        function openTab(tabName) {
            document.querySelectorAll('.tab-content').forEach(tab => tab.classList.remove('active'));
            document.getElementById(tabName).classList.add('active');
        }
    </script>
</body>
</html>
