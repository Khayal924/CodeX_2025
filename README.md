<html lang="az">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>XCodeLearn | Proqramlaşdırma və Kibertəhlükəsizlik</title>
  <style>
    body {
      font-family: Arial, sans-serif;
      background: #f2f2f2;
      padding: 20px;
      max-width: 900px;
      margin: auto;
    }
    h1 { text-align: center; color: #222; }
    .course {
      background: #fff;
      padding: 15px;
      margin-top: 20px;
      border-radius: 12px;
      box-shadow: 0 0 8px rgba(0,0,0,0.1);
    }
    .btn {
      display: inline-block;
      padding: 10px 15px;
      background: #25D366;
      color: #fff;
      text-decoration: none;
      border-radius: 8px;
      margin-top: 10px;
      font-weight: bold;
    }
    .btn:hover { background: #1eb254; }
    .price { font-size: 18px; font-weight: bold; color: #444; }
    input[type="password"] {
      padding: 8px;
      width: 70%;
      margin-top: 10px;
      font-size: 16px;
    }
    button {
      padding: 8px 12px;
      background: #007bff;
      color: #fff;
      border: none;
      border-radius: 8px;
      margin-left: 5px;
    }
    .video-box {
      display: none;
      margin-top: 15px;
    }
    iframe {
      width: 100%;
      height: 315px;
      border-radius: 10px;
    }
  </style>
</head>
<body>

  <h1>💻 XCodeLearn Kursları</h1>
  <p style="text-align:center;">Proqramlaşdırma və Kibertəhlükəsizlik üzrə 3 dildə kurslar</p>

  <!-- Azərbaycan dili kursu -->
  <div class="course">
    <h2>🇦🇿 Azərbaycan Dili Kursu</h2>
    <p class="price">Qiymət: 20 AZN</p>
    <p><strong>Kart nömrəsi:</strong> 5411 **** **** 1013<br>
       <strong>Ad:</strong> Khayal Garibov<br>
       <strong>Bank:</strong> Leobank</p>

    <a class="btn" href="https://wa.me/994514852886?text=Salam,%20Azərbaycan%20kursu%20üçün%2020%20AZN%20ödədim.%20Adım:%20[Adınızı%20yazın]" target="_blank">
      📲 WhatsApp ilə ödənişi bildir
    </a>

    <div>
      <input type="password" placeholder="Şifrəni daxil edin" id="passAz">
      <button onclick="checkPassword('Az')">Giriş</button>
      <p id="errorAz" style="color:red;display:none;">❌ Yanlış şifrə</p>
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

    <a class="btn" href="https://wa.me/994514852886?text=Salam,%20İngilis%20kursu%20üçün%2010%20AZN%20ödədim.%20Adım:%20[Adınızı%20yazın]" target="_blank">
      📲 WhatsApp ilə ödənişi bildir
    </a>

    <div>
      <input type="password" placeholder="Şifrəni daxil edin" id="passEn">
      <button onclick="checkPassword('En')">Giriş</button>
      <p id="errorEn" style="color:red;display:none;">❌ Yanlış şifrə</p>
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

    <a class="btn" href="https://wa.me/994514852886?text=Salam,%20Türkcə%20kurs%20üçün%2015%20AZN%20ödədim.%20Adım:%20[Adınızı%20yazın]" target="_blank">
      📲 WhatsApp ilə ödənişi bildir
    </a>

    <div>
      <input type="password" placeholder="Şifrəni daxil edin" id="passTr">
      <button onclick="checkPassword('Tr')">Giriş</button>
      <p id="errorTr" style="color:red;display:none;">❌ Yanlış şifrə</p>
    </div>

    <div class="video-box" id="fileTr">
      <h3>📹 Türk Kursu</h3>
      <iframe src="https://www.youtube.com/embed/VIDEO_ID_TR" allowfullscreen></iframe>
    </div>
  </div>

  <script>
    const passwords = {
      Az: "AZ2025",
      En: "EN2025",
      Tr: "TR2025"
    };

    function checkPassword(lang) {
      const input = document.getElementById("pass" + lang).value.trim();
      if (input === passwords[lang]) {
        document.getElementById("file" + lang).style.display = "block";
        document.getElementById("error" + lang).style.display = "none";
      } else {
        document.getElementById("error" + lang).style.display = "block";
      }
    }
  </script>
</body>
</html>
