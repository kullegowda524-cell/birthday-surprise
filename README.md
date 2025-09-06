<!DOCTYPE html><html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Happy Birthday Sister 🎉</title>
  <style>
    body {
      margin: 0;
      font-family: 'Poppins', sans-serif;
      display: flex;
      justify-content: center;
      align-items: center;
      height: 100vh;
      background: linear-gradient(135deg, #ff9a9e, #fad0c4);
      overflow: hidden;
      color: white;
      text-align: center;
    }
    .container {
      max-width: 90%;
    }
    h1, h2, p {
      animation: fadeIn 2s ease;
    }
    button {
      margin-top: 20px;
      padding: 10px 20px;
      border: none;
      border-radius: 20px;
      font-size: 18px;
      cursor: pointer;
      background: #fff;
      color: #ff4b5c;
      font-weight: bold;
    }
    @keyframes fadeIn {
      from { opacity: 0; transform: translateY(20px); }
      to { opacity: 1; transform: translateY(0); }
    }
    canvas {
      position: absolute;
      top: 0;
      left: 0;
      width: 100%;
      height: 100%;
      pointer-events: none;
    }
  </style>
</head>
<body>
  <div class="container" id="content">
    <h1>🎉 Happy Birthday Sister! 🎉</h1>
    <p>Click below to unlock your surprises 💝</p>
    <button onclick="nextPage()">Next Surprise 🎁</button>
  </div><canvas id="canvas"></canvas>

  <script>
    let page = 1;
    const content = document.getElementById('content');

    function nextPage() {
      page++;
      switch(page) {
        case 2:
          content.innerHTML = `<h1>🎂 Here’s a Cake for You 🎂</h1><p>Make a wish and blow the candles!</p><button onclick="nextPage()">Next Surprise 🎁</button>`;
          break;
        case 3:
          content.innerHTML = `<h1>🎈 Balloons for My Lovely Sister 🎈</h1><p>Let them rise high like your dreams!</p><button onclick="nextPage()">Next Surprise 🎁</button>`;
          break;
        case 4:
          content.innerHTML = `<h1>💖 Message 💖</h1><p>You are My Favourite Sister forever 💖♾️</p><button onclick="nextPage()">Next Surprise 🎁</button>`;
          break;
        case 5:
          content.innerHTML = `<h1>🌸 Flowers Bloom For You 🌸</h1><p>Because you deserve all beauty in life!</p><button onclick="nextPage()">Next Surprise 🎁</button>`;
          break;
        case 6:
          content.innerHTML = `<h1>🎶 Music in the Air 🎶</h1><p>Life with you is a melody!</p><button onclick="nextPage()">Next Surprise 🎁</button>`;
          break;
        case 7:
          content.innerHTML = `<h1>📸 Memory Frame 📸</h1><p>I’ll always cherish our bond 💕</p><button onclick="nextPage()">Next Surprise 🎁</button>`;
          break;
        case 8:
          content.innerHTML = `<h1>✨ Stars Just for You ✨</h1><p>You shine the brightest in my world 🌟</p><button onclick="nextPage()">Next Surprise 🎁</button>`;
          break;
        case 9:
          content.innerHTML = `<h1>💌 Special Note 💌</h1><p>Two souls one heart 🌍 You are my best sister!</p><button onclick="nextPage()">Next Surprise 🎁</button>`;
          break;
        case 10:
          content.innerHTML = `<h1>🎊 Final Surprise 🎊</h1><p>I Love You Sis 💕 Forever</p><button onclick="nextPage()">Replay Surprises 🔄</button>`;
          page = 0; // reset
          break;
      }
    }
  </script></body>
</html>
