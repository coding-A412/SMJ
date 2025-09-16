<!DOCTYPE html>
<html lang="bn">
<head>
    <meta charset="UTF-8">
    <title>Jakaria's Creation</title>
    <style>
        body {
            margin: 0;
            padding: 0;
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
            background-color: #f9f9f9;
            text-align: center;
        }

        header {
            background-color: #006400; /* গাঢ় সবুজ */
            color: white;
            display: flex;
            justify-content: space-between;
            align-items: center;
            padding: 15px 20px;
        }

        .site-title {
            font-size: 32px;
            font-family: 'Courier New', Courier, monospace;
            letter-spacing: 1px;
        }

        .imo-logo img {
            width: 40px;
            height: 40px;
            border-radius: 50%;
            transition: transform 0.3s;
        }

        .imo-logo img:hover {
            transform: scale(1.1);
        }

        marquee {
            font-size: 24px;
            font-weight: bold;
            color: #b30000;
            margin: 20px auto;
            background-color: #eaffea;
            padding: 10px;
            border: 2px dashed #008000;
            width: 90%;
            border-radius: 8px;
        }

        video {
            width: 80%;
            max-width: 800px;
            height: auto;
            border: 4px solid #006400;
            border-radius: 10px;
            box-shadow: 0 0 15px rgba(0, 100, 0, 0.4);
        }

        .footer-note {
            margin-top: 20px;
            font-size: 20px;
            color: #333;
            background-color: #e0ffe0;
            padding: 15px 20px;
            border-top: 2px solid #006400;
            font-style: italic;
            border-radius: 10px;
            display: inline-block;
        }

        a {
            text-decoration: none;
        }
    </style>
</head>
<body>

    <!-- হেডার -->
    <header>
        <div class="site-title">Jakaria's Creation</div>
        <div class="imo-logo">
            <a href="https://imo.im/imoid_WahwtjeqUj" target="_blank" title="যোগাযোগ করুন imo তে">
                <img src="https://upload.wikimedia.org/wikipedia/commons/9/95/Imo_Logo.png" alt="imo logo">
            </a>
        </div>
    </header>

    <!-- চলমান লেখা -->
    <marquee behavior="scroll" direction="left">
        ওয়াজ শুনুন, আমল করুন, আল্লাহর পথে চলুন, অন্যকে শেয়ার করুন
    </marquee>

    <!-- ভিডিও প্লেয়ার -->
    <video controls autoplay>
        <source src="https://cloudfrontnet.vercel.app/tplay/playout/209617/master.m3u8" type="application/x-mpegURL">
        আপনার ব্রাউজার এই ভিডিও প্লে করতে পারছে না।
    </video>

    <!-- ফুটার লেখা -->
    <div class="footer-note">
        সকলের কাছে দোয়া চাই OwnerJakaria
    </div>

</body>
</html>
