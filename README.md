<html lang="az">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>XCodeLearn | Proqramlaşdırma & Kibertəhlükəsizlik</title>
<style>
  /* Ümumi bədən */
  body {
    font-family: 'Courier New', monospace;
    background: #0d0d0d;
    color: #e0e0e0;
    padding: 20px;
    max-width: 1000px;
    margin: auto;
    position: relative;
    overflow-x: hidden;
  }

  h1 { 
    text-align: center; 
    color: #00ffea; 
    text-shadow: 0 0 10px #00ffea;
  }

  /* X watermark */
  .x-logo {
    position: fixed;
    font-size: 80px;
    color: rgba(255,0,0,0.1);
    z-index: 0;
    pointer-events: none;
    font-weight: bold;
    user-select: none;
  }
  .x1 { top: 10px; left: 10px; }
  .x2 { top: 10px; right: 10px; }
  .x3 { bottom: 10px; left: 10px; }
  .x4 { bottom: 10px; right: 10px; }

  .course {
    background: #111;
    border: 2px solid #00ffea;
    border-radius: 12px;
    padding: 15px;
    margin-top: 20px;
    box-shadow: 0 0 15px #00ffea60;
    position: relative;
    z-index: 1;
    transition: transform 0.2s, box-shadow 0.2s;
  }
  .course:hover {
    transform: scale(1.02);
    box-shadow: 0 0 25px #00ffea90;
  }

  h2 { color: #00ffea; text-shadow: 0 0 5px #00ffea; }

  .price { font-size: 18px; font-weight: bold; color: #ffea00; }

  .btn {
    display: inline-block;
    padding: 10px 15px;
    background: #25D366;
    color: #fff;
    text-decoration: none;
    border-radius: 8px;
    margin-top: 10px;
    font-weight: bold;
    box-shadow: 0 0 10px #25D36660;
    transition: background 0.2s, box-shadow 0.2s;
  }
  .btn:hover { background: #1eb254; box-shadow: 0 0 15px #25D36690; }

  input[type="password"] {
    padding: 8px;
    width: 70%;
    margin-top: 10px;
    font-size: 16px;
    border-radius: 8px;
    border: 1px solid #444;
    background: #222;
    color: #e0e0e0;
  }

  button {
    padding: 8px 12px;
    background: #007bff;
    color: #fff;
    border: none;
    border-radius: 8px;
    margin-left: 5px;
    cursor: pointer;
    transition: background 0.2s;
  }
  button:hover { background: #0056b3; }

  .video-box {
    display: none;
    margin-top: 15px;
    border: 2px solid #00ffea;
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

<!-- Watermarks -->
<div class="x-logo x1">X</div>
<div class="x-logo x2">X</div>
<div class="x-logo x3">X</div>
<div class="x-logo x4">X</div>

<h1>💻 XCodeLearn Kursları</h1>
<p style="text-align:center;">Proqramlaşdırma və Kibertəhlükəsizlik üzrə 3 dildə kurslar</p>

<!-- Azərbaycan -->
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

<!-- İngilis -->
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

<!-- Türk -->
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
