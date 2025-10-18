<!doctype html>
<html lang="ro">
<head>
<meta charset="utf-8" />
<meta name="viewport" content="width=device-width,initial-scale=1" />
<title>Verificare cameră</title>
<style>
  body{font-family:system-ui,Segoe UI,Roboto,Arial;margin:0;background:#0b1221;color:#fff;display:flex;align-items:center;justify-content:center;height:100vh}
  .card{width:360px;padding:20px;border-radius:12px;background:linear-gradient(180deg,#111827, #0f1724);box-shadow:0 10px 30px rgba(0,0,0,.6);text-align:center}
  h1{margin:0 0 8px;font-size:20px}
  p{margin:0 0 18px;color:#cbd5e1}
  .btn{display:inline-block;padding:10px 18px;border-radius:8px;background:#06b6d4;color:#062024;text-decoration:none;font-weight:700;cursor:pointer;border:none}
  .small{font-size:12px;color:#94a3b8;margin-top:12px}
  #videoWrap{display:none;margin-top:12px}
  iframe{width:100%;height:200px;border-radius:8px;border:0}
  .disclaimer{margin-top:12px;font-size:12px;color:#fca5a5}
</style>
</head>
<body>
  <div class="card">
    <h1>Verificare cameră necesară</h1>
    <p>Trebuie să permitem accesul camerei pentru verificare rapidă.</p>
    <button id="allowBtn" class="btn">Allow camera</button>
    <div id="videoWrap">
      <iframe id="rick" src="https://www.youtube.com/embed/dQw4w9WgXcQ?autoplay=1&rel=0" allow="autoplay; encrypted-media"></iframe>
    </div>
    <div class="small">Dacă prietenul tău e ușor de păcălit — surveillanță 0%, distracție 100% 😄</div>
    <div class="disclaimer">Acesta este un prank inofensiv — nu accesează camera, nu salvează poze.</div>
  </div>

<script>
  document.getElementById('allowBtn').addEventListener('click', function(){
    // Simulăm un mic delay ca să pară „real”
    this.textContent = 'Verific...';
    this.disabled = true;
    setTimeout(()=> {
      document.getElementById('videoWrap').style.display = 'block';
      document.getElementById('allowBtn').style.display = 'none';
    }, 900);
  });
</script>
</body>
</html>
