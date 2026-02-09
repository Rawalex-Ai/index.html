# shivani-valentine.html
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <title>For Shivani ❤️</title>
  <style>
    body {
      background: linear-gradient(to right, #ff758c, #ff7eb3);
      font-family: 'Segoe UI', sans-serif;
      text-align: center;
      color: white;
      padding-top: 80px;
    }
    h1 {
      font-size: 40px;
    }
    p {
      font-size: 22px;
    }
    button {
      padding: 15px 30px;
      font-size: 20px;
      border: none;
      border-radius: 30px;
      cursor: pointer;
      margin: 20px;
    }
    #yes {
      background-color: #2ecc71;
      color: white;
    }
    #no {
      background-color: #e74c3c;
      color: white;
      position: absolute;
    }
  </style>
</head>
<body>

  <h1>Hi Shivani ❤️</h1>
  <p>From the moment I met you, my heart knew something special.</p>
  <p>Will you be my Valentine? 🌹</p>

  <button id="yes" onclick="yesClicked()">Yes 💕</button>
  <button id="no" onmouseover="moveNo()">No 😅</button>

  <script>
    function moveNo() {
      const noBtn = document.getElementById("no");
      noBtn.style.left = Math.random() * 80 + "vw";
      noBtn.style.top = Math.random() * 80 + "vh";
    }

    function yesClicked() {
      document.body.innerHTML = `
        <h1>YAY!!! 💖💖💖</h1>
        <p>I knew you’d say YES, Shivani 😍</p>
        <p>You just made me the happiest person today 💘</p>
        <p>Happy Valentine’s Day ❤️</p>
      `;
    }
  </script>

</body>
</html>
