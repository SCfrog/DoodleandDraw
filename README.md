# DoodleandDraw

<html>
<body>
  <title>Doodle & Draw!</title>
  <link rel="icon" href="http://www.clipartbest.com/cliparts/y9c/zRg/y9czRgRTE.png">
  <link rel="preconnect" href="https://fonts.googleapis.com">
<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
<link href="https://fonts.googleapis.com/css2?family=Titan+One&display=swap" rel="stylesheet">
  <h1>Doodle & Draw!</h1>
  <canvas id="imgCanvas" width="1500" height="1000"
  onclick="draw(event)" onmousemove="draw(event)"> </canvas>

  <style>
    body{
      background-image: url("https://static.vecteezy.com/system/resources/previews/000/532/483/original/paper-line-vector-background-detailed-lined-paper-texture.jpg");
      background-size: 130%;
    }
    h1{
        text-align: center;
        font-family: 'Titan One', cursive;
        font-size: 70px;
      }

  </style>

  <script>

  function draw(e){
    var canvas = document.getElementById("imgCanvas");
    var ctx = canvas.getContext("2d");
    var rect = canvas.getBoundingClientRect();
    var posx = e.clientX - rect.left;
    var posy = e.clientY - rect.top;
    ctx.fillStyle = "Black"
    ctx.beginPath();
    ctx.arc(posx, posy, 20, 0, Math.PI * 2);
    ctx.fill();
    ctx.strokeStyle = "Black";
    ctx.beginPath();
    ctx.arc(posx, posy, 20, 0, Math.PI * 2);
    ctx.stroke();
  }
  </script>
</body>
</html>
