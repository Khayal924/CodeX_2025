<html lang="az">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>CodeX | Proqramlaşdırma və Kibertəhlükəsizlik</title>
  <style>
    body {
      font-family: Arial, sans-serif;
      background: #f8f9fb;
      padding: 20px;
      max-width: 900px;
      margin: auto;
    }
    h1 {
      text-align: center;
      color: #111;
      font-size: 2.2em;
      font-weight: 800;
      letter-spacing: 1px;
    }
    .course {
      background: #fff;
      padding: 20px;
      margin-top: 20px;
      border-radius: 16px;
      box-shadow: 0 0 12px rgba(0,0,0,0.1);
      transition: transform 0.2s ease;
    }
    .course:hover { transform: scale(1.02); }
    .btn {
      display: inline-block;
      padding: 12px 18px;
      background: #25D366;
      color: #fff;
      text-decoration: none;
      border-radius: 10px;
      margin-top: 10px;
      font-weight: bold;
      transition: background 0.3s;
    }
    .btn:hover { background: #1eb254; }
    .price { font-size: 18px; font-weight: bold; color: #333; }
    input[type="password"] { padding: 8px; width: 70%; margin-top: 10px; font-size: 16px; }
    button { padding: 8px 12px; background: #007bff; color: #fff; border: none; border-radius: 8px; margin-left: 5px; }
    .video-box { display: none; margin-top: 15px; }
    a.download-link {
      display: block; background: #007bff; color: #fff; text-align: center;
      padding: 10px; border-radius: 8px; text-decoration: none; margin-top: 10px; font-weight: bold;
    }
    a.download-link:hover { background: #0056b3; }
    iframe { width: 100%; height: 315px; border-radius: 10px; margin-top:10px; }
  </style>
</head>
<body>

  <h1>💻 CodeX Kursları</h1>
  <p style="text-align:center;">Kibertəhlükəsizlik və Proqramlaşdırma üzrə kurslar</p>

  <!-- İngilis dili kursu -->
  <div class="course">
    <h2>🇬🇧 İngilis Dili Kursu</h2>
    <p class="price">Qiymət: 5 AZN</p>
    <p><strong>Kart nömrəsi:</strong> 5411 **** **** 1013<br>
       <strong>Ad:</strong> Khayal Garibov<br>
       <strong>Bank:</strong> Leobank</p>

    <a class="btn" href="https://wa.me/994514852886?text=Salam,%20kurs%20haqqında%20məlumat%20istəyirəm%20(İngilis%20kursu%20-%205%20AZN)" target="_blank">
      📲 WhatsApp ilə məlumat alın
    </a>

    <div>
      <input type="password" placeholder="Şifrəni daxil edin" id="passEn">
      <button onclick="checkPassword('En')">Giriş</button>
      <p id="errorEn" style="color:red;display:none;">❌ Yanlış şifrə</p>
    </div>

    <div class="video-box" id="fileEn">
      <h3>📁 İngilis Kursu Faylları</h3>

      <!-- Bir Qeyd bölməsi -->
      <div style="background:#fffbcc; padding:10px; border-radius:8px; margin-bottom:10px;">
        <strong>Bir Qeyd:</strong>
        <p>
          Qeyd olunan file → part 1 → 1-ci fayl (geethams) yazılı file. (İzləməyin)<br>
          İstifadəçi şifrəni yazdıqdan sonra ilk fayldan başqa bütün faylları izləyə bilərsiniz. Digər faylları sırasıyla izləyə bilərsiniz. Hər şey Proqramlaşdırma, Kibertəhlükəsizlik və s. mövzuları üzrədir.
        </p>
      </div>

      <a href="https://mega.nz/folder/t69gha4L#IE4bFM_UtjvsANNF0FojLQ/folder/dm0VFL5A" target="_blank" class="download-link">📦 Kursu aç</a>
    </div>
  </div>

  <!-- Türk dili kursu -->
  <div class="course">
    <h2>🇹🇷 Türk Dili Kursu</h2>
    <p><em>Kibergüvenlik ve C++ Dərsləri</em></p>
    <p class="price">Qiymət: 2.99 AZN</p>
    <p><strong>Kart nömrəsi:</strong> 5411 **** **** 1013<br>
       <strong>Ad:</strong> Khayal Garibov<br>
       <strong>Bank:</strong> Leobank</p>

    <a class="btn" href="https://wa.me/994514852886?text=Salam,%20kurs%20haqqında%20məlumat%20istəyirəm%20(Türkçe%20kursu%20-%202.99%20AZN)" target="_blank">
      📲 WhatsApp ilə məlumat alın
    </a>

    <div>
      <input type="password" placeholder="Şifrəni daxil edin" id="passTr">
      <button onclick="checkPassword('Tr')">Giriş</button>
      <p id="errorTr" style="color:red;display:none;">❌ Yanlış şifrə</p>
    </div>

    <div class="video-box" id="fileTr">
      <h3>📁 Türk Kursu — YouTube Playlist</h3>
      <iframe src="https://www.youtube.com/embed/videoseries?list=PLY20HpFruiK17RArt5Guq8fF4GQgssQ0m" frameborder="0" allow="autoplay; encrypted-media" allowfullscreen></iframe>
    </div>
  </div>

  <script>
    const passwords = { En: "EN2025", Tr: "TR2025" };
    function checkPassword(lang) {
      const input = document.getElementById("pass" + lang).value.trim();
      const err = document.getElementById("error" + lang);
      const box = document.getElementById("file" + lang);
      if (input === passwords[lang]) {
        err.style.display = "none";
        box.style.display = "block";
        box.scrollIntoView({ behavior: "smooth" });
      } else {
        err.style.display = "block";
        box.style.display = "none";
      }
    }
  </script>
</body>
</html>
