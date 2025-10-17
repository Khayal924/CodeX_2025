<!doctype html>
<html lang="az">
<head>
  <meta charset="utf-8"/>
  <meta name="viewport" content="width=device-width,initial-scale=1"/>
  <title>XCodeLearn — Kurslar</title>
  <style>
    body{font-family:Arial,Helvetica,sans-serif;background:#f3f4f6;padding:18px;max-width:900px;margin:auto}
    h1{text-align:center;color:#222}
    .course{background:#fff;padding:14px;border-radius:10px;margin-top:16px;box-shadow:0 6px 18px rgba(0,0,0,0.06)}
    .meta{color:#444;margin:6px 0}
    .price{font-weight:700;color:#1f2937}
    .btn{display:inline-block;padding:10px 14px;border-radius:8px;text-decoration:none;color:#fff;background:#25D366;font-weight:700}
    .btn.orange{background:#ff9900}
    .row{display:flex;gap:8px;flex-wrap:wrap;margin-top:10px}
    input[type="password"], input[type="text"]{padding:8px;border-radius:8px;border:1px solid #ddd;font-size:15px;width:60%}
    button{padding:8px 10px;border-radius:8px;border:none;background:#0ea5e9;color:#fff;font-weight:700;cursor:pointer}
    .small{font-size:13px;color:#666}
    .video-box{display:none;margin-top:12px}
    iframe{width:100%;height:315px;border-radius:10px;border:0;margin-top:8px}
    .gen-row{display:flex;gap:8px;align-items:center;margin-top:10px;flex-wrap:wrap}
    .copy-btn{background:#111;color:#fff;padding:8px 10px;border-radius:8px;border:none;cursor:pointer}
    .notice{background:#fff8e1;padding:10px;border-radius:8px;margin-top:10px;color:#664d03}
  </style>
</head>
<body>

  <h1>💻 XCodeLearn — Proqramlaşdırma & Kibertəhlükəsizlik</h1>
  <p class="small" style="text-align:center">3 dil: Azərbaycan, İngilis, Türkçe — ödəniş WhatsApp vasitəsilə. Ödənişi sən yoxlayıb unik şifrə verirsən.</p>

  <!-- Azərbaycan -->
  <div class="course" id="courseAz">
    <h2>🇦🇿 Azərbaycan Dili Kursu</h2>
    <p class="price">Qiymət: <strong>20 AZN</strong></p>
    <p class="meta"><strong>Kart:</strong> 5411 **** **** 1013 • <strong>Ad:</strong> Khayal Garibov • <strong>Bank:</strong> Leobank</p>

    <!-- WhatsApp: dəyişdirilmiş mesaj (istifadəçinin göndərəcəyi) -->
    <div class="row">
      <a class="btn" href="https://wa.me/994514852886?text=Salam,%20Azərbaycan%20kursu%20üçün%2020%20AZN%20ödenis%20etmək%20istəyirəm.%20Adım:%20[Adınızı%20yazın]" target="_blank" rel="noopener">
        📲 WhatsApp ilə ödəniş etmək istəyirəm
      </a>

      <a class="btn orange" href="https://wa.me/994514852886?text=Salam,%20Azərbaycan%20kursu%20haqqında%20əlavə%20məlumat%20istəyirəm.%20Ad:%20[Adınız]" target="_blank" rel="noopener">
        ℹ️ Əlavə məlumat
      </a>
    </div>

    <div class="notice">
      İstifadəçi bu düyməyə basıb sənə mesaj göndərir. Ödənişi bank tətbiqində yoxladıqdan sonra ona unik şifrə yaradıb WhatsApp-la göndərin.
    </div>

    <!-- Owner üçün: şifrə yaratma -->
    <div class="gen-row">
      <input type="text" id="ownerGenAz" placeholder="Yeni şifrə (owner üçün)" readonly>
      <button onclick="generatePassword('Az')">Şifrə yarat</button>
      <button class="copy-btn" onclick="copyOwnerPassword('Az')">Kopyala</button>
      <span class="small">— Yaradılan kodu WhatsApp ilə alıcıya göndərin.</span>
    </div>

    <!-- İstifadəçi üçün: şifrə daxil edib faylları görmə -->
    <div style="margin-top:12px">
      <input type="password" id="passAz" placeholder="Şifrənizi daxil edin">
      <button onclick="checkPass('Az')">Giriş</button>
      <p id="errAz" class="small" style="color:#c00;display:none">Yanlış şifrə</p>
    </div>

    <!-- Gizli məzmun (YouTube və ya fayl linkləri) -->
    <div class="video-box" id="contentAz">
      <h3>📚 Azərbaycan Kursu — Məzmun</h3>
      <!-- Əgər YouTube videoları olacaqsa buraya iframe əlavə et -->
      <!-- Misal: <iframe src="https://www.youtube.com/embed/dzkCrgtfiiY" allowfullscreen></iframe> -->
      <p class="small">Burada dərs videoları və ya yükləmə linkləri görünəcək. (Sən əlavə edəcəksən)</p>
    </div>
  </div>

  <!-- İngilis -->
  <div class="course" id="courseEn">
    <h2>🇬🇧 English Course</h2>
    <p class="price">Price: <strong>10 AZN</strong></p>
    <p class="meta"><strong>Card:</strong> 5411 **** **** 1013 • <strong>Name:</strong> Khayal Garibov • <strong>Bank:</strong> Leobank</p>

    <div class="row">
      <a class="btn" href="https://wa.me/994514852886?text=Salam,%20İngilis%20kursu%20üçün%2010%20AZN%20ödenis%20etmək%20istəyirəm.%20Adım:%20[Adınızı%20yazın]" target="_blank" rel="noopener">
        📲 WhatsApp ilə ödəniş etmək istəyirəm
      </a>
      <a class="btn orange" href="https://wa.me/994514852886?text=Salam,%20İngilis%20kursu%20haqqında%20əlavə%20məlumat%20istəyirəm.%20Ad:%20[Adınız]" target="_blank" rel="noopener">
        ℹ️ More info
      </a>
    </div>

    <div class="notice">Ödənişi yoxlayıb, unik şifrə yaradıb WhatsApp ilə göndərin.</div>

    <div class="gen-row">
      <input type="text" id="ownerGenEn" placeholder="Yeni şifrə (owner üçün)" readonly>
      <button onclick="generatePassword('En')">Generate password</button>
      <button class="copy-btn" onclick="copyOwnerPassword('En')">Copy</button>
      <span class="small">— Send this code to buyer after payment.</span>
    </div>

    <div style="margin-top:12px">
      <input type="password" id="passEn" placeholder="Enter password">
      <button onclick="checkPass('En')">Enter</button>
      <p id="errEn" class="small" style="color:#c00;display:none">Wrong password</p>
    </div>

    <div class="video-box" id="contentEn">
      <h3>📚 English Course — Content</h3>
      <p class="small">Add YouTube embeds or file links here.</p>
    </div>
  </div>

  <!-- Türkçe -->
  <div class="course" id="courseTr">
    <h2>🇹🇷 Türkçe Kurs</h2>
    <p class="price">Fiyat: <strong>15 AZN</strong></p>
    <p class="meta"><strong>Kart:</strong> 5411 **** **** 1013 • <strong>Ad:</strong> Khayal Garibov • <strong>Bank:</strong> Leobank</p>

    <div class="row">
      <a class="btn" href="https://wa.me/994514852886?text=Salam,%20Türkcə%20kursu%20üçün%2015%20AZN%20ödenis%20etmək%20istəyirəm.%20Adım:%20[Adınızı%20yazın]" target="_blank" rel="noopener">
        📲 WhatsApp ilə ödəniş etmək istəyirəm
      </a>
      <a class="btn orange" href="https://wa.me/994514852886?text=Salam,%20Türkcə%20kursu%20haqqında%20əlavə%20məlumat%20istəyirəm.%20Ad:%20[Adınız]" target="_blank" rel="noopener">
        ℹ️ Daha çox məlumat
      </a>
    </div>

    <div class="notice">Ödənişi təsdiqləyib unik şifrə verin.</div>

    <div class="gen-row">
      <input type="text" id="ownerGenTr" placeholder="Yeni şifrə (owner üçün)" readonly>
      <button onclick="generatePassword('Tr')">Şifrə yarat</button>
      <button class="copy-btn" onclick="copyOwnerPassword('Tr')">Kopyala</button>
      <span class="small">— Alıcıya WhatsApp ilə göndərin.</span>
    </div>

    <div style="margin-top:12px">
      <input type="password" id="passTr" placeholder="Şifrənizi daxil edin">
      <button onclick="checkPass('Tr')">Giriş</button>
      <p id="errTr" class="small" style="color:#c00;display:none">Yanlış şifrə</p>
    </div>

    <div class="video-box" id="contentTr">
      <h3>📚 Türk Kursu — İçerik</h3>
      <p class="small">YouTube videoları və ya yükləmə linkləri bura əlavə edin.</p>
    </div>
  </div>

<script>
  // Başlanğıcda heç bir publik şifrə yoxdur;
  // Owner şifrə yarat düyməsi ilə unik kod yaradar və alıcıya WhatsApp ilə göndərər.
  const valid = {
    Az: [], // misal: ["AZ-0001"]
    En: [],
    Tr: []
  };

  // Random şifrə generator (8 simvol: hərf+rəqəm)
  function generatePassword(lang) {
    const charset = "ABCDEFGHJKLMNPQRSTUVWXYZabcdefghijkmnpqrstuvwxyz23456789";
    let pw = "";
    for (let i=0;i<8;i++) pw += charset.charAt(Math.floor(Math.random()*charset.length));
    // əlavə et massivə
    valid[lang].push(pw);
    // göstər owner sahəsində
    document.getElementById("ownerGen" + lang).value = pw;
    alert("Yeni şifrə yaradıldı: " + pw + "\nİndi WhatsApp ilə alıcıya göndərin.");
  }

  function copyOwnerPassword(lang) {
    const val = document.getElementById("ownerGen" + lang).value;
    if (!val) { alert("Əvvəlcə 'Şifrə yarat' düyməsinə basın."); return; }
    navigator.clipboard.writeText(val).then(()=>{
      alert("Şifrə clipboard-a kopyalandı: " + val);
    }, ()=>{ alert("Kopyalama alınmadı. Şifrəni əllə kopyalayın: " + val); });
  }

  // Şifrə yoxlama (istifadəçi daxil etdiyi şifrə valid massivində varsa content göstər)
  function checkPass(lang) {
    const pass = document.getElementById("pass" + lang).value.trim();
    const arr = valid[lang];
    const errId = "err" + lang;
    const contentId = "content" + lang;
    if (arr.includes(pass)) {
      document.getElementById(contentId).style.display = "block";
      document.getElementById(errId).style.display = "none";
    } else {
      document.getElementById(errId).style.display = "block";
      document.getElementById(contentId).style.display = "none";
    }
  }
</script>

</body>
</html>
