<html lang="az">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Code X | Proqramlaşdırma və Kibertəhlükəsizlik</title>
  <style>
    :root{
      --bg:#f9f9f9;
      --card:#ffffff;
      --accent:#ff3b3b;
      --neon:#00e6e6;
      --text:#222;
      --muted:#666;
    }
    body{
      font-family: Arial, sans-serif;
      background: linear-gradient(120deg,var(--bg),#eef2f6);
      margin:0;
      padding:20px;
      max-width:980px;
      margin-left:auto;
      margin-right:auto;
      color:var(--text);
    }
    h1{
      text-align:center;
      font-size:36px;
      margin:6px 0 6px;
      background:linear-gradient(90deg,var(--accent),#0000ff);
      -webkit-background-clip:text;
      -webkit-text-fill-color:transparent;
      letter-spacing:1px;
    }
    p.lead{ text-align:center;color:var(--muted); margin-bottom:22px; }
    .course{
      position:relative;
      background:var(--card);
      border-radius:14px;
      padding:18px;
      margin:18px 0;
      box-shadow:0 6px 18px rgba(0,0,0,0.06);
      border-left:6px solid var(--accent);
      transition:transform .18s ease,box-shadow .18s ease;
      overflow:hidden;
    }
    .course:hover{ transform:translateY(-6px); box-shadow:0 18px 40px rgba(0,0,0,0.10); }
    .course h2{ margin:0 0 8px; color:var(--accent); }
    .meta{ color:var(--muted); margin:6px 0 12px; font-size:14px; line-height:1.4; }
    .price{ font-weight:700; color:var(--neon); margin-bottom:10px; display:block; }
    .row{ display:flex; gap:10px; flex-wrap:wrap; align-items:center; margin-top:8px; }
    .btn{
      display:inline-block;
      text-decoration:none;
      background:#25D366;
      color:#fff;
      padding:10px 14px;
      border-radius:9px;
      font-weight:700;
      box-shadow:0 6px 18px rgba(37,211,102,0.12);
    }
    .btn.info{ background: #ff9900; color:#fff; }
    input[type="password"]{
      padding:10px;
      border-radius:8px;
      border:1px solid #d0d7de;
      width:64%;
      font-size:15px;
    }
    button.action{
      padding:9px 12px;
      border-radius:8px;
      border:none;
      background:#1366d6;
      color:#fff;
      cursor:pointer;
      font-weight:700;
    }
    .video-box{ display:none; margin-top:14px; border-radius:10px; overflow:hidden; border:2px solid rgba(0,230,230,0.12); padding:12px; background:#fafafa; }
    .video-grid{ display:grid; grid-template-columns:1fr; gap:10px; }
    .video-card{ background:#000; border-radius:8px; overflow:hidden; box-shadow:0 8px 20px rgba(0,0,0,0.25); }
    .video-card iframe{ width:100%; height:260px; display:block; border:0; }
    .muted{ color:var(--muted); font-size:13px; margin-top:8px; }
    @media(min-width:760px){
      .video-grid{ grid-template-columns:1fr 1fr; }
      input[type="password"]{ width:64%; }
    }
  </style>
</head>
<body>

  <h1>Code X</h1>
  <p class="lead">İngilis və Azərbaycan dilində kibertəhlükəsizlik və proqramlaşdırma kursları — ödəniş WhatsApp ilə.</p>

  <!-- ENGLISH COURSE -->
  <div class="course" id="courseEn">
    <h2>🇬🇧 English — Kibertəhlükəsizlik və Proqramlaşdırma Kursu (Licensed)</h2>
    <span class="price">Price: <strong>10 AZN</strong></span>
    <p class="meta"><strong>Pay (card):</strong> 5411 **** **** 1013 — Khayal Garibov (Leobank)</p>
    <div class="row">
      <a class="btn" href="https://wa.me/994514852886?text=Salam,%20kurs%20haqq%C4%B1nda%20m%C9%99lumat%20ist%C9%99yir%C9%99m%20(English%20Course%20-%2010%20AZN)" target="_blank">📲 WhatsApp ilə məlumat alın</a>
      <a class="btn info" href="https://wa.me/994514852886?text=Salam,%20m%C9%99n%20Code%20X%20haqq%C4%B1nda%20%C9%99lav%C9%99%20m%C9%99lumat%20ist%C9%99yir%C9%99m." target="_blank">ℹ️ Kontakt</a>
    </div>
    <div style="margin-top:12px;">
      <input type="password" id="passEn" placeholder="Şifrəni daxil edin"/>
      <button class="action" onclick="checkPassword('En')">Giriş</button>
      <p id="errorEn" class="muted" style="color:#d23;display:none;margin-top:8px;">❌ Yanlış şifrə</p>
    </div>
    <div id="videoEn" class="video-box">
      <h3>📚 English Course — Content</h3>
      <div class="video-grid">
        <div class="video-card"><iframe src="https://www.youtube.com/embed/VIDEO_ID_EN_1" allowfullscreen></iframe></div>
        <div class="video-card"><iframe src="https://www.youtube.com/embed/VIDEO_ID_EN_2" allowfullscreen></iframe></div>
      </div>
    </div>
  </div>

  <!-- AZERBAIJANI COURSE -->
  <div class="course" id="courseAz">
    <h2>🇦🇿 Azərbaycan Dili — Kibertəhlükəsizlik və Proqramlaşdırma Kursu</h2>
    <span class="price">Qiymət: <strong>20 AZN</strong></span>
    <p class="meta"><strong>Pay (card):</strong> 5411 **** **** 1013 — Khayal Garibov (Leobank)</p>
    <div class="row">
      <a class="btn" href="https://wa.me/994514852886?text=Salam,%20kurs%20haqq%C4%B1nda%20m%C9%99lumat%20ist%C9%99yir%C9%99m%20(Azərbaycan%20kursu%20-%2020%20AZN)" target="_blank">📲 WhatsApp ilə məlumat alın</a>
      <a class="btn info" href="https://wa.me/994514852886?text=Salam,%20m%C9%99n%20Code%20X%20haqq%C4%B1nda%20%C9%99lav%C9%99%20m%C9%99lumat%20ist%C9%99yir%C9%99m." target="_blank">ℹ️ Kontakt</a>
    </div>
    <div style="margin-top:12px;">
      <input type="password" id="passAz" placeholder="Şifrəni daxil edin"/>
      <button class="action" onclick="checkPassword('Az')">Giriş</button>
      <p id="errorAz" class="muted" style="color:#d23;display:none;margin-top:8px;">❌ Yanlış şifrə</p>
    </div>
    <div id="videoAz" class="video-box">
      <h3>📚 Azərbaycan Kursu — Videolar</h3>
      <div class="video-grid">
        <div class="video-card"><iframe src="https://www.youtube.com/embed/dzkCrgtfiiY" allowfullscreen></iframe></div>
      </div>
    </div>
  </div>

  <script>
    const passwords = { En: "EN2025", Az: "AZ2025" };
    function checkPassword(lang){
      const input = document.getElementById("pass"+lang).value.trim();
      const err = document.getElementById("error"+lang);
      const box = document.getElementById("video"+lang);
      if(input === passwords[lang]){
        err.style.display = "none";
        box.style.display = "block";
        box.scrollIntoView({behavior:"smooth"});
      } else {
        err.style.display = "block";
        box.style.display = "none";
      }
    }
  </script>
</body>
</html>
