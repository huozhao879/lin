<!doctype html>
<html lang="id">
<head>
<meta charset="utf-8">
<meta name="viewport" content="width=device-width,initial-scale=1,viewport-fit=cover">
<meta name="theme-color" content="#020617">
<title>Huo Zhao • Official Links</title>
<style>
*{margin:0;padding:0;box-sizing:border-box;-webkit-tap-highlight-color:transparent}
body{
  min-height:100vh;
  font-family:system-ui,-apple-system,'Segoe UI',Roboto,sans-serif;
  color:#e2e8f0;
  background:#020617;
  display:flex;
  justify-content:center;
  align-items:center;
  padding:20px;
  overflow-x:hidden;
  position:relative;
}
/* Cahaya background */
body::before{
  content:"";
  position:fixed;
  top:-200px;left:50%;
  width:600px;height:600px;
  transform:translateX(-50%);
  background:radial-gradient(circle,#0ea5e9 0%,transparent 60%);
  opacity:.15;
  pointer-events:none;
  filter:blur(60px);
}
body::after{
  content:"";
  position:fixed;
  bottom:-200px;right:-100px;
  width:500px;height:500px;
  background:radial-gradient(circle,#06b6d4 0%,transparent 60%);
  opacity:.12;
  pointer-events:none;
  filter:blur(60px);
}
.box{
  width:100%;
  max-width:480px;
  position:relative;
  z-index:1;
}
/* Kartu utama */
.card{
  background:rgba(15,23,42,.7);
  border:1px solid rgba(14,165,233,.25);
  border-radius:24px;
  padding:32px 20px 24px;
  backdrop-filter:blur(20px);
  -webkit-backdrop-filter:blur(20px);
  box-shadow:
    0 0 60px rgba(14,165,233,.15),
    0 20px 50px rgba(0,0,0,.5);
  position:relative;
  overflow:hidden;
}
.card::before{
  content:"";
  position:absolute;
  top:0;left:0;right:0;
  height:1px;
  background:linear-gradient(90deg,transparent,#0ea5e9,transparent);
}
/* Foto profil */
.photo-wrap{
  display:flex;
  justify-content:center;
  margin-bottom:16px;
  position:relative;
}
.photo-wrap::before{
  content:"";
  position:absolute;
  width:110px;height:110px;
  border-radius:50%;
  border:2px dashed rgba(14,165,233,.4);
  animation:rotate 20s linear infinite;
}
.photo-wrap::after{
  content:"";
  position:absolute;
  width:130px;height:130px;
  border-radius:50%;
  border:1px solid rgba(14,165,233,.15);
  animation:rotate 30s linear infinite reverse;
}
.photo{
  width:90px;height:90px;
  border-radius:50%;
  object-fit:cover;
  border:3px solid #0ea5e9;
  box-shadow:0 0 30px rgba(14,165,233,.5);
  position:relative;
  z-index:1;
  background:#0f172a;
}
/* Fallback kalau foto tidak ada */
.photo-fallback{
  width:90px;height:90px;
  border-radius:50%;
  display:grid;
  place-items:center;
  font-size:32px;
  font-weight:900;
  color:#0ea5e9;
  background:#0f172a;
  border:3px solid #0ea5e9;
  box-shadow:0 0 30px rgba(14,165,233,.5);
  position:relative;
  z-index:1;
}
/* Nama */
.name{
  text-align:center;
  font-size:26px;
  font-weight:800;
  color:#fff;
  letter-spacing:-.5px;
  margin-bottom:6px;
}
.name span{color:#0ea5e9}
.tagline{
  text-align:center;
  font-size:11px;
  color:#64748b;
  letter-spacing:.3em;
  text-transform:uppercase;
  font-weight:600;
  margin-bottom:8px;
}
.bio{
  text-align:center;
  font-size:13px;
  color:#94a3b8;
  line-height:1.5;
  margin-bottom:24px;
  padding:0 10px;
}
/* Tombol link */
.links{
  display:flex;
  flex-direction:column;
  gap:10px;
}
.btn{
  display:flex;
  align-items:center;
  gap:14px;
  padding:14px 16px;
  background:rgba(30,41,59,.6);
  border:1px solid rgba(51,65,85,.6);
  border-radius:14px;
  color:#e2e8f0;
  text-decoration:none;
  transition:all .25s ease;
  position:relative;
  overflow:hidden;
}
.btn::before{
  content:"";
  position:absolute;
  left:0;top:0;bottom:0;
  width:3px;
  background:#0ea5e9;
  transform:scaleY(0);
  transition:transform .25s ease;
  transform-origin:center;
}
.btn:hover{
  background:rgba(30,41,59,.9);
  border-color:rgba(14,165,233,.5);
  transform:translateX(4px);
  box-shadow:0 8px 24px rgba(14,165,233,.15);
}
.btn:hover::before{transform:scaleY(1)}
.btn:active{transform:scale(.98)}
.btn-icon{
  width:40px;height:40px;
  flex:0 0 40px;
  display:grid;
  place-items:center;
  border-radius:10px;
  font-size:18px;
  background:rgba(14,165,233,.15);
  color:#0ea5e9;
  font-weight:900;
}
.btn-icon.red{background:rgba(239,68,68,.15);color:#ef4444}
.btn-icon.cyan{background:rgba(6,182,212,.15);color:#06b6d4}
.btn-icon.green{background:rgba(34,197,94,.15);color:#22c55e}
.btn-text{
  flex:1;
  min-width:0;
}
.btn-text b{
  display:block;
  font-size:14px;
  font-weight:700;
  margin-bottom:2px;
}
.btn-text small{
  font-size:11px;
  color:#64748b;
  display:block;
  white-space:nowrap;
  overflow:hidden;
  text-overflow:ellipsis;
}
.btn-arrow{
  color:#475569;
  font-size:16px;
  transition:all .25s ease;
}
.btn:hover .btn-arrow{
  color:#0ea5e9;
  transform:translateX(3px);
}
/* Footer */
.footer{
  text-align:center;
  font-size:10px;
  color:#475569;
  margin-top:18px;
  padding-top:16px;
  border-top:1px solid rgba(51,65,85,.3);
}
/* Animasi */
@keyframes rotate{to{transform:rotate(360deg)}}
/* Responsive */
@media(max-width:400px){
  .card{padding:26px 16px 20px;border-radius:20px}
  .photo,.photo-fallback{width:80px;height:80px}
  .photo-wrap::before{width:96px;height:96px}
  .photo-wrap::after{width:114px;height:114px}
  .name{font-size:22px}
  .btn{padding:12px 14px}
}
@media(prefers-reduced-motion:reduce){
  *{animation:none!important;transition:none!important}
}
</style>
</head>
<body>

<div class="box">
  <div class="card">

    <!-- FOTO PROFIL -->
    <div class="photo-wrap">
      <!-- Ganti "foto.jpg" dengan nama file foto kamu -->
      <img src="foto.jpg" alt="Huo Zhao" class="photo" onerror="this.outerHTML='<div class=&quot;photo-fallback&quot;>龍</div>'">
    </div>

    <!-- NAMA -->
    <div class="name">Huo <span>Zhao</span></div>
    <div class="tagline">Official Links</div>
    <div class="bio">Ikuti semua kanal resmi Huo Zhao melalui tombol di bawah ini.</div>

    <!-- TOMBOL LINK -->
    <div class="links">

      <a class="btn" href="https://www.youtube.com/@huozhao1" target="_blank" rel="noopener">
        <div class="btn-icon red">▶</div>
        <div class="btn-text">
          <b>YouTube</b>
          <small>@huozhao1</small>
        </div>
        <div class="btn-arrow">→</div>
      </a>

      <a class="btn" href="https://www.tiktok.com/@huozhao5" target="_blank" rel="noopener">
        <div class="btn-icon cyan">♪</div>
        <div class="btn-text">
          <b>TikTok</b>
          <small>@huozhao5</small>
        </div>
        <div class="btn-arrow">→</div>
      </a>

      <a class="btn" href="https://whatsapp.com/channel/0029Vb5dhRcJ93weFEQ1Tm3z" target="_blank" rel="noopener">
        <div class="btn-icon green">◉</div>
        <div class="btn-text">
          <b>Saluran WhatsApp</b>
          <small>Gabung ke saluran WhatsApp</small>
        </div>
        <div class="btn-arrow">→</div>
      </a>

    </div>

    <div class="footer">Tekan tombol untuk membuka kanal resmi</div>
  </div>
</div>

</body>
</html>
