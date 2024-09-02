<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>A Complex Game</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            text-align: center;
            margin-top: 50px;
        }
        #number-display {
            font-size: 2em;
            margin-bottom: 20px;
        }
        .button {
            margin: 5px;
            padding: 10px;
            font-size: 1em;
        }
    </style>
</head>
<body>
    <div id="number-display">(0)</div>
    <button class="button" onclick="increment(1)">+1</button>
    <button class="button" onclick="increment(5)">+5</button>
    <button class="button" onclick="increment(10)">+10</button>
    
    <script>
        let number = 0;
        const display = document.getElementById('number-display');
        
        function increment(n) {
            number += n;
            display.textContent = `(${number})`;
        }
    </script>
</body>
</html>

