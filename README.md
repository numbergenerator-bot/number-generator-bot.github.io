<!DOCTYPE html>
<html lang="it">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Generatore di Numeri</title>
</head>
<body>
    <h1>Generatore di Numeri</h1>
    <p>Genera un numero fra:</p>
    
    <input type="number" id="minNumero" placeholder="Min" min="1">
    <input type="number" id="maxNumero" placeholder="Max" max="28">
    <button onclick="generaNumero()">Genera</button>
    
    <p id="risultato"></p>

    <script>
        function generaNumero() {
            var min = document.getElementById("minNumero").value;
            var max = document.getElementById("maxNumero").value;
            var numeroPreimpostato = 15; // Cambia questo numero con quello che vuoi sempre ottenere
            
            if (min !== "" && max !== "" && Number(min) < Number(max)) {
                document.getElementById("risultato").innerText = "Numero generato: " + numeroPreimpostato;
            } else {
                document.getElementById("risultato").innerText = "Per favore, inserisci un intervallo valido.";
            }
        }
    </script>
</body>
</html>
