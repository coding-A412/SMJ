<!DOCTYPE html>
<html>
<head>
  <title>Jakaria's Live Sports</title>
  <style>
    /* আগের সব CSS ঠিকই আছে, শুধু নিচে নতুন বাটনের জন্য একটু স্টাইল */
    .server-btns {
      display: flex;
      justify-content: center;
      gap: 12px;
      margin-bottom: 18px;
    }
    .server-btn {
      background: #ff69b4;
      color: #fff;
      border: none;
      border-radius: 6px;
      padding: 7px 18px;
      font-weight: bold;
      cursor: pointer;
      box-shadow: 0 2px 8px #ff69b488;
      transition: background 0.2s;
    }
    .server-btn.active, .server-btn:hover {
      background: #ff1744;
    }
  </style>
</head>
<body>
  <div class="header">
    <a class="tg-link" href="https://www.facebook.com/sheikh.muhammad.639043" target="_blank" title="Join Telegram">
      <img class="tg-logo" src="https://cdn-icons-png.flaticon.com/512/2111/2111646.png" alt="Telegram"/>
    </a>
    <div class="web-name">Jakaria Live TV</div>
    <div class="owner">Owner Jakaria</div>
  </div>

  <div class="section-title">Football And Cricket Live</div>

  <div class="channel-box">
    <div class="circles">
      <div class="circle"></div>
      <div class="circle"></div>
      <div class="circle"></div>
    </div>
    <div class="channel-title">
      Live Sports International <span class="live-dot"></span>
    </div>
    <div class="server-btns">
      <button class="server-btn active" onclick="changeServer(1)">Server 1</button>
      <button class="server-btn" onclick="changeServer(2)">Server 2</button>
      <button class="server-btn" onclick="changeServer(3)">Server 3</button>
      <button class="server-btn" onclick="changeServer(4)">Server 4</button>
    </div>
    <video id="liveVideo" controls autoplay>
      <source src="https://nohddaezronnaz.sbs/automatically/1" type="application/x-mpegURL">
      Your browser does not support the video tag.
    </video>
  </div>
  <script>
    const servers = [
      "http://103.73.107.122:3255/TSportsHD/tracks-v1a1/mono.m3u8",
      "https://edge3-moblive.yuppcdn.net/drm/smil:tencricketdrm.smil/index.m3u8",
      "http://103.15.140.138/tsports/index.m3u8",
      "http://103.73.107.122:3255/TSportsHD/tracks-v1a1/mono.m3u8",
    function changeServer(idx) {
      const video = document.getElementById('liveVideo');
      video.src = servers[idx - 1];
      video.load();
      video.play();
      document.querySelectorAll('.server-btn').forEach((btn, i) => {
        btn.classList.toggle('active', i === idx - 1);
      });
    }
  </script>
</body>
</html>
<html>
<head>
  <title>Jakaria Live TV</title>
  <style>
    body {
      background: #21232b;
      color: #fff;
      font-family: 'Segoe UI', Arial, sans-serif;
      margin: 0;
      padding: 0;
    }
    .header {
      background: #ff69b4;
      display: flex;
      align-items: center;
      justify-content: space-between;
      padding: 18px 22px 12px 18px;
      box-shadow: 0 2px 12px #18181855;
      border-bottom: 3px solid #fff;
    }
    .tg-link {
      display: flex;
      align-items: center;
      text-decoration: none;
      margin-right: 12px;
    }
    .tg-logo {
      width: 36px;
      height: 36px;
      margin-right: 6px;
      vertical-align: middle;
    }
    .web-name {
      flex: 1;
      text-align: center;
      font-size: 2.1em;
      font-weight: bold;
      color: #fff;
      letter-spacing: 2px;
      text-shadow: 0 2px 10px #ff69b488;
    }
    .owner {
      font-size: 1em;
      font-weight: 700;
      background: linear-gradient(90deg, #111 60%, #ff1744 100%);
      color: #fff;
      padding: 4px 16px;
      border-radius: 8px;
      border: 2px solid #ff1744;
      margin-left: 12px;
      letter-spacing: 1.2px;
      text-shadow: 0 2px 8px #0008;
    }
    .section-title {
      text-align: center;
      font-size: 1.4em;
      margin: 32px 0 16px 0;
      color: #ff69b4;
      font-weight: bold;
      letter-spacing: 1px;
      text-shadow: 0 1px 2px #232a34;
    }
    .channel-box {
      background: #282a36;
      max-width: 420px;
      margin: 0 auto 40px auto;
      padding: 34px 16px 24px 16px;
      border-radius: 15px;
      box-shadow: 0 4px 24px #0008, 0 1.5px 8px #222;
      text-align: center;
      border: 1.5px solid #ff69b4;
      position: relative;
    }
    .circles {
      display: flex;
      justify-content: center;
      gap: 10px;
      position: absolute;
      top: -20px;
      left: 0;
      width: 100%;
    }
    .circle {
      width: 18px;
      height: 18px;
      background: #00e676;
      border-radius: 50%;
      border: 2.5px solid #fff;
      box-shadow: 0 0 10px #00e67699;
      display: inline-block;
    }
    .channel-title {
      font-size: 1.15em;
      font-weight: bold;
      margin-bottom: 16px;
      color: #fff;
      letter-spacing: 1px;
      display: flex;
      align-items: center;
      justify-content: center;
      gap: 8px;
    }
    .live-dot {
      width: 10px;
      height: 10px;
      background: #ff1744;
      border-radius: 50%;
      display: inline-block;
      margin-left: 2px;
      box-shadow: 0 0 8px #ff174488;
    }
    video, iframe {
      width: 100%;
      max-width: 370px;
      height: 210px;
      border-radius: 10px;
      background: #000;
      border: 2px solid #ff69b4;
      box-shadow: 0 2px 12px #ff69b466;
    }
  </style>
</head>
<body>
  <div class="header">
    <a class="tg-link" href="https://www.facebook.com/sheikh.muhammad.639043" target="_blank" title="Join Telegram">
      <img class="tg-logo" src="https://cdn-icons-png.flaticon.com/512/2111/2111646.png" alt="Telegram"/>
    </a>
    <div class="web-name">Jakaria Live TV</div>
    <div class="owner">Owner Jakaria</div>
  </div>

  <div class="section-title">Football Live</div>

  <div class="channel-box">
    <div class="circles">
      <div class="circle"></div>
      <div class="circle"></div>
      <div class="circle"></div>
    </div>
    <div class="channel-title">
      PSG VS ATM <span class="live-dot"></span>
    </div>
    <video controls autoplay>
      <source src="http://103.73.107.122:3255/TSportsHD/tracks-v1a1/mono.m3u8" type="application/x-mpegURL">
      Your browser does not support the video tag.
    </video>
  </div>
</body>
</html>
