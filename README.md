<!DOCTYPE html>
<html lang="bn">
<head>
<meta charset="UTF-8" />
<meta name="viewport" content="width=device-width, initial-scale=1" />
<title>Jakaria Web Tv</title>
<style>
  body {
    margin: 0; 
    font-family: Arial, sans-serif;
    background: #000;
    color: white;
  }
  header {
    background-color: pink;
    display: flex;
    align-items: center;
    justify-content: space-between;
    padding: 12px 20px;
  }
  header h1 {
    margin: 0;
    font-size: 24px;
    font-weight: bold;
    color: #000;
  }.social-icons a {
    margin-left: 15px;
    text-decoration: none;
    display: inline-block;
  }.social-icons img {
    width: 28px;
    height: 28px;
    vertical-align: middle;
  }
  main {
    max-width: 800px;
    margin: 20px auto;
    padding: 0 10px;
    text-align: center;
  }
  video {
    width: 100%;
    border: 3px solid #e31b23;
    border-radius: 8px;
    background: black;
  }.server-buttons {
    margin-top: 15px;
    display: flex;
    justify-content: space-around;
    flex-wrap: wrap;
  }.server-buttons button {
    background-color: #e31b23;
    border: none;
    padding: 10px 16px;
    font-size: 16px;
    color: white;
    cursor: pointer;
    border-radius: 6px;
    transition: background-color 0.2s ease;
    min-width: 100px;
    margin: 5px;
  }.server-buttons button:hover {
    background-color: #a01517;
  }.owner-text {
    margin-top: 15px;
    font-size: 20px;
    font-weight: 600;
    color: #e31b23;
  }
  footer {
    margin-top: 40px;
    padding: 10px 0;
    background: linear-gradient(45deg, red, black);
    text-align: center;
    font-weight: bold;
    font-size: 18px;
    color: white;
  }
</style>
</head>
<body>

<header>
  <h1>Jakaria Web Tv</h1>
  <div class="social-icons">
    <a href="https://www.facebook.com/sheikh.muhammad.639043" target="_blank" title="Facebook">
      <img src="https://upload.wikimedia.org/wikipedia/commons/0/05/Facebook_Logo_(2019).png" alt="Facebook Logo" />
    </a>
    <a href="https://www.facebook.com/sheikh.muhammad.639043" target="_blank" title="Telegram (Linked same as FB)">
      <img src="https://upload.wikimedia.org/wikipedia/commons/8/82/Telegram_logo.svg" alt="Telegram Logo" />
    </a>
  </div>
</header>

<main>
  <video id="player" controls autoplay playsinline>
    <source src="https://cloudfrontnet.vercel.app/tplay/playout/209617/master.m3u8" type="application/x-mpegURL" />
    Your browser does not support the video tag.
  </video>

  <div class="server-buttons">
    <button data-src="https://cloudfrontnet.vercel.app/tplay/playout/209617/master.m3u8">Waz Bd</button>
    <button data-src="https://edge3-moblive.yuppcdn.net/drm/smil:tencricketdrm.smil/index.m3u8">Server 2</button>
    <button data-src="https://alibabacdn2.tamashaweb.com/alibaba02/alibaba02stream_720p.m3u8">Server 3</button>
    <button data-src="https://af.ayassport.ir/hls2/ssc1.m3u8">Server 4</button>
  </div>

  <div class="owner-text">
    Sheikh Muhammad
  </div>
</main>

<footer>
  Owner Jakaria
</footer>

<script>
const player = document.getElementById('player');
const buttons = document.querySelectorAll('.server-buttons button');

function setSource(src) {
  while (player.firstChild) player.removeChild(player.firstChild);
  const source = document.createElement('source');
  source.src = src;
  source.type = 'application/x-mpegURL';
  player.appendChild(source);
  player.load();
  player.play().catch(e => console.log(e));
}

buttons.forEach(button => {
  button.addEventListener('click', () => {
    setSource(button.getAttribute('data-src'));
  });
});

// পেজ লোড হওয়ার সাথে সাথে প্রথম সার্ভার চালাবে
setSource(buttons.getAttribute('data-src'));
</script>

</body>
</html>

