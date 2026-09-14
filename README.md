<!DOCTYPE html>
<html lang="id">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width,initial-scale=1.0">

<title>Huo Zhao • Official Links</title>

https://fonts.googleapis.com/css2?family=Poppins:wght@300;400;500;700;800&display=swap

<style>

:root{
--primary:#9F75FF;
--bg:#050816;
}

*{
margin:0;
padding:0;
box-sizing:border-box;
}

body{
font-family:'Poppins',sans-serif;
min-height:100vh;
display:flex;
justify-content:center;
align-items:center;
overflow:hidden;
background:var(--bg);
color:white;
position:relative;
}

/* AURORA */

body::before{
content:"";
position:fixed;
inset:0;
background:
radial-gradient(circle at 20% 20%,#8d5eff55,transparent 35%),
radial-gradient(circle at 80% 80%,#00cfff33,transparent 35%),
radial-gradient(circle at 50% 10%,#ff66ff22,transparent 40%);
filter:blur(90px);
animation:aurora 12s ease-in-out infinite alternate;
}

@keyframes aurora{
100%{
transform:scale(1.3) rotate(15deg);
}
}

/* GRID */

body::after{
content:"";
position:fixed;
inset:0;
background-image:
linear-gradient(rgba(255,255,255,.03) 1px,transparent 1px),
linear-gradient(90deg,rgba(255,255,255,.03) 1px,transparent 1px);
background-size:40px 40px;
pointer-events:none;
}

/* LOADER */

#loader{
position:fixed;
inset:0;
background:#050816;
display:flex;
flex-direction:column;
justify-content:center;
align-items:center;
z-index:99999;
transition:1s;
}

#loader.hide{
opacity:0;
visibility:hidden;
}

.loader-logo{
width:120px;
height:120px;
border-radius:50%;
display:flex;
justify-content:center;
align-items:center;
font-size:64px;
background:linear-gradient(135deg,#d3c3ff,#7857ff);
box-shadow:
0 0 40px #9f75ff,
0 0 90px rgba(159,117,255,.45);
animation:pulse 2s infinite;
}

.loader-ring{
position:absolute;
width:160px;
height:160px;
border-radius:50%;
border:2px solid transparent;
border-top-color:white;
border-right-color:#9f75ff;
animation:spin 1s linear infinite;
}

.loader-text{
margin-top:25px;
font-size:13px;
letter-spacing:4px;
}

@keyframes spin{
to{transform:rotate(360deg);}
}

@keyframes pulse{
50%{
transform:scale(1.08);
}
}

/* TRANSITION */

#transition{
position:fixed;
inset:0;
background:#050816;
display:flex;
justify-content:center;
align-items:center;
opacity:0;
visibility:hidden;
transition:.4s;
z-index:99998;
}

#transition.active{
opacity:1;
visibility:visible;
}

/* CARD */

.card{
width:min(92%,580px);
padding:35px 25px;
border-radius:32px;

background:
rgba(20,20,35,.7);

backdrop-filter:blur(20px);

border:1px solid rgba(255,255,255,.08);

box-shadow:
0 25px 80px rgba(0,0,0,.5);

position:relative;
z-index:2;
animation:show 1s ease;
}

@keyframes show{
from{
opacity:0;
transform:translateY(30px);
}
to{
opacity:1;
transform:none;
}
}

/* LOGO */

