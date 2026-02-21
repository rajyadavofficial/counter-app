index.html
<!DOCTYPE html>
<html>
<head>
  <title>Raj Counter App</title>
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <style>
    body {
      text-align: center;
      font-family: Arial;
      margin-top: 100px;
    }
    h1 {
      font-size: 40px;
    }
    button {
      padding: 10px 20px;
      margin: 10px;
      font-size: 18px;
    }
  </style>
</head>
<body>

  <h1 id="count">0</h1>

  <button onclick="increase()">+5</button>
  <button onclick="decrease()">-5</button>
  <button onclick="reset()">Reset</button>

  <script>
    let count = 0;

    function increase() {
      count += 5;
      document.getElementById("count").innerText = count;
    }

    function decrease() {
      count -= 5;
      document.getElementById("count").innerText = count;
    }

    function reset() {
      count = 0;
      document.getElementById("count").innerText = count;
    }
  </script>

</body>
</html>
