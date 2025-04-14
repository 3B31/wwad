<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Modern Calculator</title>
    <style>
        body {
            display: flex;
            justify-content: center;
            align-items: center;
            height: 100vh;
            background-color: #282c34;
            font-family: 'Arial', sans-serif;
        }
        #calculator {
            width: 360px;
            background: #ffffff;
            border-radius: 15px;
            box-shadow: 0 10px 30px rgba(0, 0, 0, 0.2);
            padding: 20px;
        }
        input[type="text"] {
            width: 100%;
            padding: 20px;
            font-size: 32px;
            border: none;
            border-radius: 10px;
            margin-bottom: 20px;
            text-align: right;
            background-color: #f0f0f0;
        }
        button {
            width: 80px;
            height: 80px;
            font-size: 24px;
            margin: 10px;
            border: none;
            border-radius: 10px;
            background-color: #61dafb;
            color: #282c34;
            cursor: pointer;
            transition: background-color 0.3s, transform 0.1s;
        }
        button:hover {
            background-color: #21a1f1;
        }
        button:active {
            transform: scale(0.95);
        }
        .button-row {
            display: flex;
            justify-content: center;
        }
    </style>
</head>
<body>
    <div id="calculator">
        <input type="text" id="result" disabled>
        <div class="button-row">
            <button onclick="clearResult()">C</button>
            <button onclick="appendToResult('7')">7</button>
            <button onclick="appendToResult('8')">8</button>
            <button onclick="appendToResult('9')">9</button>
            <button onclick="appendToResult('/')">÷</button>
        </div>
        <div class="button-row">
            <button onclick="appendToResult('4')">4</button>
            <button onclick="appendToResult('5')">5</button>
            <button onclick="appendToResult('6')">6</button>
            <button onclick="appendToResult('*')">×</button>
        </div>
        <div class="button-row">
            <button onclick="appendToResult('1')">1</button>
            <button onclick="appendToResult('2')">2</button>
            <button onclick="appendToResult('3')">3</button>
            <button onclick="appendToResult('-')">−</button>
        </div>
        <div class="button-row">
            <button onclick="appendToResult('0')">0</button>
            <button onclick="calculateResult()">=</button>
            <button onclick="appendToResult('+')">+</button>
        </div>
    </div>

    <script>
        function appendToResult(value) {
            document.getElementById('result').value += value;
        }

        function clearResult() {
            document.getElementById('result').value = '';
        }

        function calculateResult() {
            const resultField = document.getElementById('result');
            try {
                resultField.value = eval(resultField.value);
            } catch (e) {
                resultField.value = 'Error';
            }
        }
    </script>
</body>
</html>
