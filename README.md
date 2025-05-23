# im.like.that.yo.03921
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <title>PlayZone - Games & Web</title>
  <style>
    body {
      font-family: Arial, sans-serif;
      background-color: #1c1c1c;
      color: #ffffff;
      margin: 0;
      padding: 0;
    }
    header {
      background-color: #2a2a2a;
      padding: 20px;
      text-align: center;
    }
    h1 {
      margin: 0;
      color: #4caf50;
    }
    .section {
      padding: 20px;
    }
    .games {
      display: flex;
      gap: 20px;
      flex-wrap: wrap;
      justify-content: center;
    }
    .game {
      background-color: #333333;
      padding: 10px;
      width: 200px;
      text-align: center;
      border-radius: 8px;
    }
    .game img {
      width: 100%;
      border-radius: 5px;
    }
    .game a {
      display: block;
      margin-top: 10px;
      color: #4caf50;
      text-decoration: none;
    }
    .browser {
      margin-top: 40px;
      text-align: center;
    }
    .browser input {
      width: 60%;
      padding: 8px;
      border-radius: 5px;
      border: none;
    }
    .browser button {
      padding: 8px 16px;
      border: none;
      background-color: #4caf50;
      color: white;
      border-radius: 5px;
      cursor: pointer;
    }
    .browser iframe {
      width: 100%;
      height: 600px;
      border: none;
      margin-top: 10px;
    }
  </style>
</head>
<body>
  <header>
    <h1>PlayZone</h1>
    <p>Top Games + Mini Browser</p>
  </header>

  <div class="section">
    <h2>Popular Games</h2>
    <div class="games">
      <div class="game">
        <img src="https://via.placeholder.com/200x120?text=Crazy+Cattle+3D" alt="Crazy Cattle 3D">
        <a href="https://crazycattle3d.com/" target="_blank">Play Crazy Cattle 3D</a>
      </div>
      <div class="game">
        <img src="https://via.placeholder.com/200x120?text=Slope" alt="Slope">
        <a href="https://slopegame3d.io/" target="_blank">Play Slope</a>
      </div>
      <div class="game">
        <img src="https://via.placeholder.com/200x120?text=Retro+Bowl" alt="Retro Bowl">
        <a href="https://retro-bowl.gg/" target="_blank">Play Retro Bowl</a>
      </div>
    </div>
  </div>

  <div class="section browser">
    <h2>Mini Web Browser</h2>
    <input id="urlInput" type="text" placeholder="Enter a website (https://...)" />
    <button onclick="loadSite()">Go</button>
    <iframe id="browserFrame" src=""></iframe>
  </div>

  <script>
    function loadSite() {
      const url = document.getElementById('urlInput').value;
      document.getElementById('browserFrame').src = url;
    }
  </script>
</body>
</html>
