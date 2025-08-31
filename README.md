# rpg
<!DOCTYPE html>
<html lang="pt-br">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1" />
  <title>O Mundo dos RPGs - Ordem Paranormal</title>
  <link href="https://fonts.googleapis.com/css2?family=Roboto:wght@400;700&display=swap" rel="stylesheet" />
  <style>
    body {
      background-color: #1a0033;
      color: #ffccff;
      font-family: 'Roboto', Arial, sans-serif;
      margin: 0;
      padding: 20px;
      line-height: 1.6;
    }

    h1, h2 {
      text-align: center;
      text-shadow: 2px 2px 4px #000;
      transition: color 0.3s ease;
      cursor: pointer;
    }

    h1 {
      color: #ff6600;
      margin-bottom: 10px;
    }

    h2 {
      color: #ff99ff;
      margin-bottom: 30px;
    }

    h1:hover, h2:hover {
      color: #ffffff;
    }

    p {
      max-width: 800px;
      margin: 0 auto 40px auto;
      font-size: 18px;
    }

    .video-container {
      display: flex;
      justify-content: center;
      flex-wrap: wrap;
      gap: 20px;
      margin-bottom: 40px;
    }

    iframe {
      border: 3px solid #ff6600;
      border-radius: 10px;
      width: 100%;
      max-width: 500px;
      height: 280px;
    }

    @media (max-width: 600px) {
      iframe {
        height: 200px;
      }
      p {
        font-size: 16px;
      }
    }

    button {
      display: block;
      margin: 0 auto 30px auto;
      background-color: #ff6600;
      border: none;
      color: #1a0033;
      font-weight: 700;
      padding: 12px 25px;
      font-size: 16px;
      border-radius: 30px;
      cursor: pointer;
      box-shadow: 0 4px 10px rgba(255, 102, 0, 0.6);
      transition: background-color 0.3s ease;
    }

    button:hover {
      background-color: #cc5200;
    }

    #extra-info {
      max-width: 800px;
      margin: 0 auto 40px auto;
      font-size: 18px;
      display: none;
      color: #ffd6ff;
      border-left: 4px solid #ff6600;
      padding-left: 15px;
      background-color: rgba(255, 102, 0, 0.1);
      border-radius: 6px;
    }

    section {
      margin-bottom: 50px;
    }
  </style>
</head>
<body>
  <h1>O Mundo dos RPGs</h1>
  <h2>Explorando o universo de <em>Ordem Paranormal</em> com Cellbit</h2>

  <section>
    <div class="video-container">
      <!-- Exemplo de vídeo introdutório -->
      <iframe width="560" height="315" src="https://www.youtube.com/embed/Pf4HzTdA2WE?si=gacmOhPlZsvM_v3h" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
    </div>
    <p>
      A websérie <strong>Ordem Paranormal</strong>, criada e apresentada por Cellbit, é uma experiência imersiva de RPG de mesa com temática de investigação paranormal, onde um grupo de agentes enfrenta mistérios sobrenaturais. A segunda temporada, “O Segredo na Floresta”, utiliza um sistema inspirado em *Call of Cthulhu* :contentReference[oaicite:0]{index=0}.
    </p>
  </section>

  <button id="toggle-info">Mostrar mais informações</button>

  <div id="extra-info">
    <p>
      A websérie começou em fevereiro de 2020 e conta com múltiplas campanhas como “A Ordem Paranormal”, “O Segredo na Floresta” e várias temporadas posteriores, além de spin-offs :contentReference[oaicite:1]{index=1}.
    </p>
    <p>
      Essas histórias se expandiram além das lives: ganharam adaptações em livros de regras, HQs e até inspiraram o jogo digital *Enigma do Medo*, lançado em novembro de 2024 :contentReference[oaicite:2]{index=2}.
    </p>
    <p>
      É uma narrativa que mistura investigação, horror e drama, reunindo jogadores e espectadores em uma experiência rica e colaborativa.
    </p>
  </div>

  <section>
    <h2>Vídeos de Ordem Paranormal</h2>
    <div class="video-container">
      <iframe width="560" height="315" src="https://www.youtube.com/embed/zgaZoMswQG4?si=zqa7_82Mdo8lncl5" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
      <iframe width="560" height="315" src="https://www.youtube.com/embed/k5y48mQTdpE?si=PpPK67aVHhSOgM3S" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
      <iframe width="560" height="315" src="https://www.youtube.com/embed/wiGlOf3mCVM?si=WRk8_q4PfpZzGCNn" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
    </div>
  </section>

  <script>
    const btn = document.getElementById('toggle-info');
    const extraInfo = document.getElementById('extra-info');

    btn.addEventListener('click', () => {
      if (extraInfo.style.display === 'none' || extraInfo.style.display === '') {
        extraInfo.style.display = 'block';
        btn.textContent = 'Mostrar menos informações';
      } else {
        extraInfo.style.display = 'none';
        btn.textContent = 'Mostrar mais informações';
      }
    });
  </script>
</body>
</html>
