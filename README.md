<html lang="en">
<head>
  <meta charset="UTF-8">
  <title>For Sev ❤️</title>
  <style>
    body {
      margin: 0;
      padding: 0;
      font-family: 'Comic Sans MS', cursive, sans-serif;
      background: linear-gradient(135deg, #ffb6c1, #ffe4e1);
      display: flex;
      justify-content: center;
      align-items: center;
      min-height: 100vh;
      text-align: center;
    }

    .card {
      background: white;
      padding: 40px;
      border-radius: 25px;
      box-shadow: 0 10px 25px rgba(0,0,0,0.2);
      max-width: 440px;
    }

    h1 {
      color: #ff69b4;
      margin-bottom: 10px;
    }

    p {
      color: #555;
      font-size: 17px;
      line-height: 1.6;
    }

    .heart {
      font-size: 60px;
      animation: beat 1s infinite;
      margin: 20px 0;
      cursor: pointer;
    }

    @keyframes beat {
      0% { transform: scale(1); }
      50% { transform: scale(1.2); }
      100% { transform: scale(1); }
    }

    .letter, .countdown, .daily-message, .music, .secret {
      background: #fff0f5;
      padding: 20px;
      border-radius: 15px;
      margin-top: 20px;
      font-size: 16px;
    }

    .countdown span {
      font-weight: bold;
      color: #ff1493;
    }

    .secret {
      display: none;
      margin-top: 15px;
      border: 2px dashed #ff69b4;
    }

    button {
      background: #ff69b4;
      border: none;
      padding: 12px 22px;
      border-radius: 20px;
      color: white;
      font-size: 16px;
      cursor: pointer;
      margin-top: 20px;
    }

    button:hover {
      background: #ff1493;
    }

    footer {
      margin-top: 20px;
      font-size: 14px;
      color: #999;
    }
  </style>
</head>
<body>

  <div class="card">
    <h1>Hi Sev 💕</h1>

    <p>
      This little website is just for you.<br>
      I made it with all my heart.
    </p>

    <div class="heart" onclick="revealSecret()">❤️</div>

    <div class="letter">
      <p>
        Sev, I just want you to know that I'm so lucky to have you.
        You mean so much to me.
        I can't lose you again. Never again. 
        
      </p>
      <p>
        Even if you’re far away, I’ll make sure you always feel how much I care.
      </p>
      <p>
        <strong>See you soon, baby.</strong> 💖
      </p>
    </div>

    <div class="countdown">
      ⏳ <span id="timer"></span> until I see you, Sev 🥰
    </div>

    <div class="daily-message">
      💌 <strong>Message of the Day:</strong>
      <p id="dailyMessage"></p>
    </div>

    <div class="music">
  🎶 <strong>This song reminds me of you</strong><br><br>
  <iframe style="border-radius:12px"
    src="https://open.spotify.com/embed/track/0l13vtSXzPAKJ2m3q3WXX8"
    width="100%" height="80"
    frameBorder="0"
    allow="autoplay; clipboard-write; encrypted-media; fullscreen; picture-in-picture">
  </iframe>
  <p><em>“One Only” – Pamungkas</em></p>
</div>

</div class="secret" id="secretMessage">
  💞 <strong>For Sev Only:</strong>
  <p>
    I am so sure about you.<br>
    There is no doubt in my heart that you are the one I choose,
    every day and in every lifetime.
  </p>
  <p>
    I can’t wait to be your wife someday.
    well asawa na kita sa kwento 'ko hehehehhe
  </p>
  <p>
    You are my one and only, Baby❤️
  </p>
</div>

<button onclick="alert('I Love You more than you could ever know, Sev ❤️')">
  Click me 🥰
</button>

<footer>
  Made with love 💌
</footer>
  </div>

  <script>
    // COUNTDOWN TO FEB 5, 2026
    const targetDate = new Date("February 5, 2026 00:00:00").getTime();
    const timer = document.getElementById("timer");

    setInterval(() => {
      const now = new Date().getTime();
      const distance = targetDate - now;

      if (distance < 0) {
        timer.innerHTML = "Today is the day ❤️";
        return;
      }

      const days = Math.floor(distance / (1000 * 60 * 60 * 24));
      const hours = Math.floor((distance / (1000 * 60 * 60)) % 24);
      const minutes = Math.floor((distance / (1000 * 60)) % 60);
      const seconds = Math.floor((distance / 1000) % 60);

      timer.innerHTML = `${days}d ${hours}h ${minutes}m ${seconds}s`;
    }, 1000);

    // MESSAGE OF THE DAY
    const messages = [
      "I can’t wait to pay my utang kisses hehe",
      "Don't be pasaway eat your dinner ha!",
      "Always remember that I love you because you are YOU",
      "You are worth every wait, Sev"
    ];

    const today = new Date().getDate();
    document.getElementById("dailyMessage").innerText =
      messages[today % messages.length];

    // HIDDEN MESSAGE
    function revealSecret() {
      const secret = document.getElementById("secretMessage");
      secret.style.display = "block";
    }
  </script>

</body>
</html>
