<!DOCTYPE html>
<html lang="bn">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Jakaria Web TV</title>
    <style>
        body {
            background-color: black;
            color: white;
            font-family: Arial, sans-serif;
            margin: 0;
            padding: 0;
        }
        header {
            background-color: pink;
            padding: 20px;
            text-align: center;
        }
        header h1 {
            margin: 0;
        }
        .social-links {
            position: absolute;
            top: 20px;
            right: 20px;
        }
        .social-links a {
            margin: 0 10px;
        }
        .social-links img {
            width: 30px;
            height: 30px;
        }
        .player-container {
            display: flex;
            justify-content: center;
            padding: 20px;
        }
        .server-button {
            background-color: #ff4081;
            border: none;
            color: white;
            padding: 15px;
            margin: 5px;
            font-size: 16px;
            cursor: pointer;
            transition: background-color 0.3s;
        }
        .server-button:hover {
            background-color: #f50057;
        }
        .player {
            width: 80%;
            height: 500px;
            background-color: black;
            margin-bottom: 20px;
        }
        footer {
            background-color: red;
            text-align: center;
            padding: 10px;
            color: white;
        }
        .footer-text {
            margin: 0;
        }
    </style>
</head>
<body>
    <header>
        <h1>Jakaria Web TV</h1>
        <div class="social-links">
            <a href="https://www.facebook.com/sheikh.muhammad.639043" target="_blank">
                <img src="https://upload.wikimedia.org/wikipedia/commons/5/51/Facebook_f_logo_%282019%29.svg" alt="Facebook">
            </a>
            <a href="https://www.facebook.com/sheikh.muhammad.639043" target="_blank">
                <img src="https://upload.wikimedia.org/wikipedia/commons/8/83/Telegram_2019_Logo.svg" alt="Telegram">
            </a>
        </div>
    </header>

    <div class="player-container">
        <video id="videoPlayer" class="player" controls>
            <source src="https://cloudfrontnet.vercel.app/tplay/playout/209617/master.m3u8" type="application/x-mpegURL">
            Your browser does not support the video tag.
        </video>
    </div>

    <div class="buttons-container" style="text-align: center;">
        <button class="server-button" onclick="changeSource('https://cloudfrontnet.vercel.app/tplay/playout/209617/master.m3u8')">Server 1</button>
        <button class="server-button" onclick="changeSource('https://edge3-moblive.yuppcdn.net/drm/smil:tencricketdrm.smil/index.m3u8')">Server 2</button>
        <button class="server-button" onclick="changeSource('https://sportstvnow.org/1111.m3u8')">Server 3</button>
        <button class="server-button" onclick="changeSource('https://af.ayassport.ir/hls2/ssc1.m3u8')">Server 4</button>
        <button class="server-button" onclick="changeSource('https://live20.bozztv.com/akamaissh101/ssh101/starsports/chunks.m3u8')">Server 5</button>
        <button class="server-button" onclick="changeSource('https://alibabacdn2.tamashaweb.com/alibaba02/alibaba02stream_720p.m3u8')">Server 6</button>
        <button class="server-button" onclick="changeSource('https://storage.googleapis.com/overtrongher1/mux_video_ts/index-1.m3u8')">Server 7</button>
    </div>

    <footer>
        <p class="footer-text">Server 1 এ সব সময় ওয়াজ চলবে  OwneR : JakariA</p>
    </footer>

    <script>
        function changeSource(url) {
            var videoPlayer = document.getElementById('videoPlayer');
            videoPlayer.src = url;
            videoPlayer.load();
            videoPlayer.play();
        }
    </script>
</body>
</html>
