<!DOCTYPE html>
<html lang="pt-BR">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Surpresa de 1 Ano de Namoro</title>

    <link rel="preconnect" href="https://fonts.googleapis.com">
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
    <link href="https://fonts.googleapis.com/css2?family=Dancing+Script:wght@400;700&family=Irish+Grover&family=Slackey&display=swap" rel="stylesheet">
    <style>
        body {
            background-image: url('8860978-fundo-romantico-com-coracoes-dia-dos-namorados-gratis-vetor.jpg');
            background-size: 100%;
            background-repeat: no-repeat;
            background-color: #ffe6e6;
            text-align: center;
            height: 100%;
            margin: 0;
            padding: 80px;
        }

        h1 {
            font-family: 'Dancing Script', cursive;
            color: #352121;
            margin-bottom: 30px;
            font-size: 36px;
        }

        label {
            font-family: 'Dancing Script', cursive;
            font-size: 28px;
            color: #49085e;
        }

        input {
            font-family: 'Irish Grover', cursive;
            padding: 10px;
            font-size: 16px;
            margin: 10px 0;
            border: 2px solid #ff9999;
            border-radius: 10px;
            width: 300px;
        }

        button {
            font-family: 'Slackey', cursive;
            padding: 15px 10px;
            font-size: 18px;
            color: white;
            background-color: #ff9999;
            border: none;
            border-radius: 10px;
            cursor: pointer;
            margin: 50px;
        }

        button:hover {
            background-color: #ff4d4d;
        }

        .mensagem {
            font-family: 'Frijole';
            color: #070707;
            margin-top: 20px;
            display: none;
        }

        .final-mensagem {
            margin-top: 30px;
            font-size: 20px;
            color: #111111;
        }

        .surpresa {
            display: none;
        }

        .surpresa h2 {
            font-family: 'Dancing Script', cursive;
            font-size: 32px;
            color: #100f0f;
            margin-bottom: 20px;
        }

        .surpresa video {
            width: 80%;
            max-width: 600px;
            border: 4px solid #ff9999;
            border-radius: 10px;
            margin-top: 20px;
        }
    </style>
