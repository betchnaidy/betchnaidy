<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Futuristic README</title>
  <style>
    /* Exemplo de estilo futurista */
    body {
      font-family: 'Arial', sans-serif;
      background-color: #1c1c1c;
      color: white;
      padding: 20px;
    }
    h1 {
      color: #00ffff;
      text-align: center;
      animation: glow 1.5s ease-in-out infinite alternate;
    }
    @keyframes glow {
      0% { text-shadow: 0 0 5px #00ffff, 0 0 10px #00ffff; }
      100% { text-shadow: 0 0 20px #00ffff, 0 0 30px #00ffff; }
    }
    .tab {
      display: flex;
      gap: 10px;
      cursor: pointer;
      font-size: 20px;
      margin-bottom: 20px;
    }
    .tab:hover {
      color: #ff6600;
    }
    .content {
      display: none;
    }
    .active {
      display: block;
    }
  </style>
</head>
<body>

  <h1>Project: Futuristic README</h1>

  <div class="tab" onclick="showContent('overview')">Overview</div>
  <div class="tab" onclick="showContent('installation')">Installation</div>
  <div class="tab" onclick="showContent('features')">Features</div>

  <div id="overview" class="content">
    <h2>Overview</h2>
    <p>This project aims to demonstrate futuristic README design with modern web technologies.</p>
  </div>
  <div id="installation" class="content">
    <h2>Installation</h2>
    <p>Install using npm: <code>npm install project-name</code></p>
  </div>
  <div id="features" class="content">
    <h2>Features</h2>
    <p>Includes animations, dynamic content, and modern UI elements.</p>
  </div>

  <script>
    function showContent(tabId) {
      let contents = document.querySelectorAll('.content');
      contents.forEach(content => content.classList.remove('active'));

      let activeContent = document.getElementById(tabId);
      activeContent.classList.add('active');
    }
  </script>

</body>
</html>
