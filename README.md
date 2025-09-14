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
    <button data-src="https://tataplay.slivcdn.com/hls/live/2020591/TEN3HD/master_900.m3u8">Server 3</button>
    <button data-src="https://af.ayassport.ir/hls2/ssc1.m3u8">Server 4</button>





<!DOCTYPE html>
<html lang="bn">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1">
  <title>Jakaria Web Tv</title>

  <!-- Video.js CSS -->
  <link href="https://vjs.zencdn.net/7.20.3/video-js.css" rel="stylesheet" />

  <!-- FontAwesome for icons -->
  <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css" />

  <style>
    body {
      margin: 0;
      font-family: Arial, sans-serif;
      background-color: #000;
      color: white;
      text-align: center;
    }

    header {
      background-color: pink;
      padding: 10px 20px;
      display: flex;
      justify-content: space-between;
      align-items: center;
      flex-wrap: wrap;
    }

    header h1 {
      margin: 0;
      font-size: 24px;
      color: black;
    }

    .social-icons a {
      margin-left: 10px;
      color: black;
      font-size: 20px;
      text-decoration: none;
    }

    .player-container {
      margin: 20px auto;
      max-width: 720px;
    }

    .server-buttons {
      margin: 20px 0;
    }

    .server-buttons button {
      margin: 5px;
      padding: 10px 15px;
      font-size: 16px;
      cursor: pointer;
      border: none;
      border-radius: 5px;
      background-color: #444;
      color: white;
      transition: 0.3s;
    }

    .server-buttons button:hover {
      background-color: #888;
    }

    footer {
      background: linear-gradient(to right, red, black);
      padding: 15px;
      color: white;
      font-weight: bold;
    }
  </style>
</head>
<body>

  <header>
    <h1>Jakaria Web Tv</h1>
    <div class="social-icons">
      <a href="https://www.facebook.com/sheikh.muhammad.639043" target="_blank" title="Facebook">
        <i class="fab fa-facebook"></i>
      </a>
      <a href="https://www.facebook.com/sheikh.muhammad.639043" target="_blank" title="Telegram">
        <i class="fab fa-telegram"></i>
      </a>
    </div>
  </header>

  <div class="player-container">
    <video id="videoPlayer" class="video-js vjs-default-skin" controls preload="auto" width="720" height="400">
      <source src="" type="application/x-mpegURL">
    </video>
  </div>

  <div class="server-buttons">
    <button onclick="changeStream('https://cloudfrontnet.vercel.app/tplay/playout/209617/master.m3u8')">Server 1</button>
    <button onclick="changeStream('https://edge3-moblive.yuppcdn.net/drm/smil:tencricketdrm.smil/index.m3u8')">Server 2</button>
    <button onclick="changeStream('https://alibabacdn2.tamashaweb.com/alibaba02/alibaba02stream_720p.m3u8')">Server 3</button>
    <button onclick="changeStream('https://af.ayassport.ir/hls2/ssc1.m3u8')">Server 4</button>
    <button onclick="changeStream('https://alibabacdn2.tamashaweb.com/alibaba02/alibaba02stream_1080p.m3u8')">Server 5</button>
    <button onclick="changeStream('http://tv.bdiptv.store:80/live/restreauuX58y/refstream/218.m3u8')">Server 6</button>
    <button onclick="changeStream('https://storage.googleapis.com/overtrongher1/mux_video_ts/index-1.m3u8')">Server 7</button>
  </div>

  <footer>
    owner Jakaria
  </footer>

  <!-- Video.js JS -->
  <script src="https://vjs.zencdn.net/7.20.3/video.min.js"></script>

  <script>
    var player = videojs('videoPlayer');

    function changeStream(url) {
      player.src({ src: url, type: 'application/x-mpegURL' });
      player.play();
    }
  </script>

</body>
</html>




