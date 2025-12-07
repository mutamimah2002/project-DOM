<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <meta http-equiv="X-UA-Compatible" content="ie=edge">
  <title>Tugas Mutamimah</title>
</head>
<body>
    <h1 id="judul">Mutamimah</h1>
  <button onclick="changeColor()">Ganti Warna</button>
  <input type="color" id="colorPicker" onchange="setCustomColor()">

  <script>
    const colors = ["red", "blue", "green", "purple", "orange", "pink"];
    let index = 0;

    function changeColor() {
      const h1 = document.getElementById("judul");
      h1.style.color = colors[index];
       index = (index + 1) % colors.length;
    }

    function setCustomColor() {
      const custom = document.getElementById("colorPicker").value;
      document.getElementById("judul").style.color = custom;
    }
  </script>
</body>
</html>
