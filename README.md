<!DOCTYPE html>
<html lang="lt">
<head>
  <meta charset="UTF-8">
  <title>Valentine 💘</title>
  <style>
    body {
      margin: 0;
      height: 100vh;
      display: flex;
      justify-content: center;
      align-items: center;
      background: linear-gradient(135deg, #ffd6e8, #ffeef5);
      font-family: Arial, sans-serif;
    }

    .card {
      background: white;
      padding: 40px;
      border-radius: 20px;
      text-align: center;
      box-shadow: 0 20px 40px rgba(0,0,0,0.1);
      max-width: 350px;
      width: 90%;
    }

    h1 {
      margin-bottom: 30px;
    }

    button {
      font-size: 18px;
      padding: 12px 24px;
      border: none;
      border-radius: 12px;
      cursor: pointer;
      margin: 10px;
      transition: all 0.2s ease;
    }

    #yes {
      background: #ff4d88;
      color: white;
    }

    #no {
      background: #ddd;
      position: absolute;
    }

    .heart {
      font-size: 60px;
      margin-bottom: 20px;
    }
  </style>
</head>
<body>

  <div class="card">
    <div class="heart">💘</div>
    <h1>Samanta,<br>ar būsi mano Valentine?</h1>
    <button id="yes">Taip 💖</button>
    <button id="no">Ne 😅</button>
  </div>

  <script>
    const noBtn = document.getElementById("no");
    const yesBtn = document.getElementById("yes");

    noBtn.addEventListener("mouseover", () => {
      const x = Math.random() * (window.innerWidth - 100);
      const y = Math.random() * (window.innerHeight - 50);
      noBtn.style.left = x + "px";
      noBtn.style.top = y + "px";
    });

    yesBtn.addEventListener("click", () => {
      document.body.innerHTML = `
        <div style="
          display:flex;
          justify-content:center;
          align-items:center;
          height:100vh;
          background: linear-gradient(135deg, #ffb6d5, #ffeef5);
          font-family: Arial;
          text-align:center;
        ">
          <div>
            <h1>💖 Jėėė! 💖</h1>
            <p style="font-size:22px;">
              Geriausias sprendimas ever 😘<br>
              Myliu tave ❤️
            </p>
          </div>
        </div>
      `;
    });
  </script>

</body>
</html>