</head>
<body>
    <h1>Nosso Dia 03/11/2024!!! <br>
        Feliz 1 Ano de Namoro meu amor S2
    </h1>

    <div id="pergunta1">
        <label>Qual o nome do seu namorado?</label><br>
        <input type="text" id="nome" placeholder="Digite o nome do seu namorado"> 
        <br>
        <button onclick="verificarNome()">Responder</button>
        <p class="mensagem" id="mensagem1">IIIIIHHH TA CONFUNDINDO FIOOO????</p>
    </div>

    <div id="pergunta2" style="display: none;">
        <label>Qual a idade do seu namorado?</label><br>
        <input type="number" id="idade" placeholder="Digite a idade">
        <br>
        <button onclick="verificarIdade()">Responder</button>
        <p class="mensagem" id="mensagem2">MANOOOOOOOO, ERROU PQ TIOO?? TA ME CONFUNDINDO???</p>
    </div>

    <div id="pergunta3" style="display: none;">
        <label>Qual a comida favorita dele?</label><br>
        <input type="text" id="comida" placeholder="Digite a comida favorita dele">
        <br>
        <button onclick="verificarComida()">Responder</button>
        <p class="mensagem" id="mensagem3">COMEÇA COM P E TERMINA COM A</p>
    </div>

    <div id="pergunta4" style="display: none;">
        <label>Qual a cor favorita do Luquinhas?</label><br>
        <input type="text" id="color" placeholder="Digite a cor favorita do Luquinhas">
        <br>
        <button onclick="verificarColor()">Responder</button>
        <p class="mensagem" id="mensagem4">NAOOO VIDAA, ME CONHECE NÃO??</p>
    </div>

    <div id="pergunta5" style="display: none;">
        <label>Qual carro eu escolheria Audi R8/Porsche 911/LancerEvo?</label><br>
        <input type="text" id="carro" placeholder="Pense bem e digite qual carro o Luquinhas pegaria?">
        <br>
        <button onclick="verificarCarro()">Responder</button>
        <p class="mensagem" id="mensagem5">KKKKKKKKKKKKKKKKKKKKKKKKKKK NEM EU SEI NESSA</p>
    </div>

    <div id="pergunta6" style="display: none;">
        <label>Quem ele escolheria pra casar, você ou o Cristiano Ronaldo?</label><br>
        <input type="text" id="casar" placeholder="Digite sua resposta">
        <br>
        <button onclick="verificarCasamento()">Responder</button>
        <p class="mensagem" id="mensagem6">AAAA MY AMORR, eu casaria com ele, mas vou casar com você vai</p>
    </div>

    <div id="perguntaFinal" style="display: none;">
        <p class="final-mensagem">BOM MESMO VOCÊ TER ACERTADO TUDO MALANDRO, QUER ABRIR A SURPRESA!?</p>
        <button onclick="mostrarSurpresa()">Sim</button>
        <button onclick="fecharAba()">Não</button>
    </div>

    <div class="surpresa" id="surpresa">
        <h2>Parabéns, amor! Aqui está sua surpresa:</h2>
        <video controls>
            <source src="video_surpresa.mp4" type="video/mp4">
            Seu navegador não suporta a exibição de vídeos.
        </video>
    </div>

    <script>
        function verificarNome() {
            const nome = document.getElementById('nome').value;
            if (nome.trim() === '') {
                alert("OOOO CABEÇA DE BAGRE, PREENCHE O CAMPO");
                return;
            }
            if (nome.toLowerCase() === 'lucas') {
                document.getElementById('pergunta1').style.display = 'none';
                document.getElementById('pergunta2').style.display = 'block';
            } else {
                document.getElementById('mensagem1').style.display = 'block';
            }
        }

        function verificarIdade() {
            const idade = document.getElementById('idade').value;
            if (idade.trim() === '') {
                alert("MY AMORTADELA, PREENCHE O CAMPO");
                return;
            }
            if (idade === '17') {
                document.getElementById('pergunta2').style.display = 'none';
                document.getElementById('pergunta3').style.display = 'block';
            } else {
                document.getElementById('mensagem2').style.display = 'block';
            }
        }

        function verificarComida() {
            const comida = document.getElementById('comida').value.toLowerCase();
            if (comida.trim() === '') {
                alert("MEOO DEUSS, DE NOVO?? PREENCHE FIOO");
                return;
            }
            if (comida === 'pizza') {
                document.getElementById('pergunta3').style.display = 'none';
                document.getElementById('pergunta4').style.display = 'block';
            } else {
                document.getElementById('mensagem3').style.display = 'block';
            }
        }

        function verificarColor() {
            const color = document.getElementById('color').value.toLowerCase();
            if (color.trim() === '') {
                alert("OOO LAIA VIUUU, PREENCHE O CAMPOOOO");
                return;
            }
            if (color === 'azul') {
                document.getElementById('pergunta4').style.display = 'none';
                document.getElementById('pergunta5').style.display = 'block';
            } else {
                document.getElementById('mensagem4').style.display = 'block';
            }
        }

        function verificarCarro() {
            const carro = document.getElementById('carro').value.toLowerCase();
            if (carro.trim() === '') {
                alert("VIDAAAAAAAAAAAAAAAAAAA PREENCHEE MEOO");
                return;
            }
            if (carro === 'porsche 911') {
                document.getElementById('pergunta5').style.display = 'none';
                document.getElementById('pergunta6').style.display = 'block';
            } else {
                document.getElementById('mensagem5').style.display = 'block';
            }
        }

        function verificarCasamento() {
            const casar = document.getElementById('casar').value.toLowerCase();
            if (casar.trim() === '') {
                alert("AAAAA NAOO, DE NOVO???");
                return;
            }
            if (casar === 'eu') {
                document.getElementById('pergunta6').style.display = 'none';
                document.getElementById('perguntaFinal').style.display = 'block';
                alert("AIAII, AUTOESTIMA TA ALTA HEIN");
            } else {
                document.getElementById('mensagem6').style.display = 'block';
            }
        }

        function mostrarSurpresa() {
            // Oculta todas as perguntas e exibe a surpresa
            document.getElementById('perguntaFinal').style.display = 'none';
            document.getElementById('surpresa').style.display = 'block';
        }

        function fecharAba() {
            alert("IHHHHHHHHHHHHH TEM ESSA NÃO, VAI ABRIR SIMMMMMMM");
            window.close();
        }
    </script>
</body>
</html>
