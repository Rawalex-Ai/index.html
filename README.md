<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <title>For Shivani ❤️</title>
  <meta name="viewport" content="width=device-width, initial-scale=1.0">

  <style>
    body {
      margin: 0;
      height: 100vh;
      background: linear-gradient(135deg, #ff5f6d, #ffc371);
      display: flex;
      justify-content: center;
      align-items: center;
      font-family: 'Segoe UI', sans-serif;
      overflow: hidden;
      color: white;
    }

    .card {
      background: rgba(255, 255, 255, 0.15);
      padding: 30px;
      border-radius: 25px;
      text-align: center;
      width: 90%;
      max-width: 400px;
      box-shadow: 0 20px 40px rgba(0,0,0,0.2);
      backdrop-filter: blur(10px);
    }

    h1 {
      font-size: 32px;
      margin-bottom: 10px;
    }

    p {
      font-size: 18px;
      margin: 10px 0;
    }

    button {
      margin: 15px;
      padding: 14px 28px;
      font-size: 18px;
      border: none;
      border-radius: 30px;
      cursor: pointer;
      transition: transform 0.2s;
    }

    button:hover {
      transform: scale(1.1);
    }

    #yes {
      background: #2ecc71;
      color: white;
    }

    #no {
      background: #e74c3c;
      color: white;
      position: absolute;
    }

    .heart {
      position: absolute;
      color: rgba(255,255,255,0.8);
      font-size: 20px;
      animation: floatUp 6s linear infinite;
    }

    @keyframes floatUp {
      from {
        transform: translateY(100vh);
        opacity: 1;
      }
      to {
        transform: translateY(-10vh);
        opacity: 0;
      }
    }
  </style>
</head>
<body>

  <div class="card" id="card">
    <h1>Hi Shivani ❤️</h1>
    <p>Every smile of yours makes my day brighter.</p>
    <p>I have something important to ask you…</p>
    <p><strong>Will you be my Valentine? 🌹</strong></p>

    <button id="yes" onclick="yesClicked()">Yes 💕</button>
    <button id="no" onmouseover="moveNo()">No 🙈</button>
  </div>

  <script>
    function moveNo() {
      const noBtn = document.getElementById("no");
      noBtn.style.left = Math.random() * 80 + "vw";
      noBtn.style.top = Math.random() * 80 + "vh";
    }

    function yesClicked() {
      document.getElementById("card").innerHTML = `
        <h1>She said YES 💖</h1>
        <p>I knew it, Shivani 😍</p>
        <p>You just made my heart the happiest.</p>
        <p>Happy Valentine’s Day ❤️</p>
      `;
    }

    // Floating hearts
    setInterval(() => {
      const heart = document.createElement("div");
      heart.className = "heart";
      heart.innerHTML = "💖";
      heart.style.left = Math.random() * 100 + "vw";
      heart.style.fontSize = (15 + Math.random() * 20) + "px";
      document.body.appendChild(heart);

      setTimeout(() => {
        heart.remove();
      }, 6000);
    }, 300);
  </script>

</body>
</html>
