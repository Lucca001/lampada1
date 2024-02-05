<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Lâmpada</title>
  <style>
    body {
      display: flex;
      justify-content: center;
      align-items: center;
      height: 100vh;
      margin: 0;
    }

    #lampada {
      width: 100px;
      height: 200px;
      background-color: #f0f0f0;
      border: 5px solid #ddd;
      border-radius: 10px;
      position: relative;
    }

    #bulbo {
      width: 80px;
      height: 80px;
      background-color: #f0f0f0;
      border: 5px solid #ddd;
      border-radius: 50%;
      position: absolute;
      top: 30px;
      left: 50%;
      transform: translateX(-50%);
    }

    #fio {
      width: 5px;
      height: 100px;
      background-color: #ddd;
      position: absolute;
      top: 110px;
      left: 50%;
      transform: translateX(-50%);
    }

    #interruptor {
      display: block;
      margin-top: 20px;
      padding: 10px;
      font-size: 16px;
      cursor: pointer;
    }
  </style>
</head>
<body>
  <div id="lampada">
    <div id="bulbo"></div>
    <div id="fio"></div>
  </div>

  <button id="interruptor" onclick="toggleLamp()">Interruptor</button>

  <script>
    function toggleLamp() {
      var lampada = document.getElementById('lampada');
      lampada.classList.toggle('ligada');
    }
  </script>
</body>
</html>
