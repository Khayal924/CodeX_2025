<html lang="az">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>XCodeLearn | Proqramlaşdırma və Kibertəhlükəsizlik Kursları</title>
  <style>
    body {
      font-family: Arial, sans-serif;
      background: #f2f2f2;
      padding: 20px;
      max-width: 900px;
      margin: auto;
    }
    h1 {
      text-align: center;
      color: #2b2b2b;
    }
    .course-box, .password-box, .file-box {
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
    .btn:hover {
      background: #1eb254;
    }
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
    h2 { color: #333; }
  </style>
</head>
<body>

  <h1>💻 XCodeLearn Kursları</h1>
  <p style="text-align:center;">Proqramlaşdırma və Kibertəhlükəsizlik sahəsində 3 dildə kurslar</p>

  <!-- 🇬🇧 İngiliscə Kurs -->
  <div class="course-box">
    <h2>🇬🇧 İngiliscə Kurs — 20 AZN</h2>
    <p><strong>Kart nömrəsi:</strong> 5411 **** **** 1013</p>
    <p><strong>Ad:</strong> Khayal Garibov | <strong>Bank:</strong> Leobank</p>
    <p><strong>Qiymət:</strong> 20 AZN</p>

    <a class="btn" href="https://wa.me/994514852886?text=Salam,%20mən%20İngiliscə%20kurs%20üçün%2020%20AZN%20ödədim.%20Adım:%20[Ad]%20TXN:%20[Əməliyyat%20ID]" target="_blank">
      📲 WhatsApp ilə ödənişi bildir
    </a>

    <div class="password-box">
      <p>Şifrəni daxil et:</p>
      <input type="password" id="passwordInputEn" placeholder="İngiliscə kurs şifrəsi">
      <button onclick="checkPassword('en')">Giriş</button>
      <p id="errorEn" style="color:red; display:none;">❌ Yanlış şifrə</p>
    </div>

    <div class="file-box" id="fileBoxEn" style="display:none;">
      <h3>📥 Kurs Faylları (İngiliscə)</h3>
      <a href="https://mega.nz/file/SENIN-LINKIN-EN" target="_blank" style="display:inline-block;padding:10px 15px;background:#007bff;color:#fff;text-decoration:none;border-radius:8px;font-weight:bold;">
        Endir
      </a>
    </div>
  </div>

  <!-- 🇹🇷 Türkçe Kurs -->
  <div class="course-box">
    <h2>🇹🇷 Türkçe Kurs — 15 AZN</h2>
    <p><strong>Kart nömrəsi:</strong> 5411 **** **** 1013</p>
    <p><strong>Ad:</strong> Khayal Garibov | <strong>Bank:</strong> Leobank</p>
    <p><strong>Qiymət:</strong> 15 AZN</p>

    <a class="btn" href="https://wa.me/994514852886?text=Salam,%20mən%20Türkcə%20kurs%20üçün%2015%20AZN%20ödədim.%20Adım:%20[Ad]%20TXN:%20[Əməliyyat%20ID]" target="_blank">
      📲 WhatsApp ilə ödənişi bildir
    </a>

    <div class="password-box">
      <p>Şifrəni daxil et:</p>
      <input type="password" id="passwordInputTr" placeholder="Türkcə kurs şifrəsi">
      <button onclick="checkPassword('tr')">Giriş</button>
      <p id="errorTr" style="color:red; display:none;">❌ Yanlış şifrə</p>
    </div>

    <div class="file-box" id="fileBoxTr" style="display:none;">
      <h3>📥 Kurs Faylları (Türkcə)</h3>
      <a href="https://mega.nz/file/SENIN-LINKIN-TR" target="_blank" style="display:inline-block;padding:10px 15px;background:#007bff;color:#fff;text-decoration:none;border-radius:8px;font-weight:bold;">
        Endir
      </a>
    </div>
  </div>

  <!-- 🇦🇿 Azərbaycan Dili Kursu -->
  <div class="course-box">
    <h2>🇦🇿 Azərbaycan Dili Kursu — 10 AZN</h2>
    <p><strong>Kart nömrəsi:</strong> 5411 **** **** 1013</p>
    <p><strong>Ad:</strong> Khayal Garibov | <strong>Bank:</strong> Leobank</p>
    <p><strong>Qiymət:</strong> 10 AZN</p>

    <a class="btn" href="https://wa.me/994514852886?text=Salam,%20mən%20Azərbaycan%20dili%20kursu%20üçün%2010%20AZN%20ödədim.%20Adım:%20[Ad]%20TXN:%20[Əməliyyat%20ID]" target="_blank">
      📲 WhatsApp ilə ödənişi bildir
    </a>

    <div class="password-box">
      <p>Şifrəni daxil et:</p>
      <input type="password" id="passwordInputAz" placeholder="Azərbaycan dili kursu şifrəsi">
      <button onclick="checkPassword('az')">Giriş</button>
      <p id="errorAz" style="color:red; display:none;">❌ Yanlış şifrə</p>
    </div>

    <div class="file-box" id="fileBoxAz" style="display:none;">
      <h3>📥 Kurs Faylları (Azərbaycan dili)</h3>
      <a href="https://mega.nz/file/SENIN-LINKIN-AZ" target="_blank" style="display:inline-block;padding:10px 15px;background:#007bff;color:#fff;text-decoration:none;border-radius:8px;font-weight:bold;">
        Endir
      </a>
    </div>
  </div>

  <script>
    const passwords = {
      en: "EN2025",
      tr: "TR2025",
      az: "AZ2025"
    };

    function checkPassword(lang) {
      const input = document.getElementById("passwordInput" + lang.toUpperCase()).value.trim();
      if (input === passwords[lang]) {
        document.getElementById("fileBox" + lang.toUpperCase()).style.display = "block";
        document.getElementById("error" + lang.toUpperCase()).style.display = "none";
      } else {
        document.getElementById("error" + lang.toUpperCase()).style.display = "block";
      }
    }
  </script>

</body>
</html>
