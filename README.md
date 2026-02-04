<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<title>Valentine 💖</title>

<style>
body {
  background: #ffe6ee;
  font-family: Arial, sans-serif;
  text-align: center;
  padding-top: 100px;
}

h1 {
  color: #d6336c;
}

button {
  padding: 15px 25px;
  font-size: 18px;
  border: none;
  border-radius: 12px;
  cursor: pointer;
  margin: 20px;
}

#yes {
  background-color: #ff4d6d;
  color: white;
}

#no {
  background-color: #999;
  color: white;
  position: absolute;
}
</style>
</head>

<body>

<h1>💖 Ayouba, will you be my Valentine? 💖</h1>

<button id="yes" onclick="yesClick()">Yes 💕</button>
<button id="no" onmouseover="moveNo()">No 🙈</button>

<script>
function yesClick() {
  document.body.innerHTML =
    "<h1>💘 Yayyy! 💘</h1><p>You just made my heart happy ❤️</p>";
}

function moveNo() {
  var x = Math.random() * (window.innerWidth - 100);
  var y = Math.random() * (window.innerHeight - 100);
  var btn = document.getElementById("no");
  btn.style.left = x + "px";
  btn.style.top = y + "px";
}
</script>

</body>
</html>
