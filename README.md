
<html lang="en">
<head>
  <meta charset="UTF-8">
  <title>Valentine Question 💖</title>
  <style>
    body {
      height: 100vh;
      display: flex;
      justify-content: center;
      align-items: center;
      font-family: 'Comic Sans MS', cursive, sans-serif;
      background: linear-gradient(135deg, #ff9a9e, #fad0c4);
    }

    .container {
      text-align: center;
    }

    h1 {
      color: #b30059;
      margin-bottom: 30px;
    }

    .buttons {
      position: relative;
      height: 120px;
    }

    button {
      padding: 12px 28px;
      font-size: 18px;
      border: none;
      border-radius: 8px;
      cursor: pointer;
    }

    #yesBtn {
      background-color: #ff4d6d;
      color: white;
      margin-right: 200px;
    }

    #noBtn {
      background-color: #555;
      color: white;
      position: absolute;
      left: 140px;
    }

    #gif {
      display: none;
      margin-top: 30px;
    }

    #gif img {
      width: 250px;
      border-radius: 12px;
    }
  </style>
</head>
<body>

  <div class="container">
    <h1>Husna, will you be my Valentine? 💘</h1>

    <div class="buttons">
      <button id="yesBtn">Yes 💖</button>
      <button id="noBtn">No 🙈</button>
    </div>

    <div id="gif">
      <h2>Yayyyy! 💃🕺</h2>
      <img src="https://media.giphy.com/media/l0MYt5jPR6QX5pnqM/giphy.gif" alt="Dancing GIF">
    </div>
  </div>

  <script>
    const noBtn = document.getElementById("noBtn");
    const yesBtn = document.getElementById("yesBtn");
    const gif = document.getElementById("gif");

    // Make NO button run away
    noBtn.addEventListener("mouseenter", () => {
      const maxX = 300;
      const maxY = 80;

      const randomX = Math.floor(Math.random() * maxX);
      const randomY = Math.floor(Math.random() * maxY);

      noBtn.style.left = randomX + "px";
      noBtn.style.top = randomY + "px";
    });

    // YES button click
    yesBtn.addEventListener("click", () => {
      gif.style.display = "block";
    });
  </script>

</body>
</html>
