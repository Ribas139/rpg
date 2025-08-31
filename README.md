# rpg
rpg-site/
├── index.html
├── style.css
└── script.js
<!DOCTYPE html>
<html lang="pt-br">
<head>
  <meta charset="UTF-8">
  <title>Reino dos Heróis</title>
  <link rel="stylesheet" href="style.css">
</head>
<body>
  <header>
    <h1>🏰 Reino dos Heróis</h1>
    <nav>
      <ul>
        <li><a href="#historia">História</a></li>
        <li><a href="#videos">Vídeos</a></li>
        <li><a href="#personagens">Personagens</a></li>
      </ul>
    </nav>
  </header>

  <section id="historia">
    <h2>A História do Reino</h2>
    <p>Em um mundo de dragões e magos, heróis surgem para defender a paz contra as forças das trevas...</p>
  </section>

  <section id="videos">
    <h2>🎥 Vídeos do RPG</h2>
    <div class="video-container">
      <iframe src="https://www.youtube.com/embed/VIDEO_ID_AQUI" allowfullscreen></iframe>
      <iframe src="https://www.youtube.com/embed/VIDEO_ID_AQUI2" allowfullscreen></iframe>
    </div>
  </section>

  <section id="personagens">
    <h2>⚔️ Personagens Principais</h2>
    <ul>
      <li><strong>Arthas</strong> – O Cavaleiro da Luz</li>
      <li><strong>Lyra</strong> – A Maga Elemental</li>
      <li><strong>Gorun</strong> – O Orc Guerreiro</li>
    </ul>
  </section>

  <footer>
    <p>&copy; 2025 Reino dos Heróis</p>
  </footer>

  <script src="script.js"></script>
</body>
</html>
body {
  font-family: 'Segoe UI', sans-serif;
  background: linear-gradient(to bottom, #2e1a47, #0f0c29);
  color: #fff;
  margin: 0;
  padding: 0;
}

header {
  background-color: #4b0082;
  padding: 20px;
  text-align: center;
}

nav ul {
  list-style: none;
  padding: 0;
  display: flex;
  justify-content: center;
  gap: 20px;
}

nav a {
  color: #ffd700;
  text-decoration: none;
  font-weight: bold;
}

section {
  padding: 40px 20px;
  background-color: rgba(0, 0, 0, 0.3);
  margin: 20px;
  border-radius: 8px;
}

.video-container {
  display: flex;
  gap: 20px;
  flex-wrap: wrap;
}

iframe {
  width: 300px;
  height: 180px;
  border: none;
}

footer {
  text-align: center;
  background-color: #222;
  padding: 20px;
}
// Apenas um efeito básico de boas-vindas
window.onload = () => {
  alert("Bem-vindo ao Reino dos Heróis!");
};