.logo{
width:130px;
height:130px;
margin:auto;
border-radius:50%;

display:flex;
justify-content:center;
align-items:center;

font-size:72px;
font-weight:700;

background:
linear-gradient(135deg,#cdb8ff,#6c48ff);

box-shadow:
0 0 40px #8f75ff,
0 0 120px rgba(143,117,255,.4);

animation:float 5s ease-in-out infinite;
}

@keyframes float{
50%{
transform:translateY(-10px);
}
}

/* TEXT */

h1{
text-align:center;
font-size:38px;
margin-top:20px;
}

.subtitle{
text-align:center;
font-size:12px;
letter-spacing:5px;
color:#cbbdf5;
margin-top:5px;
}

.desc{
margin-top:15px;
text-align:center;
color:#b1b7ca;
line-height:1.8;
font-size:14px;
}

/* LINKS */

.links{
margin-top:30px;
display:grid;
gap:15px;
}

.link{
position:relative;
overflow:hidden;

display:flex;
align-items:center;
gap:15px;

padding:18px;

border-radius:22px;

background:
rgba(255,255,255,.05);

border:1px solid rgba(255,255,255,.08);

text-decoration:none;
color:white;

transition:
transform .55s cubic-bezier(.22,1,.36,1),
box-shadow .55s cubic-bezier(.22,1,.36,1),
border-color .55s cubic-bezier(.22,1,.36,1);

-webkit-tap-highlight-color:transparent;
}

.link:hover{
transform:translateY(-5px);
border-color:#9f75ff;
box-shadow:
0 15px 40px rgba(159,117,255,.25);
}

/* SHINE */

.link::before{
content:"";
position:absolute;
top:0;
left:-100%;
width:100%;
height:100%;

background:
linear-gradient(
90deg,
transparent,
rgba(255,255,255,.15),
transparent);

transition:.8s;
}

.link:hover::before{
left:120%;
}

/* ICON */

.icon{
width:60px;
height:60px;
border-radius:18px;

display:flex;
align-items:center;
justify-content:center;

position:relative;
overflow:hidden;
}

/* YOUTUBE */

.youtube{
background:#ff000015;
color:#ff4040;
}

.youtube svg{
filter:
drop-shadow(0 0 10px #ff0000)
drop-shadow(0 0 20px rgba(255,0,0,.7));
}

/* TIKTOK */

.tiktok{
background:#25F4EE15;
color:#25F4EE;
}

.tiktok svg{
filter:
drop-shadow(0 0 10px #25F4EE)
drop-shadow(0 0 20px rgba(37,244,238,.7));
}

/* WHATSAPP */

.whatsapp{
background:#25D36615;
color:#25D366;
}

.whatsapp svg{
filter:
drop-shadow(0 0 10px #25D366)
drop-shadow(0 0 20px rgba(37,211,102,.7));
}

.link:hover .icon{
transform:scale(1.1);
transition:.4s;
}

.text{
flex:1;
}

.text strong{
display:block;
}

.text small{
color:#aeb5c5;
}

.arrow{
font-size:22px;
transition:.4s;
}

.link:hover .arrow{
transform:translate(5px,-3px);
}

/* RIPPLE */

.ripple-effect{
position:absolute;
border-radius:50%;
pointer-events:none;

background:
radial-gradient(
circle,
rgba(255,255,255,.45),
rgba(159,117,255,.3),
transparent 70%);

transform:translate(-50%,-50%) scale(0);

animation:ripple .8s ease-out forwards;
}

@keyframes ripple{
to{
transform:translate(-50%,-50%) scale(12);
opacity:0;
}
}

/* PARTICLES */

.particles{
position:fixed;
inset:0;
pointer-events:none;
}

.p{
position:absolute;
width:4px;
height:4px;
border-radius:50%;
background:white;
opacity:.3;
animation:rise linear infinite;
}

@keyframes rise{
from{
transform:translateY(110vh);
}
to{
transform:translateY(-10vh);
}
}

/* FOOTER */

.footer{
margin-top:25px;
text-align:center;
font-size:12px;
color:#7f8796;
}

@media(max-width:480px){

.logo{
width:110px;
height:110px;
font-size:58px;
}

h1{
font-size:32px;
}

}

</style>
</head>

<body>

<!-- LOADER -->

<div id="loader">
<div class="loader-ring"></div>
<div class="loader-logo">龍</div>
<div class="loader-text">LOADING...</div>
</div>

<!-- TRANSITION -->

<div id="transition">
<div class="loader-ring"></div>
<div class="loader-logo">龍</div>
</div>

<div class="particles"></div>

<div class="card">

<div class="logo">龍</div>

<h1>Huo Zhao</h1>

<div class="subtitle">
OFFICIAL LINKS
</div>

<p class="desc">
Ikuti semua kanal resmi Huo Zhao melalui tombol di bawah.
</p>

<div class="links">

<a class="link ripple-btn"
href="https://www.youtube.com/@huozhao1">

<div class="icon youtube">

<svg width="28" height="28" viewBox="0 0 24 24" fill="currentColor">
<path d="M23.5 6.2c-.3-1.2-1.3-2.2-2.5-2.5C18.8 3 12 3 12 3s-6.8 0-9 .7C1.8 4 .8 5 .5 6.2 0 8.4 0 12 0 12s0 3.6.5 5.8c.3 1.2 1.3 2.2 2.5 2.5C5.2 21 12 21 12 21s6.8 0 9-.7c1.2-.3 2.2-1.3 2.5-2.5.5-2.2.5-5.8.5-5.8s0-3.6-.5-5.8zM9.8 15.5V8.5L16 12l-6.2 3.5z"/>
</svg>

</div>

<div class="text">
<strong>YouTube</strong>
<small>@huozhao1</small>
</div>

<div class="arrow">↗</div>

</a>

https://www.tiktok.com/@huozhao5

<div class="icon tiktok">

<svg width="28" height="28" viewBox="0 0 24 24" fill="currentColor">
<path d="M19.6 8.5c-1.6 0-3.1-.5-4.2-1.6v7.2c0 3.3-2.7 6-6 6s-6-2.7-6-6 2.7-6 6-6c.3 0 .6 0 .9.1v3.1c-.3-.1-.6-.2-.9-.2-1.6 0-2.9 1.3-2.9 2.9s1.3 2.9 2.9 2.9 2.9-1.3 2.9-2.9V2h3c.2 1.7 1.5 3.2 3.3 3.8 1 .4 1.7.5 2 .5v2.2z"/>
</svg>

</div>

<div class="text">
<strong>TikTok</strong>
<small>@huozhao5</small>
</div>

<div class="arrow">↗</div>

</a>

<a class="link ripple-btn"
href="https://whatsapp.com/channel/0029Vb5dhRcJ93weFEQ1Tm3z">

<div class="icon whatsapp">

<svg width="28" height="28" viewBox="0 0 24 24" fill="currentColor">
<path d="M12.04 2C6.53 2 2.06 6.46 2.06 11.97c0 1.76.46 3.47 1.34 4.99L2 22l5.19-1.36a10 10 0 0 0 4.85 1.24h.01c5.5 0 9.97-4.47 9.97-9.98C22.02 6.47 17.55 2 12.04 2z"/>
</svg>

</div>

<div class="text">
<strong>WhatsApp Channel</strong>
<small>Gabung Sekarang</small>
</div>

<div class="arrow">↗</div>

</a>

</div>

<div class="footer">
© Huo Zhao Official Links
</div>

</div>

<script>

/* LOADER */

window.addEventListener('load',()=>{

setTimeout(()=>{
document.getElementById('loader').classList.add('hide');
},1800);

});

/* PARTICLES */

const particles=document.querySelector('.particles');

for(let i=0;i<40;i++){

const p=document.createElement('i');

p.className='p';

p.style.left=Math.random()*100+'%';
p.style.animationDuration=(8+Math.random()*10)+'s';
p.style.animationDelay=(-Math.random()*15)+'s';

particles.appendChild(p);

}

/* RIPPLE */

document.querySelectorAll('.ripple-btn').forEach(btn=>{

btn.addEventListener('pointerdown',e=>{

const rect=btn.getBoundingClientRect();

const ripple=document.createElement('span');

ripple.className='ripple-effect';

const size=Math.max(rect.width,rect.height);

ripple.style.width=size+'px';
ripple.style.height=size+'px';

ripple.style.left=(e.clientX-rect.left)+'px';
ripple.style.top=(e.clientY-rect.top)+'px';

btn.appendChild(ripple);

setTimeout(()=>ripple.remove(),800);

});

});

/* PAGE TRANSITION */

document.querySelectorAll('.link').forEach(link=>{

link.addEventListener('click',function(e){

e.preventDefault();

const url=this.href;

document
.getElementById('transition')
.classList.add('active');

setTimeout(()=>{
window.location.href=url;
},1000);

});

});

</script>

</body>
</html>
