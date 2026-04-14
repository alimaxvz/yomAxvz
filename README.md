<!DOCTYPE html>
<html>
<head>
  <title>My AI Site</title>
  <style>
    body {
      background: linear-gradient(to right, purple, blue);
      color: white;
      text-align: center;
      font-family: Arial;
      padding-top: 100px;
    }
    input, button {
      padding: 10px;
      border-radius: 10px;
      border: none;
    }
    button {
      background: black;
      color: white;
    }
  </style>
</head>

<body>

<h1>🤖 AI Assistant</h1>

<input type="text" id="input" placeholder="Сұрақ жаз">
<button onclick="answer()">Жауап</button>

<p id="result"></p>

<script>
function answer() {
  let text = document.getElementById("input").value;

  let reply = "Қайта жазып көр";

  if (text.includes("дизайн")) {
    reply = "Минимализм және градиент қолдан";
  } else if (text.includes("түс")) {
    reply = "Көк – сенімділік, қызыл – энергия";
  }

  document.getElementById("result").innerText = reply;
}
</script>

</body>
</html>
