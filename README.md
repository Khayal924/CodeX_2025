<!DOCTYPE html>
<html lang="az">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Onlayn Kurs — Proqramlaşdırma Öyrən</title>
  <style>
    body {
      font-family: Arial, sans-serif;
      background: #f2f2f2;
      padding: 20px;
      text-align: center;
    }
    h1 {
      color: #333;
    }
    .video {
      max-width: 560px;
      margin: 20px auto;
      border-radius: 10px;
      overflow: hidden;
      box-shadow: 0 4px 8px rgba(0,0,0,0.1);
      display: none; /* Şifrə yoxdursa gizli */
    }
    iframe {
      width: 100%;
      height: 315px;
      border: none;
    }
    input {
      padding: 10px;
      font-size: 16px;
      width: 200px;
      margin-top: 20px;
    }
    button {
      padding: 10px 15px;
      font-size: 16px;
      cursor: pointer;
      margin-left: 5px;
    }
    p {
      color: red;
      font-weight: bold;
    }
  </style>
</head>
<body>

<h1>📚 Proqramlaşdırma Öyrən — Onlayn Kurs</h1>
<p>Videoya baxmaq üçün ödəniş etdikdən sonra şifrəni daxil edin:</p>

<input type="password" id="passInput" placeholder="Şifrəni daxil edin">
<button onclick="checkPassword()">Təsdiqlə</button>
<p id="errorMsg"></p>

<!-- Videoların blokları -->
<div class="video" id="video1">
  <h3>Proqramlaşdırma Öyrən — Dərs 1</h3>
  <iframe src="https://www.youtube.com/embed/dzkCrgtfiiY" allowfullscreen></iframe>
</div>

<script>
  // Burada şifrələri təyin edirsən
  const passwords = {
    video1: "1234" // Ödəniş edənlər üçün şifrə
  };

  function checkPassword() {
    const input = document.getElementById("passInput").value;
    let anyCorrect = false;

    for (let videoId in passwords) {
      if(input === passwords[videoId]) {
        document.getElementById(videoId).style.display = "block";
        anyCorrect = true;
      } else {
        document.getElementById(videoId).style.display = "none";
      }
    }

    const errorMsg = document.getElementById("errorMsg");
    if(anyCorrect) {
      errorMsg.textContent = "";
    } else {
      errorMsg.textContent = "Yanlış şifrə! Ödəniş etməmisinizsə, link almaq üçün bizimlə əlaqə saxlayın.";
    }
  }
</script>

</body>
</html>
