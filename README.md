# index.html-
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <title>Valentine Proposal ❤️</title>
  <style>
    body {
      margin: 0;
      height: 100vh;
      display: flex;
      justify-content: center;
      align-items: center;
      background: linear-gradient(135deg, #ff4b7d, #ff85a2);
      font-family: Arial, sans-serif;
      color: white;
    }

    .card {
      background: rgba(255, 255, 255, 0.15);
      padding: 40px;
      border-radius: 20px;
      text-align: center;
      box-shadow: 0 10px 25px rgba(0,0,0,0.2);
    }

    h1 {
      font-size: 2.5rem;
      margin-bottom: 10px;
    }

    h2 {
      margin-bottom: 30px;
    }

    button {
      padding: 12px 25px;
      font-size: 18px;
      border: none;
      border-radius: 25px;
      cursor: pointer;
      margin: 10px;
    }

    #yes {
      background-color: #28a745;
      color: white;
    }

    #no {
      background-color: #dc3545;
      color: white;
      position: absolute;
    }

    #msg {
      margin-top: 25px;
      font-size: 22px;
    }
  </style>
</head>
<body>

  <div class="card">
    <h1>Hey ❤️</h1>
    <h2>Will you be my Valentine?</h2>

    <button id="yes">Yes 😍</button>
    <button id="no">No 🙈</button>

    <div id="msg"></div>
  </div>

  <script>
    const noBtn = document.getElementById("no");
    const yesBtn = document.getElementById("yes");
    const msg = document.getElementById("msg");

    noBtn.addEventListener("mouseover", () => {
      const x = Math.random() * (window.innerWidth - 100);
      const y = Math.random() * (window.innerHeight - 100);
      noBtn.style.left = x + "px";
      noBtn.style.top = y + "px";
    });

    yesBtn.addEventListener("click", () => {
      msg.innerHTML = "Yayyy! ❤️🥰 You made my day!";
    });
  </script>

</body>
</html>
