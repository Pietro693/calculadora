# calculadora
calc
<!DOCTYPE html>
<html lang="pt-br">
<head>
    <meta charset="UTF-8">
    <title>Soma Web</title>
    <style>
        body { font-family: sans-serif; text-align: center; padding-top: 50px; }
        input { padding: 10px; margin: 10px; }
        button { padding: 10px 20px; cursor: pointer; }
    </style>
</head>
<body>
    <h2>Minha Calculadora</h2>
    <input type="number" id="numero" placeholder="Digite um número">
    <button onclick="adicionar()">Somar</button>
    <p id="resultado">A soma total é: 0</p>

    <script>
        let soma = 0;
        function adicionar() {
            let num = parseInt(document.getElementById('numero').value);
            if (!isNaN(num)) {
                soma += num;
                document.getElementById('resultado').innerText = "A soma total é: " + soma;
            }
        }
    </script>
</body>
</html>
