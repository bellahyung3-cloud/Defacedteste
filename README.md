# Defacedteste
Cachau
pegadinha.html
<!DOCTYPE html>
<html>
<head>
    <meta charset="UTF-8">
    <title>⚠️ AVISO IMPORTANTE</title>
    <style>
        * { margin: 0; padding: 0; box-sizing: border-box; font-family: Arial, sans-serif; }
        body {
            background: #1a1a2e;
            min-height: 100vh;
            display: flex;
            align-items: center;
            justify-content: center;
            color: white;
            padding: 20px;
        }
        .caixa {
            background: #16213e;
            padding: 40px 30px;
            border-radius: 12px;
            border: 2px solid #e94560;
            box-shadow: 0 0 30px rgba(233, 69, 96, 0.3);
            text-align: center;
            max-width: 400px;
        }
        .alerta { font-size: 50px; margin-bottom: 20px; }
        h1 { color: #e94560; font-size: 22px; margin-bottom: 15px; }
        p { color: #ccc; margin-bottom: 25px; line-height: 1.6; }
        .botao {
            background: #e94560;
            color: white;
            border: none;
            padding: 12px 30px;
            font-size: 16px;
            border-radius: 6px;
            cursor: pointer;
            transition: 0.3s;
        }
        .botao:hover { background: #ff6b6b; }
        .escondido { display: none; }
        .susto { font-size: 60px; margin: 20px 0; }
        h2 { color: #4ade80; font-size: 28px; }
    </style>
</head>
<body>
    <div class="caixa" id="pagina1">
        <div class="alerta">⚠️</div>
        <h1>SEU COMPUTADOR FOI BLOQUEADO!</h1>
        <p>Detectamos vírus no seu sistema. Clique abaixo para resolver agora:</p>
        <button class="botao" onclick="revelar()">🔧 Remover Vírus</button>
    </div>

    <div class="caixa escondido" id="pagina2">
        <div class="susto">😆</div>
        <h2>PEGADINHA!!!</h2>
        <p>Relaxa, está tudo certo! 😂<br>Não tem nenhum vírus aqui, foi só brincadeira!</p>
        <button class="botao" style="background: #4ade80;" onclick="window.close()">😅 Que susto, hein?</button>
    </div>

    <script>
        function revelar() {
            document.getElementById('pagina1').style.display = 'none';
            document.getElementById('pagina2').style.display = 'block';
        }
    </script>
</body>
</html>
cd ~/meus-projetos/minha-pagina
nano pegadinha.html
python -m http.server 9090



