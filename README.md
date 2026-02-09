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
      background: radial-gradient(circle at top, #ff9a9e, #fad0c4);
      display: flex;
      justify-content: center;
      align-items: center;
      font-family: 'Georgia', serif;
      color: #fff;
      overflow: hidden;
    }

    .container {
      background: rgba(255, 255, 255, 0.15);
      backdrop-filter: blur(12px);
      border-radius: 30px;
      padding: 40px 30px;
      width: 90%;
      max-width: 420px;
      text-align: center;
      box-shadow: 0 25px 50px rgba(0,0,0,0.25);
      animation: fadeIn 1.2s ease;
    }

    h1 {
      font-size: 30px;
      margin-bottom: 10px;
    }

    p {
      font-size: 18px;
      line-height: 1.6;
      margin: 12px 0;
    }

    .buttons {
      margin-top: 25px;
    }

    button {
      padding: 14px 32px;
      font-size: 17px;
      border: none;
      border-radius: 30px;
      cursor: pointer;
      margin: 10px;
      transition: all 0.3s ease;
    }

    #yes {
      background: linear-gradient(135deg, #43e97b, #38f9d7);
      color: #0b3d2e;
      font-weight: bold;
    }

    #yes:hover {
      transform: scale(1.08);
      box-shadow: 0 0 20px rgba(255,255,255,0.6);
    }

    #no {
      background: rgba(255,255,255,0.3);
      color: #fff;
      position: absolute;
    }

    @keyframes fadeIn {
      from { opacity: 0; transform: translateY(20px); }
      to { opacity: 1; transform: translateY(0); }
    }

    .heart {
      position: absolute;
      font-size: 18px;
      animation: float 6s linear infinite;
      opacity: 0.8;
    }

    @keyframes float {
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

  <div class="container" id="box">
    <h1>Dear Shivani ❤️</h1>
    <p>
      Some people make life brighter without even trying.
    </p>
    <p>
      You are that person for me.
    </p>
    <p>
      And today, I just want to ask you something from my heart…
    </p>
    <p><strong>Will you be my Valentine? 🌹</strong></p>

    <div class="buttons">
      <button id="yes" onclick="yesClicked()">Yes ❤️</button>
      <button id="no" onmouseover="moveNo()">No</button>
    </div>
  </div>

  <script>
    function moveNo() {
      const no = document.getElementById("no");
      no.style.left = Math.random() * 80 + "vw";
      no.style.top = Math.random() * 80 + "vh";
    }

    function yesClicked() {
      document.getElementById("box").innerHTML = `
        <h1>She said YES ❤️</h1>
        <p>
          This moment means more to me than words can say.
        </p>
        <p>
          Thank you for choosing me, Shivani.
        </p>
        <p>
          Happy Valentine’s Day 💖
        </p>
      `;
    }

    // floating hearts
    setInterval(() => {
      const heart = document.createElement("div");
      heart.className = "heart";
      heart.innerHTML = "❤️";
      heart.style.left = Math.random() * 100 + "vw";
      heart.style.fontSize = (14 + Math.random() * 20) + "px";
      document.body.appendChild(heart);
      setTimeout(() => heart.remove(), 6000);
    }, 400);
  </script>

</body>
</html>
