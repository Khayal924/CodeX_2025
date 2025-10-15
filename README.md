<!doctype html>
<html lang="az">
<head>
  <meta charset="utf-8"/>
  <meta name="viewport" content="width=device-width,initial-scale=1"/>
  <title>Proqramlaşdırma Kursu</title>
  <style>
    :root{--bg:#f3f4f6;--card:#ffffff;--accent:#25D366;--muted:#666;}
    body{margin:0;font-family:system-ui,-apple-system,Segoe UI,Roboto,Arial;background:var(--bg);color:#111}
    .wrap{max-width:900px;margin:18px auto;padding:16px}
    header{background:#111;color:#fff;padding:18px;border-radius:10px;text-align:center}
    main{background:var(--card);padding:18px;border-radius:12px;margin-top:14px;box-shadow:0 6px 22px rgba(0,0,0,0.06)}
    h1,h2{margin:0 0 8px 0}
    p{margin:8px 0 12px 0;line-height:1.45}
    .btn{display:inline-block;padding:12px 16px;border-radius:8px;text-decoration:none;font-weight:600}
    .wh{background:var(--accent);color:#fff}
    .pay-box{background:#f9fafb;padding:12px;border-radius:10px;margin-top:12px;font-size:15px}
    .pay-row{display:flex;justify-content:space-between;align-items:center;gap:10px;flex-wrap:wrap}
    .muted{color:var(--muted);font-size:14px}
    .copy-btn{padding:8px 10px;border-radius:8px;border:1px solid #ddd;background:#fff}
    .video{position:relative;padding-bottom:56.25%;height:0;overflow:hidden;border-radius:10px;margin-top:14px}
    .video iframe{position:absolute;left:0;top:0;width:100%;height:100%;border:0}
    footer{margin-top:14px;text-align:center;color:var(--muted);font-size:13px}
    .small{font-size:13px;color:var(--muted)}
    @media(max-width:420px){.pay-row{flex-direction:column;align-items:flex-start}}
  </style>
</head>
<body>
  <div class="wrap">
    <header>
      <h1>Proqramlaşdırma Kursu</h1>
      <p class="small">Hər gün yeni dərslər — telefonla öyrən</p>
    </header>

    <main>
      <h2>Kursa qoşulmaq üçün</h2>
      <p>Ödənişi kartla et və dərhal WhatsApp vasitəsilə bizə yaz. Ödəniş təsdiqləndikdən sonra dərs linklərini göndərəcəyik.</p>

      <!-- WhatsApp düyməsi -->
      <a class="btn wh" href="https://wa.me/994514852886?text=Salam,%20kurs%20haqq%C4%B1nda%20m%C9%99lumat%20ist%C9%99yir%C9%99m." target="_blank" rel="noopener">
        WhatsApp ilə yaz 📲
      </a>

      <!-- Kart məlumatı -->
      <div class="pay-box" style="margin-top:14px">
        <div class="pay-row">
          <div>
            <div><strong>Kart nömrəsi:</strong> <span id="card-masked">5411 **** **** 1013</span></div>
            <div class="muted"><strong>Ad:</strong> Khayal Garibov</div>
            <div class="muted"><strong>Bank:</strong> Leobank</div>
            <div class="muted"><strong>Məbləğ:</strong> 10 AZN</div>
          </div>
          <div style="display:flex;flex-direction:column;gap:8px">
            <button class="copy-btn" id="show-card">Kartı göstər</button>
            <button class="copy-btn" id="copy-card">Kartı kopyala</button>
          </div>
        </div>
        <p class="small" style="margin-top:10px">
          Qeyd: Kart nömrəsi təhlükəsizlik üçün maskalanıb. “Kartı göstər” düyməsinə basaraq tam nömrəni görə və kopyalaya bilərsiniz.
        </p>
      </div>

      <hr style="margin:18px 0">

      <h3>Dərslər</h3>
      <p>Videoları sonradan buraya əlavə edəcəksiniz. Hər video üçün aşağıdakı kodu istifadə edin:</p>
      <pre class="small" style="background:#f1f1f1;padding:10px;border-radius:8px;overflow:auto"
<h3>Test Video — 16 Oktyabr 2025</h3>
<div class="video">
  <iframe src="https://www.youtube.com/embed/dzkCrgtfiiY" allowfullscreen></iframe>
</div>
      <!-- Nümunə video -->
      <!--
      <div class="video">
        <iframe src="https://www.youtube.com/embed/VIDEO_ID" allowfullscreen></iframe>
      </div>
      -->

      <footer>
        <p class="small">© 2025 — Proqramlaşdırma Kursu | Əlaqə: WhatsApp ilə yaz</p>
      </footer>
    </main>
  </div>

  <script>
    const FULL_CARD = "5411249812061013";
    const showBtn = document.getElementById("show-card");
    const copyBtn = document.getElementById("copy-card");
    const cardMasked = document.getElementById("card-masked");
    let shown = false;

    showBtn.addEventListener("click", () => {
      if(!shown){
        cardMasked.textContent = FULL_CARD;
        showBtn.textContent = "Kartı gizlət";
        shown = true;
      } else {
        cardMasked.textContent = FULL_CARD.slice(0,4) + " **** **** " + FULL_CARD.slice(-4);
        showBtn.textContent = "Kartı göstər";
        shown = false;
      }
    });

    copyBtn.addEventListener("click", async () => {
      try {
        await navigator.clipboard.writeText(FULL_CARD);
        copyBtn.textContent = "Kopyalandı ✓";
        setTimeout(()=> copyBtn.textContent = "Kartı kopyala", 1800);
      } catch(e) {
        alert("Kopyalama alınmadı. Kart nömrəsi: " + FULL_CARD);
      }
    });

    cardMasked.textContent = FULL_CARD.slice(0,4) + " **** **** " + FULL_CARD.slice(-4);
  </script>
</body>
</html>

