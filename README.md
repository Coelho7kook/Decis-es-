echo "# Decis-es-" >> README.md
git init
git add README.md
git commit -m "first commit"
git branch -M main
git remote add origin https://github.com/Coelho7kook/Decis-es-.git
git push -u origin main




<!DOCTYPE html>
<html lang="pt-BR">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Para Kamille</title>
    <style>
        body {
            background-image: url('background.jpg'); /* Adiciona a imagem de fundo */
            background-size: cover;
            font-family: 'Times New Roman', serif;
            color: #333;
            text-align: center;
            padding: 50px;
        }
        .content {
            margin: auto;
            width: 70%;
            background-color: rgba(255, 255, 255, 0.8);
            padding: 20px;
            border-radius: 10px;
        }
        h1 {
            font-size: 2em;
            margin-bottom: 20px;
        }
        p {
            font-size: 1.2em;
            line-height: 1.6;
            text-align: justify;
            text-indent: 2em;
        }
        img {
            width: 100%;
            height: auto;
            margin: 20px 0;
            border-radius: 10px;
        }
        .buttons {
            margin-top: 30px;
        }
        .buttons button {
            padding: 15px 25px;
            font-size: 1.2em;
            margin: 10px;
            border-radius: 5px;
            border: none;
            cursor: pointer;
        }
        .button1 {
            background-color: #4CAF50;
            color: white;
        }
        .button2 {
            background-color: #f44336;
            color: white;
        }
        .button3 {
            background-color: #2196F3;
            color: white;
        }
        .button4 {
            background-color: #FF9800;
            color: white;
        }
    </style>
</head>
<body onload="playAudio('musica1')">

    <!-- Elementos de áudio -->
    <audio id="musica1" loop autoplay>
        <source src="musica1.mp3" type="audio/mp3">
        Seu navegador não suporta o elemento de áudio.
    </audio>

    <audio id="musica2" loop>
        <source src="musica2.mp3" type="audio/mp3">
        Seu navegador não suporta o elemento de áudio.
    </audio>

    <audio id="musica3" loop>
        <source src="musica3.mp3" type="audio/mp3">
        Seu navegador não suporta o elemento de áudio.
    </audio>

    <div class="content">
        <h1>Minha Querida Kamille</h1>
        <img src="top_image.jpg" alt="Imagem Superior">
        <p id="main-text">Meu amor, Kamille. 

O que aconteceu hoje de manhã foi uma grande confusão, uma tempestade que não deveria ter existido. O que deveria ter sido um momento comum acabou se tornando algo muito doloroso para nós dois. 

Eu nunca quis te machucar, e tudo o que aconteceu foi resultado de um mal-entendido. Meu amigo, que apenas buscava um pouco de carinho, acabou usando o meu celular e, no meio disso tudo, ele se confundiu e te fez acreditar que eu estava envolvido em algo que eu nunca faria. Você é tudo para mim, e eu jamais te desrespeitaria dessa forma. 

Sei que parece impossível, mas peço que entenda que tudo o que aconteceu foi uma grande trapalhada, um engano que eu jamais deixaria acontecer se soubesse o que estava se passando. Eu te amo, Kamille, e tudo o que quero é poder te abraçar de novo, olhar nos seus olhos e dizer o quanto te amo.</p>
        <img src="bottom_image.jpg" alt="Imagem Inferior">

        <div class="buttons">
            <button class="button1" onclick="showText('continuar', 'musica2')">Recomeçar/Continuar</button>
            <button class="button2" onclick="showText('terminar', 'musica3')">Tudo Acaba por Aqui</button>
            <button class="button3" onclick="resetText()">Voltar ao Inicial</button>
        </div>

        <p id="continuar" style="display:none;">Recomeçar ao seu lado seria como reviver um sonho, um sonho que eu nunca quis acordar. 

O dia 28 de agosto está chegando, e eu não consigo imaginar um dia mais feliz do que passar esse momento especial com você. Além disso, setembro também se aproxima, e com ele nosso aniversário de namoro. Como eu poderia querer mais do que celebrar o amor que sentimos um pelo outro? 

Eu me vejo ao seu lado, planejando cada detalhe da nossa vida juntos, desde nossos passeios, nossos risos, até os momentos mais simples, como jogar Minecraft lado a lado, ou apenas ficar abraçados no sofá. Eu já consigo imaginar o dia em que finalmente poderemos nos encontrar, e o quanto esse dia será inesquecível. 

Por isso, te peço com todo o meu coração: Vamos recomeçar, vamos continuar construindo nossa história, porque nada mais importa para mim além de estar ao seu lado. 

Se você também sente isso, me envie a mensagem '143' no WhatsApp, e vamos dar continuidade ao nosso sonho, juntos.</p>
        <p id="terminar" style="display:none;">Se esta for sua escolha, Kamille, então aceitarei, mas não sem antes te lembrar de tudo o que vivemos. 

Lembro de todos os momentos em que conversamos até tarde da noite, sonhando com o dia em que nos encontraríamos. Todos os nossos planos, nossos risos, as promessas que fizemos um ao outro. Sei que não sou perfeito, mas tudo o que fiz foi com o desejo sincero de te fazer feliz. 

Sei que hoje as coisas pareceram confusas, mas eu preciso que você entenda que eu nunca quis te machucar. Se escolher que tudo deve acabar por aqui, eu respeitarei sua decisão, mesmo que meu coração se parta. 

Por favor, pense bem, e se esse realmente for seu desejo, mande 'F' no WhatsApp, e tudo entre nós acabará. Mas saiba que sempre vou te amar, e que você sempre será a minha Kamille.</p>
    </div>

    <script>
        function showText(option, audioId) {
            var mainText = document.getElementById('main-text');
            var continuarText = document.getElementById('continuar');
            var terminarText = document.getElementById('terminar');

            mainText.style.display = 'none';
            continuarText.style.display = 'none';
            terminarText.style.display = 'none';

            document.getElementById('musica1').pause();
            document.getElementById('musica2').pause();
            document.getElementById('musica3').pause();

            if (option === 'continuar') {
                continuarText.style.display = 'block';
                document.getElementById(audioId).play();
            } else if (option === 'terminar') {
                terminarText.style.display = 'block';
                document.getElementById(audioId).play();
            }
        }

        function resetText() {
            document.getElementById('main-text').style.display = 'block';
            document.getElementById('continuar').style.display = 'none';
            document.getElementById('terminar').style.display = 'none';

            document.getElementById('musica1').play();
            document.getElementById('musica2').pause();
            document.getElementById('musica3').pause();
        }

        function playAudio(audioId) {
            document.getElementById(audioId).play();
        }
    </script>
</body>
</html>
