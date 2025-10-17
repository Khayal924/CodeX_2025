<html lang="az">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Code X | Proqramlaşdırma və Kibertəhlükəsizlik</title>
  <style>
    body {
      font-family: Arial, sans-serif;
      background: #f9f9f9;
      padding: 20px;
      max-width: 900px;
      margin: auto;
    }

    h1 {
      text-align: center;
      font-size: 36px;
      font-weight: bold;
      background: linear-gradient(90deg, #ff0000, #0000ff);
      -webkit-background-clip: text;
      -webkit-text-fill-color: transparent;
      text-shadow: 0 0 8px rgba(0,0,0,0.3);
      margin-bottom: 10px;
    }

    p.subtitle {
      text-align: center;
      color: #333;
      font-size: 16px;
      margin-bottom: 30px;
    }

    .course {
      position: relative;
      background: #fff;
      padding: 20px;
      margin-top: 20px;
      border-radius: 15px;
      box-shadow: 0 4px 12px rgba(0,0,0,0.08);
      border-left: 5px solid #ff0000;
      transition: transform 0.2s, box-shadow 0.2s;
      overflow: hidden;
    }

    .course:hover {
      transform: translateY(-3px);
      box-shadow: 0 8px 20px rgba(0,0,0,0.15);
    }

    /* Futuristic blinking X logo */
    .course::after {
      content: "X";
      position: absolute;
      top: 10px;
      right: 10px;
      font-size: 40px;
      color: rgba(255,0,0,0.8);
      font-weight: bold;
      animation: blinkX 1.5s infinite;
      pointer-events: none;
    }

    @keyframes blinkX {
      0%, 100% { color: rgba(255,0,0,0.8); text-shadow: 0 0 5px #ff0000, 0 0 10px #ff0000, 0 0 15px #ff0000; }
      50% { color: rgba(255,255,255,0.8); text-shadow: 0 0 10px #ff00ff, 0 0 20px #ff00ff, 0 0 30px #ff00ff; }
    }

    h2 { color: #222; margin-bottom: 8px; }
    .price { font-size: 18px; font-weight: bold; color: #444; margin-bottom: 10px; }

    .btn {
      display: inline-block;
      padding: 10px 15px;
      background: #25D366;
      color: #fff;
      text-decoration: none;
      border-radius: 8px;
      margin-top: 10px;
      font-weight: bold;
      transition: background 0.2s, box-shadow 0.2s;
    }

    .btn:hover { 
      background: #1eb254;
      box-shadow: 0 0 8px #25D36680;
    }

    input[type="password"] {
      padding: 8px;
      width: 70%;
      margin-top: 10px;
      font-size: 16px;
      border-radius: 6px;
      border: 1px solid #ccc;
    }

    button {
      padding: 8px 12px;
      background: #007bff;
      color: #fff;
      border: none;
      border-radius: 6px;
      margin-left: 5px;
      cursor: pointer;
      transition: background 0.2s;
    }

    button:hover { background: #0056b3; }

    .video-box {
      display: none;
      margin-top: 15px;
      border-radius: 10px;
      overflow: hidden;
    }

    iframe {
      width: 100%;
      height: 315px;
      border: 0;
      display: block;
    }

    p, strong { font-size: 15px; }
    #errorAz, #errorEn, #errorTr { color: #ff4d4d; display: none; font-weight: bold; }
  </style>
</head>
<body>

<h1>Code X</h1>
<p class="subtitle">Proqramlaşdırma və Kibertəhlükəsizlik üzrə 3 dildə kurslar</p>

<!-- Azərbaycan dili kursu -->
<div class="course">
  <h2>🇦🇿 Azərbaycan Dili Kursu</h2>
  <p class="price">Qiymət: 20 AZN</p>
  <p><strong>Kart nömrəsi:</strong> 5411 **** **** 1013<br>
     <strong>Ad:</strong> Khayal Garibov<br>
     <strong>Bank:</strong> Leobank</p>

  <a class="btn" href="https://wa.me/994514852886?text=Salam,%20kurs%20haqqında%20məlumat%20istəyirəm%20(Azərbaycan%20kursu%20-%2020%20AZN)" target="_blank">
    📲 WhatsApp ilə məlumat alın
  </a>

  <div>
    <input type="password" placeholder="Şifrəni daxil edin" id="passAz">
    <button onclick="checkPassword('Az')">Giriş</button>
    <p id="errorAz">❌ Yanlış şifrə</p>
  </div>

  <div class="video-box" id="fileAz">
    <h3>📹 Azərbaycan Kursu</h3>
    <iframe src="https://www.youtube.com/embed/dzkCrgtfiiY" allowfullscreen></iframe>
  </div>
</div>

<!-- İngilis dili kursu -->
<div class="course">
  <h2>🇬🇧 İngilis Dili Kursu</h2>
  <p class="price">Qiymət: 10 AZN</p>
  <p><strong>Kart nömrəsi:</strong> 5411 **** **** 1013<br>
     <strong>Ad:</strong> Khayal Garibov<br>
     <strong>Bank:</strong> Leobank</p>

  <a class="btn" href="https://wa.me/994514852886?text=Salam,%20kurs%20haqqında%20məlumat%20istəyirəm%20(İngilis%20kursu%20-%2010%20AZN)" target="_blank">
    📲 WhatsApp ilə məlumat alın
  </a>

  <div>
    <input type="password" placeholder="Şifrəni daxil edin" id="passEn">
    <button onclick="checkPassword('En')">Giriş</button>
    <p id="errorEn">❌ Yanlış şifrə</p>
  </div>

  <div class="video-box" id="fileEn">
    <h3>📹 İngilis Kursu</h3>
    <iframe src="https://www.youtube.com/embed/VIDEO_ID_EN" allowfullscreen></iframe>
  </div>
</div>

<!-- Türk dili kursu -->
<div class="course">
  <h2>🇹🇷 Türk Dili Kursu</h2>
  <p class="price">Qiymət: 15 AZN</p>
  <p><strong>Kart nömrəsi:</strong> 5411 **** **** 1013<br>
     <strong>Ad:</strong> Khayal Garibov<br>
     <strong>Bank:</strong> Leobank</p>

  <a class="btn" href="https://wa.me/994514852886?text=Salam,%20kurs%20haqqında%20məlumat%20istəyirəm%20(Türkçe%20kursu%20-%2015%20AZN)" target="_blank">
    📲 WhatsApp ilə məlumat alın
  </a>

  <div>
    <input type="password" placeholder="Şifrəni daxil edin" id="passTr">
    <button onclick="checkPassword('Tr')">Giriş</button>
    <p id="errorTr">❌ Yanlış şifrə</p>
  </div>

  <div class="video-box" id="fileTr">
    <h3>📹 Türk Kursu</h3>
    <iframe src="https://www.youtube.com/embed/VIDEO_ID_TR" allowfullscreen></iframe>
  </div>
</div>

<script>
  const passwords = { Az:"AZ2025", En:"EN2025", Tr:"TR2025" };
  function checkPassword(lang){
    const input = document.getElementById("pass"+lang).value.trim();
    if(input===passwords[lang]){
      document.getElementById("file"+lang).style.display="block";
      document.getElementById("error"+lang).style.display="none";
    } else {
      document.getElementById("error"+lang).style.display="block";
      document.getElementById("file"+lang).style.display="none";
    }
  }
</script>
</body>
</html>
