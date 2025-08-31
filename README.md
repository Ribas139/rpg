# rpg
<!DOCTYPE html>
<html lang="pt-br">
<head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1" />
    <title>O Mundo dos RPGs</title>
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
    <h2>Explorando mundos, criando heróis e enfrentando monstros</h2>

    <section>
        <div class="video-container">
            <iframe src="https://www.youtube.com/embed/u84nTLfGfwg" title="O que é RPG?"></iframe>
        </div>

        <p>
            RPG (Role-Playing Game) é um gênero de jogo onde os participantes interpretam personagens fictícios em mundos imaginários. Com origem nos anos 1970, os RPGs misturam elementos de narrativa, estratégia e interpretação.
            Jogadores assumem papéis como guerreiros, magos, ladrões ou clérigos, enfrentando desafios, batalhas e missões dentro de histórias épicas conduzidas por um mestre ou através de videogames.
        </p>
    </section>

    <button id="toggle-info">Mostrar mais informações</button>

    <div id="extra-info">
        <p>
            Existem diversos tipos de RPG: de mesa (como Dungeons & Dragons), eletrônicos (como Final Fantasy, The Witcher e Skyrim) e até ao vivo (Live Action RPG). Cada um oferece uma forma única de imersão no enredo e na criação de mundos fantásticos.
        </p>
        <p>
            Nos RPGs de mesa, os jogadores rolam dados e usam livros de regras. Já nos eletrônicos, a experiência é guiada por sistemas digitais e gráficos complexos, permitindo mundos abertos vastos e cheios de possibilidades.
        </p>
        <p>
            O verdadeiro coração do RPG está na criatividade e cooperação. É mais do que um jogo — é uma forma de contar histórias juntos, onde cada decisão pode mudar o destino de um reino inteiro.
        </p>
    </div>

    <section>
        <h2>Mais vídeos sobre RPG</h2>
        <div class="video-container">
            <iframe src="https://www.youtube.com/embed/3BGU2ozQLlE" title="Como funciona um RPG de mesa?"></iframe>
            <iframe src="https://www.youtube.com/embed/Zb6FtlM5r3Q" title="História dos RPGs eletrônicos"></iframe>
            <iframe src="https://www.youtube.com/embed/yhUWoX2kLDg" title="Skyrim - O clássico dos RPGs modernos"></iframe>
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
