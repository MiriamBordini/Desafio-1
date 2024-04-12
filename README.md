# Desafio-1
```
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Calculadora de Despesas e Simulador de Financiamentos</title>
    <style>
       /* Estilize a interface conforme sua preferência */
       body { 
            font-family: 'Times New Roman', Times, serif, sans-serif, Courier;
            text-align: center;
            background: linear-gradient(90deg,  #b8bfd0, #6878a1); 
            color: #ffffff; /* Cor do texto */
            margin: 0; /* Remova margens para evitar espaços brancos */
            padding: 0; /* Remova preenchimentos */

        }
        input {
            width: 100%;
            padding: 10px;
            margin-bottom: 10px;
       
        }
    </style>
</head>
<body>
    <h1>Calculadora de Despesas </h1>

    <!-- Desafio 01: Cálculo e Estimativa de Despesas -->
    <h2>Cálculo e Estimativa de Despesas</h2>
    <label for="aluguel">Aluguel:</label>
    <input type="number" id="aluguel">
    <label for="agua">agua:</label>
    <input type="number" id="agua">
    <label for="Energia">Energia:</label>
    <input type="number" id="energia">
    <label for="Imposto">Imposto:</label>
    <input type="number" id="im">
    <label for="Folha de Pagamento">Folha de Pagamento:</label>
    <input type="number" id="fo">
    <!-- Adicione campos para outros gastos (água, energia elétrica, etc.) -->
    <button onclick="calcularGastos()">Calcular</button>
    <p>Total de Gastos: <span id="totalGastos"></span></p>
    <p>Média de Gastos: <span id="mediaGastos"></span></p>
    <p>Estimativa Anual: <span id="estimativaAnual"></span></p>

  

    <script>
        function calcularGastos() {
            const aluguel = parseFloat(document.getElementById('aluguel').value);
            const agua = parseFloat(document.getElementById('agua').value);
            const energia = parseFloat(document.getElementById('energia').value);
            const im = parseFloat(document.getElementById('im').value);
            const fo = parseFloat(document.getElementById('fo').value);
            // Adicione outros campos de entrada aqui

            // Cálculos
            const totalGastos = aluguel + agua + energia + im + fo; // Adicione os outros gastos aqui
            const mediaGastos = totalGastos; // Divida pelo número de gastos
            const estimativaAnual = totalGastos * 12;

            // Exiba os resultados
            document.getElementById('totalGastos').textContent = `$${totalGastos.toFixed(2)}`;
            document.getElementById('mediaGastos').textContent = `$${mediaGastos.toFixed(2)}`;
            document.getElementById('estimativaAnual').textContent = `$${estimativaAnual.toFixed(2)}`;

        }

      
    </script>
</body>
</html>

Integrantes do grupo: Bia Vizeu, Heloísa, Duda Silva, Lucas Colombo, Míriam.
```
