<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <title>Shivani</title>
  <meta name="viewport" content="width=device-width, initial-scale=1.0">

  <style>
    body {
      margin: 0;
      height: 100vh;
      background: #fff;
      display: flex;
      justify-content: center;
      align-items: center;
      font-family: -apple-system, BlinkMacSystemFont, "Segoe UI", sans-serif;
      color: #333;
    }

    .box {
      text-align: center;
      max-width: 420px;
      padding: 30px;
      animation: fade 1.2s ease;
    }

    h1 {
      font-size: 32px;
      margin-bottom: 20px;
      font-weight: 600;
    }

    p {
      font-size: 18px;
      line-height: 1.7;
      margin: 15px 0;
      color: #555;
    }

    .question {
      font-size: 20px;
      margin-top: 30px;
      color: #000;
      font-weight: 500;
    }

    button {
      margin-top: 30px;
      padding: 14px 36px;
      font-size: 16px;
      border-radius: 30px;
      border: none;
      cursor: pointer;
      background: #ff4d6d;
      color: white;
      transition: transform 0.2s ease, box-shadow 0.2s ease;
    }

    button:hover {
      transform: translateY(-2px);
      box-shadow: 0 8px 20px rgba(255, 77, 109, 0.3);
    }

    @keyframes fade {
      from { opacity: 0; transform: translateY(20px); }
      to { opacity: 1; transform: translateY(0); }
    }
  </style>
</head>
<body>

  <div class="box" id="content">
    <h1>Hi Shivani,</h1>

    <p>
      I’ve thought a lot about how to say this.
    </p>

    <p>
      You’re someone who makes moments feel lighter  
      and conversations feel easier.
    </p>

    <p>
      I don’t want anything dramatic.  
      Just something honest.
    </p>

    <div class="question">
      Will you be my Valentine?
    </div>

    <button onclick="yes()">Yes</button>
  </div>

  <script>
    function yes() {
      document.getElementById("content").innerHTML = `
        <h1>Thank you ❤️</h1>
        <p>
          This means more to me than you know.
        </p>
        <p>
          I’m really glad it’s you.
        </p>
      `;
    }
  </script>

</body> 
</html>
