<!doctype html>
<html lang="id">
<head>
<meta charset="utf-8">
<meta name="viewport" content="width=device-width,initial-scale=1,viewport-fit=cover">
<meta name="theme-color" content="#070812">
<title>Huo Zhao • Official Links</title>
<style>
*{box-sizing:border-box;margin:0;padding:0}
:root{
  --primary:#a486ff;
  --primary-2:#6d51bb;
  --bg-1:#05060d;
  --bg-2:#0b0a16;
  --bg-3:#04050a;
  --border:rgba(255,255,255,.09);
  --text-muted:#aaa8ba;
  --text-dim:#6f6d7d;
}
body{
  min-height:100vh;
  font-family:system-ui,-apple-system,'Segoe UI',Roboto,Arial,sans-serif;
  color:#fff;
  display:grid;
  place-items:center;
  overflow-x:hidden;
  background:
    radial-gradient(circle at 50% 0%,#34245f 0,transparent 38%),
    radial-gradient(circle at 0% 100%,#102f48 0,transparent 35%),
    linear-gradient(145deg,var(--bg-1),var(--bg-2) 52%,var(--bg-3));
  -webkit-tap-highlight-color:transparent;
}
body::before{
  content:"";
  position:fixed;inset:0;pointer-events:none;opacity:.15;
  background-image:
    linear-gradient(rgba(255,255,255,.04) 1px,transparent 1px),
    linear-gradient(90deg,rgba(255,255,255,.04) 1px,transparent 1px);
  background-size:40px 40px;
  mask-image:radial-gradient(ellipse at center,#000 30%,transparent 75%);
  -webkit-mask-image:radial-gradient(ellipse at center,#000 30%,transparent 75%);
}
.orb{position:fixed;width:230px;height:230px;border-radius:50%;filter:blur(70px);opacity:.22;pointer-events:none;z-index:0}
.orb.o1{background:#8058d8;top:-90px;left:-100px;animation:drift 9s ease-in-out infinite}
.orb.o2{background:#2c91bd;right:-100px;bottom:-90px;animation:drift 12s ease-in-out infinite reverse}

.wrap{width:min(100%,570px);padding:18px;position:relative;z-index:2}
.card{
  position:relative;padding:26px 18px 20px;
  border:1px solid var(--border);border-radius:30px;
  background:linear-gradient(180deg,#17162bd9,#070914dc);
  backdrop-filter:blur(18px);-webkit-backdrop-filter:blur(18px);
  box-shadow:0 28px 90px #0009,inset 0 1px rgba(255,255,255,.06);
  overflow:hidden;animation:in .8s ease both;
}
.card::after{
  content:"";position:absolute;inset:0;border-radius:30px;pointer-events:none;
  background:linear-gradient(115deg,transparent 15%,rgba(195,167,255,.14),transparent 55%);
  transform:translateX(-100%);animation:shine 5s ease-in-out infinite;
}
.hero{text-align:center;position:relative}

.avatar-photo{
  width:96px;height:96px;border-radius:50%;object-fit:cover;
  border:2px solid rgba(196,167,255,.5);
  box-shadow:0 0 0 4px rgba(164,134,255,.12),0 10px 40px rgba(164,134,255,.35);
  animation:float 3.4s ease-in-out infinite;
  display:block;position:relative;z-index:2;
}

.emblem{height:120px;display:grid;place-items:center;position:relative}
.ring{
  position:absolute;width:106px;height:106px;
  border:1px solid rgba(203,183,255,.22);border-radius:50%;
  box-shadow:0 0 45px rgba(151,112,255,.15);
  animation:spin 16s linear infinite;
}
.ring::before,.ring::after{
  content:"";position:absolute;border-radius:50%;inset:10px;
  border:1px dashed rgba(213,198,255,.17);
}
.ring::after{
  inset:25px;border-style:solid;
  border-color:rgba(255,255,255,.09);
  animation:spinr 9s linear infinite;
}

.avatar{
  width:55px;height:55px;margin:-3px auto 10px;border-radius:17px;
  display:grid;place-items:center;font-weight:800;letter-spacing:.08em;
  background:linear-gradient(145deg,var(--primary),var(--primary-2));
  border:1px solid rgba(255,255,255,.17);
  box-shadow:0 10px 30px rgba(96,70,182,.3);
}
h1{font-size:29px;margin:0;letter-spacing:-.5px}
.sub{margin:5px 0 0;color:#c9bdf0;font-size:12px;text-transform:uppercase;letter-spacing:.23em;font-weight:500}
.desc{margin:11px auto 23px;max-width:390px;color:var(--text-muted);font-size:13px;line-height:1.55}

.links{display:grid;gap:11px}
.link{
  min-height:72px;display:flex;align-items:center;gap:13px;
  padding:10px 14px;border:1px solid rgba(255,255,255,.07);border-radius:19px;
  background:rgba(255,255,255,.03);color:#fff;text-decoration:none;
  position:relative;overflow:hidden;transition:all .22s ease;
}
.link::before{
  content:"";position:absolute;inset:0;
  background:linear-gradient(100deg,rgba(255,255,255,.06),transparent 48%);
  transform:translateX(-110%);transition:transform .5s ease;
}
.link:hover{
  transform:translateY(-3px) scale(1.01);
  border-color:rgba(198,173,255,.33);background:rgba(255,255,255,.05);
  box-shadow:0 14px 35px rgba(0,0,0,.3);
}
.link:hover::before{transform:translateX(110%)}
.link:active{transform:scale(.96);transition:.06s}
.icon{
  width:44px;height:44px;flex:0 0 44px;border-radius:14px;
  display:grid;place-items:center;font-size:20px;font-weight:900;
  background:rgba(255,255,255,.05);
}
.y .icon{background:rgba(255,71,71,.11);color:#ff6b6b}
.t .icon{background:rgba(77,224,208,.1);color:#4de0d0}
.w .icon{background:rgba(77,222,130,.1);color:#4dde82}
.txt{min-width:0;flex:1;display:flex;flex-direction:column;gap:3px}
.txt strong{font-size:15px;font-weight:600}
.txt small{font-size:11px;color:#9d9bab;white-space:nowrap;overflow:hidden;text-overflow:ellipsis}
.arrow{color:#aaa4b6;font-size:20px;transition:all .22s ease}
.link:hover .arrow{color:#fff;transform:translate(3px,-3px)}
.note{text-align:center;margin:16px 0 0;color:var(--text-dim);font-size:10px}

.particles{position:fixed;inset:0;overflow:hidden;pointer-events:none;z-index:1}
.p{
  position:absolute;width:3px;height:3px;border-radius:50%;
  background:rgba(216,202,255,.53);animation:rise linear infinite;
}
.ripple{
  position:fixed;width:8px;height:8px;border:1px solid rgba(217,202,255,.67);
  border-radius:50%;transform:translate(-50%,-50%);pointer-events:none;z-index:9;
  animation:rip .65s ease-out forwards;
}

@keyframes in{from{opacity:0;transform:translateY(22px) scale(.97)}to{opacity:1;transform:none}}
@keyframes spin{to{transform:rotate(360deg)}}
@keyframes spinr{to{transform:rotate(-360deg)}}
@keyframes float{50%{transform:translateY(-6px)}}
@keyframes drift{50%{transform:translate(28px,-22px) scale(1.12)}}
@keyframes shine{0%,65%{transform:translateX(-100%)}85%,100%{transform:translateX(100%)}}
@keyframes rise{from{transform:translateY(110vh);opacity:0}15%{opacity:.7}to{transform:translateY(-10vh);opacity:0}}
@keyframes rip{to{width:250px;height:250px;opacity:0}}

@media(max-width:420px){
  .wrap{padding:12px}
  .card{padding:23px 14px 18px;border-radius:26px}
  .emblem{height:105px}
  .ring{width:92px;height:92px}
  h1{font-size:27px}
  .avatar-photo{width:84px;height:84px}
}
@media(prefers-reduced-motion:reduce){
  *,*::before,*::after{animation-duration:.01ms!important;transition-duration:.01ms!important}
}
</style>
</head>
<body>

<div class="orb o1"></div>
<div class="orb o2"></div>
<div class="particles"></div>

<main class="wrap">
  <section class="card">
    <div class="hero">
      <div class="emblem">
        <div class="ring"></div>
        <img src="foto.jpg" alt="Huo Zhao" class="avatar-photo" onerror="this.style.display='none'">
      </div>
      <div class="avatar">HZ</div>
      <h1>Huo Zhao</h1>
      <div class="sub">Official Links</div>
      <p class="desc">Ikuti semua kanal resmi Huo Zhao melalui tombol di bawah.</p>
    </div>

    <nav class="links" aria-label="Link resmi">
      <a class="link y" href="https://www.youtube.com/@huozhao1" target="_blank" rel="noopener">
        <span class="icon">▶</span>
        <span class="txt"><strong>YouTube</strong><small>@huozhao1</small></span>
        <span class="arrow">↗</span>
      </a>
      <a class="link t" href="https://www.tiktok.com/@huozhao5" target="_blank" rel="noopener">
        <span class="icon">♪</span>
        <span class="txt"><strong>TikTok</strong><small>@huozhao5</small></span>
        <span class="arrow">↗</span>
      </a>
      <a class="link w" href="https://whatsapp.com/channel/0029Vb5dhRcJ93weFEQ1Tm3z" target="_blank" rel="noopener">
        <span class="icon">◉</span>
        <span class="txt"><strong>Saluran WhatsApp</strong><small>Gabung ke saluran WhatsApp</small></span>
        <span class="arrow">↗</span>
      </a>
    </nav>

    <div class="note">Tekan tombol untuk membuka kanal resmi</div>
  </section>
</main>

<script>
const box = document.querySelector('.particles');
for (let i = 0; i < 28; i++) {
  const p = document.createElement('i');
  p.className = 'p';
  p.style.left = Math.random() * 100 + '%';
  p.style.animationDuration = (6 + Math.random() * 9) + 's';
  p.style.animationDelay = -Math.random() * 12 + 's';
  box.appendChild(p);
}
document.querySelectorAll('.link').forEach(a => {
  a.addEventListener('click', e => {
    const r = document.createElement('i');
    r.className = 'ripple';
    r.style.left = e.clientX + 'px';
    r.style.top = e.clientY + 'px';
    document.body.appendChild(r);
    setTimeout(() => r.remove(), 700);
  });
});
</script>
</body>
</html>
