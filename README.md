<!DOCTYPE html>  <html lang="as">  
<head>  
  <meta charset="UTF-8" />  
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />  
  <title>RK Gaming Spin</title>  
  <style>  
    body {  
      font-family: sans-serif;  
      background: #0f172a;  
      color: white;  
      text-align: center;  
      padding: 30px;  
    }  
    .wheel {  
      width: 300px;  
      height: 300px;  
      border-radius: 50%;  
      border: 10px solid #22d3ee;  
      margin: 30px auto;  
      position: relative;  
      background: conic-gradient(  
        #4ade80 0deg 90deg,  
        #facc15 90deg 180deg,  
        #60a5fa 180deg 270deg,  
        #f87171 270deg 360deg  
      );  
      transition: transform 5s ease-out;  
    }  
    .button {  
      background: #22c55e;  
      border: none;  
      padding: 12px 25px;  
      color: white;  
      font-size: 18px;  
      border-radius: 8px;  
      cursor: pointer;  
      margin-top: 20px;  
    }  
    .result {  
      font-size: 20px;  
      margin-top: 20px;  
    }  
    .share {  
      background: #25d366;  
      color: white;  
      text-decoration: none;  
      display: inline-block;  
      margin-top: 20px;  
      padding: 10px 20px;  
      border-radius: 6px;  
      font-weight: bold;  
    }  
  </style>  
</head>  
<body>  
  <h1>🎮 RK Gaming Spin to Win 🎁</h1>  
  <div class="wheel" id="wheel"></div>  
  <button class="button" onclick="spinWheel()">🔄 চকৰি ঘূৰাওক</button>  
  <div class="result" id="result"></div>  
  <a id="shareBtn" class="share" href="#" target="_blank">📤 WhatsAppত Share কৰক</a>    <script>  
    const wheel = document.getElementById("wheel");  
    const result = document.getElementById("result");  
    const shareBtn = document.getElementById("shareBtn");  
  
    const prizes = [  
      "₹299 Jio Recharge",  
      "1GB Net Pack",  
      "5GB Net Pack",  
      "₹499 Recharge"  
    ];  
  
    function spinWheel() {  
      const angle = 3600 + Math.floor(Math.random() * 360);  
      wheel.style.transform = `rotate(${angle}deg)`;  
  
      const prizeIndex = Math.floor(((angle % 360) / 90));  
      const selectedPrize = prizes[prizeIndex];  
  
      setTimeout(() => {  
        result.innerText = `আপুনি জিকিছে: 🎉 ${selectedPrize} 🎁`;  
        const shareText = encodeURIComponent(  
          `মই RK Gaming Spin ত ${selectedPrize} জিকিলোঁ! আপুনি চেষ্টা কৰক: https://rkgaming18.github.io/rkgamingzone18/`
        shareBtn.href = `https://wa.me/?text=${shareText}`;  
      }, 5200);  
    }  
  </script>  </body>  
</html>

