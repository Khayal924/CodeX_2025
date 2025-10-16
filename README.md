<!DOCTYPE html>
<html lang="az">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Proqramlaşdırma Öyrən | XCodeLearn</title>
  <style>
    body {
      font-family: Arial, sans-serif;
      background: #f2f2f2;
      padding: 20px;
      max-width: 800px;
      margin: auto;
    }
    h1 {
      text-align: center;
      color: #2b2b2b;
    }
    .pay-box, .video-box, .password-box {
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
    iframe {
      width: 100%;
      height: 250px;
      margin-top: 15px;
      border-radius: 10px;
    }
  </style>
</head>
<body>

  <h1>💻 Proqramlaşdırma Kursları</h1>
  <p style="text-align:center;">Onlayn öyrən, gələcəyini qur!</p>

  <!-- Ödəniş bölməsi -->
  <div class="pay-box">
    <h2>💳 Ödəniş məlumatları</h2>
    <p><strong>Kart nömrəsi:</strong> 5411 **** **** 1013</p>
    <p><strong>Ad:</strong> Khayal Garibov</p>
    <p><strong>Bank:</strong> Leobank</p>
    <p><strong>Məbləğ:</strong> 10 AZN (birdəfəlik kurs haqqı)</p>

    <!-- WhatsApp ilə bildiriş -->
    <a class="btn" href="https://wa.me/994514852886?text=Salam,%20mən%20kurs%20üçün%2010%20AZN%20ödədim.%20Adım:%20[Adınızı%20yazın]%20TXN:%20[Əməliyyat%20ID]" target="_blank">
      📲 WhatsApp ilə ödənişi bildir
    </a>

    <!-- Google Form linki -->
    <p style="margin-top:10px;">
      <a class="btn" style="background:#ff9900;" href="https://forms.gle/SENIN-FORM-LINKIN" target="_blank">
        📎 Ödənişi təsdiqlə (Form)
      </a>
    </p>

    <small>Ödəniş etdikdən sonra WhatsApp və ya Form vasitəsilə təsdiq göndərin. Təsdiqdən sonra sizə şifrə göndəriləcək.</small>
  </div>

  <!-- Şifrə ilə giriş bölməsi -->
  <div class="password-box">
    <h2>🔐 Videolara giriş</h2>
    <p>Ödəniş təsdiqləndikdən sonra sizə göndərilən şifrəni daxil edin:</p>
    <input type="password" id="passwordInput" placeholder="Şifrəni daxil edin">
    <button onclick="checkPassword()">Giriş</button>
    <p id="errorMsg" style="color:red; display:none;">❌ Yanlış şifrə. Yenidən cəhd edin.</p>
  </div>

  <!-- Video bölməsi -->
  <div class="video-box" id="videoBox" style="display:none;">
    <h2>📚 Proqramlaşdırma dərsləri</h2>
    <iframe src="https://www.youtube.com/embed/dzkCrgtfiiY" frameborder="0" allowfullscreen></iframe>
    <!-- Yeni videoları əlavə etmək üçün aşağıdakı kimi iframe-lər əlavə edə bilərsən -->
    <!--
    <iframe src="https://www.youtube.com/embed/VIDEO_ID_2" frameborder="0" allowfullscreen></iframe>
    <iframe src="https://www.youtube.com/embed/VIDEO_ID_3" frameborder="0" allowfullscreen></iframe>
    -->
  </div>

  <script>
    // ✅ İstifadəçilərə veriləcək şifrələr (istəsən artırıb azalda bilərsən)
    const validPasswords = ["XCODE2025", "KURS001", "KURS002"];

    function checkPassword() {
      const input = document.getElementById("passwordInput").value.trim();
      if (validPasswords.includes(input)) {
        document.getElementById("videoBox").style.display = "block";
        document.getElementById("errorMsg").style.display = "none";
      } else {
        document.getElementById("errorMsg").style.display = "block";
      }
    }
  </script>

</body>
</html>
