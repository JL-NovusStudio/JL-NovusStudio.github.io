[index.html](https://github.com/user-attachments/files/35528692/index.html)
<!doctype html>
<html lang="es" data-theme="light">
<head>
<meta charset="utf-8">
<meta name="viewport" content="width=device-width, initial-scale=1">
<title>Novus Studio — Estudio Creativo Digital</title>
<meta name="description" content="Marketing digital, branding y desarrollo web para marcas que quieren verse y crecer como líderes.">
<meta property="og:title" content="Novus Studio — Estudio Creativo Digital">
<meta property="og:description" content="Marketing digital, branding y desarrollo web.">
<meta property="og:image" content="assets/og-image.jpg">
<meta property="og:type" content="website">
<meta property="og:locale" content="es_PE">
<meta name="robots" content="index, follow">
<script type="application/ld+json">
{
  "@context": "https://schema.org",
  "@type": "ProfessionalService",
  "name": "JL Novus Studio",
  "alternateName": "Novus Studio",
  "description": "Estudio creativo digital: marketing digital, branding y desarrollo web.",
  "image": "assets/og-image.jpg",
  "telephone": "+51 938 437 193",
  "email": "7.jhuliniolopez@gmail.com",
  "address": { "@type": "PostalAddress", "addressLocality": "Cajamarca", "addressCountry": "PE" },
  "areaServed": "PE",
  "openingHoursSpecification": [{
    "@type": "OpeningHoursSpecification",
    "dayOfWeek": ["Monday","Tuesday","Wednesday","Thursday","Friday","Saturday"],
    "opens": "09:00", "closes": "19:00"
  }],
  "url": "https://jl-novusstudio.github.io/",
  "sameAs": [
    "https://www.instagram.com/jlnovusstudio",
    "https://www.facebook.com/share/1CuWkR24iw/",
    "https://www.linkedin.com/in/nilson-jhulinio-lopez-verastegui-5a494a190"
  ]
}
</script>
<link rel="icon" type="image/png" href="assets/favicon-32.png">
<link rel="apple-touch-icon" href="assets/apple-touch-icon-180.png">
<link rel="preconnect" href="https://fonts.googleapis.com">
<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
<link href="https://fonts.googleapis.com/css2?family=Montserrat:wght@400;500;600;700;800&display=swap" rel="stylesheet">
<style>
:root{
  --bg:#F3F4F6; --bg2:#FFFFFF; --card:#FFFFFF; --ink:#0B0B0C; --ink2:#3A3A3F; --muted:#6B6B72; --line:rgba(11,11,12,.10);
  --pill:rgba(255,255,255,.75); --pill-b:rgba(11,11,12,.08); --btn:#0B0B0C; --btn-ink:#FFFFFF;
  --accent:linear-gradient(90deg,#0B0B0C,#5A5A62); --floor:rgba(11,11,12,.22); --glass:rgba(255,255,255,.55);
  --glass-edge:rgba(120,125,140,.35); --wave:rgba(11,11,12,.07); --shadow:0 30px 60px -40px rgba(11,11,12,.35);
  --nav:rgba(243,244,246,.78);
  --dock-bg:rgba(255,255,255,.52); --dock-edge:rgba(255,255,255,.65); --dock-spec:rgba(255,255,255,.95); --dock-low:rgba(11,11,12,.05);
  --dock-sheen:rgba(255,255,255,.55); --dock-rim:rgba(255,255,255,.95); --dock-shadow:0 12px 40px -14px rgba(11,11,12,.28),0 2px 6px -2px rgba(11,11,12,.08);
  --modal-bg:rgba(250,250,252,.74);
}
[data-theme="dark"],.dz{
  --bg:#0B0B0C; --bg2:#141416; --card:#121214; --ink:#F5F5F2; --ink2:#D2D2D6; --muted:#9A9AA0; --line:rgba(255,255,255,.10);
  --pill:rgba(255,255,255,.04); --pill-b:rgba(255,255,255,.12); --btn:transparent; --btn-ink:#F5F5F2;
  --accent:linear-gradient(90deg,#F5F5F2,#8E8E93); --floor:rgba(0,0,0,.7); --glass:rgba(255,255,255,.03);
  --glass-edge:rgba(255,255,255,.18); --wave:rgba(255,255,255,.06); --shadow:0 30px 60px -40px rgba(0,0,0,.9);
  --nav:rgba(11,11,12,.72);
  --dock-bg:rgba(24,24,27,.46); --dock-edge:rgba(255,255,255,.10); --dock-spec:rgba(255,255,255,.16); --dock-low:rgba(0,0,0,.35);
  --dock-sheen:rgba(255,255,255,.07); --dock-rim:rgba(255,255,255,.28); --dock-shadow:0 14px 44px -12px rgba(0,0,0,.65),0 2px 8px -2px rgba(0,0,0,.4);
  --modal-bg:rgba(22,22,25,.72);
}
*{box-sizing:border-box;margin:0;padding:0}
html{scroll-behavior:smooth}
html,body{background:var(--bg)}
body{font-family:Montserrat,system-ui,sans-serif;color:var(--ink);-webkit-font-smoothing:antialiased;overflow-x:hidden;transition:background .3s,color .3s}
a{color:inherit}
.wrap{position:relative;max-width:1280px;margin:0 auto;padding:0 40px}

/* NAV — dock flotante Liquid Glass */
html{scroll-padding-top:104px}
header{position:fixed;top:16px;left:0;right:0;z-index:60;padding:0 20px;pointer-events:none;transition:top .35s ease}
header.scrolled{top:10px}
.dock{pointer-events:auto;position:relative;max-width:1180px;margin:0 auto;display:flex;align-items:center;justify-content:space-between;gap:16px;
  padding:9px 9px 9px 24px;border-radius:999px;isolation:isolate;
  background:var(--dock-bg);border:1px solid var(--dock-edge);
  -webkit-backdrop-filter:blur(20px) saturate(180%);backdrop-filter:blur(20px) saturate(180%);
  box-shadow:inset 0 1px 0 var(--dock-spec),inset 0 -1px 0 var(--dock-low),var(--dock-shadow);
  transition:background .4s,border-color .4s,box-shadow .4s}
/* brillo especular del vidrio */
.dock:before{content:"";position:absolute;inset:0;border-radius:inherit;pointer-events:none;z-index:-1;
  background:linear-gradient(180deg,var(--dock-sheen) 0,transparent 55%),radial-gradient(60% 140% at 18% -30%,var(--dock-sheen),transparent 60%)}
.dock:after{content:"";position:absolute;inset:-1px;border-radius:inherit;padding:1px;pointer-events:none;
  background:linear-gradient(115deg,var(--dock-rim) 0,transparent 28%,transparent 72%,var(--dock-rim) 100%);
  -webkit-mask:linear-gradient(#000 0 0) content-box,linear-gradient(#000 0 0);-webkit-mask-composite:xor;mask-composite:exclude}
.brand img{height:48px;display:block}
.dock .brand img{height:36px}
.brand .dark,[data-theme="dark"] .brand .light{display:none}
[data-theme="dark"] .brand .dark{display:block}
.dz{color:var(--ink)}
.dz .brand .light{display:none}
.dz .brand .dark{display:block}
.menu{display:flex;gap:4px;padding:4px;border-radius:999px;background:var(--pill);border:1px solid var(--pill-b)}
.menu a{font-size:14px;font-weight:500;color:var(--ink2);text-decoration:none;padding:9px 18px;border-radius:999px;transition:.25s;border:1px solid transparent}
.menu a.on{background:var(--ink);color:var(--bg)}
[data-theme="dark"] .menu a.on,.dz .menu a.on{background:transparent;border-color:var(--line);color:var(--ink)}
.menu a:hover{color:var(--ink)}
.right{display:flex;align-items:center;gap:12px}
.cta{font-size:14px;font-weight:600;text-decoration:none;color:var(--btn-ink);background:var(--btn);border:1px solid var(--ink);padding:12px 22px;border-radius:999px;display:inline-flex;gap:8px;align-items:center;transition:transform .2s}
.cta:hover,.btn:hover{transform:translateY(-2px)}
.toggle{width:42px;height:42px;border-radius:50%;border:1px solid var(--line);background:var(--pill);color:var(--ink);cursor:pointer;display:grid;place-items:center;transition:transform .3s}
.toggle:hover{transform:rotate(-18deg)}
.toggle svg{width:18px;height:18px}
.toggle .sun,[data-theme="dark"] .toggle .moon{display:none}
[data-theme="dark"] .toggle .sun{display:block}
.dock .cta{padding:11px 20px}
.cta.solid{background:var(--ink);color:var(--bg);border-color:var(--ink)}

/* HERO */
.hero{position:relative;overflow:hidden;padding-top:96px;background:#050506;min-height:min(100vh,980px);display:flex;align-items:center}
.hero>.wrap{width:100%}
.hero .grid{grid-template-columns:minmax(0,620px);min-height:calc(min(100vh,980px) - 96px)}
.hero-video{position:absolute;inset:0;pointer-events:none;overflow:hidden}
.hero-video video{position:absolute;top:52%;right:-4%;width:68%;height:auto;aspect-ratio:16/9;transform:translateY(-50%);object-fit:cover;
  -webkit-mask-image:radial-gradient(ellipse 50% 50% at 50% 50%,#000 62%,transparent 100%);mask-image:radial-gradient(ellipse 50% 50% at 50% 50%,#000 62%,transparent 100%)}
.hero-video:after{content:"";position:absolute;inset:0;
  background:linear-gradient(90deg,#050506 30%,rgba(5,5,6,.6) 44%,rgba(5,5,6,0) 58%),
             linear-gradient(0deg,#050506 0,rgba(5,5,6,0) 18%)}
.waves{position:absolute;inset:0;width:100%;height:100%;pointer-events:none}
.waves path{fill:none;stroke:var(--wave);stroke-width:1}
.grid{display:grid;grid-template-columns:1fr 1.05fr;align-items:center;gap:20px;padding:40px 0 90px}
.grid>*{min-width:0}
.eyebrow{display:flex;align-items:center;gap:14px;font-size:12px;font-weight:600;letter-spacing:.28em;color:var(--ink2);text-transform:uppercase}
.eyebrow:before{content:"";width:34px;height:1.5px;background:var(--ink)}
h1{font-size:clamp(38px,4.6vw,64px);line-height:1.04;font-weight:800;letter-spacing:-.025em;margin:22px 0}
.grad{background:var(--accent);-webkit-background-clip:text;background-clip:text;color:transparent}
.lead{font-size:18px;line-height:1.6;color:var(--muted);max-width:520px}
.actions{display:flex;gap:26px;align-items:center;margin:36px 0 56px;flex-wrap:wrap}
.btn{font-size:15px;font-weight:600;text-decoration:none;padding:16px 28px;border-radius:999px;display:inline-flex;align-items:center;gap:10px;
  color:var(--btn-ink);background:var(--btn);border:1px solid var(--ink);cursor:pointer;font-family:inherit;transition:transform .2s}
.play{display:inline-flex;align-items:center;gap:12px;font-size:15px;font-weight:600;color:var(--ink);text-decoration:none}
.play i{width:44px;height:44px;border-radius:50%;border:1.5px solid var(--ink);display:grid;place-items:center}
.play i:after{content:"";border-left:11px solid var(--ink);border-top:7px solid transparent;border-bottom:7px solid transparent;margin-left:3px}
.stats{display:flex;align-items:center}
.stat{padding:0 34px;border-left:1px solid var(--line)}
.stat:first-child{padding-left:0;border-left:0}
.stat b{display:block;font-size:28px;font-weight:700;letter-spacing:-.02em}
.stat small{font-size:13px;color:var(--muted);white-space:nowrap}
.mini{display:flex;align-items:center;gap:16px;padding-left:34px;border-left:1px solid var(--line)}
.mini svg{width:34px;height:34px;stroke:var(--ink);fill:none;stroke-width:1.4;flex:none}
.mini p{font-size:13px;line-height:1.45;color:var(--ink2);max-width:170px}

/* DEVICES */
.stage{position:relative;height:560px;perspective:1800px}
.arc{position:absolute;width:520px;height:520px;left:-10px;top:40px;border-radius:50%;
  background:radial-gradient(circle at 30% 30%,var(--glass),transparent 60%);
  border:1px solid var(--glass-edge);box-shadow:inset 0 0 60px var(--glass-edge);
  -webkit-mask:linear-gradient(180deg,#000 52%,transparent 52%);mask:linear-gradient(180deg,#000 52%,transparent 52%);transform:rotate(-14deg)}
.arc:after{content:"";position:absolute;inset:26px;border-radius:50%;border:1px solid var(--glass-edge);opacity:.6}
.floor{position:absolute;left:12%;right:2%;bottom:60px;height:60px;border-radius:50%;background:var(--floor);filter:blur(28px)}
.laptop{position:absolute;left:4%;top:70px;width:520px;transform:rotateY(-24deg) rotateX(6deg)}
.lid{position:relative;width:100%;aspect-ratio:16/10.4;border-radius:22px 22px 8px 8px;padding:14px 14px 22px;
  background:linear-gradient(145deg,#2b2c30,#0c0c0d 60%);box-shadow:0 0 0 2px #9a9ca3,0 0 0 3px #d8dadf,0 40px 80px -30px rgba(0,0,0,.6)}
.lid:before{content:"";position:absolute;top:6px;left:50%;width:7px;height:7px;margin-left:-3px;border-radius:50%;background:#1e1f22}
.screen{position:relative;height:100%;border-radius:8px;overflow:hidden;background:radial-gradient(120% 90% at 50% 20%,#1a1b1f,#060607 70%);display:grid;place-items:center}
.screen svg{position:absolute;inset:0;width:100%;height:100%}
.screen svg path{fill:none;stroke:rgba(255,255,255,.12);stroke-width:1}
.screen img{position:relative;width:46%}
.glare{position:absolute;inset:0;background:linear-gradient(115deg,rgba(255,255,255,.10),transparent 38%);pointer-events:none}
.base{position:relative;margin:-2px auto 0;width:112%;left:-6%;height:20px;border-radius:2px 2px 14px 14px;
  background:linear-gradient(180deg,#e9eaee,#a9abb2 55%,#7c7e85);box-shadow:0 14px 26px -10px rgba(0,0,0,.45)}
.base:before{content:"";position:absolute;left:50%;top:0;width:110px;height:7px;margin-left:-55px;border-radius:0 0 8px 8px;background:linear-gradient(180deg,#a6a8ae,#c9cbd0)}
.phone{position:absolute;right:-2%;top:215px;width:136px;aspect-ratio:9/19.3;border-radius:30px;padding:7px;
  background:#0d0d0e;box-shadow:0 0 0 2px #8f9198,0 0 0 3px #d5d7dc,0 40px 60px -24px rgba(0,0,0,.6);transform:rotateY(-18deg) rotateX(4deg)}
.phone .scr{height:100%;border-radius:24px;background:radial-gradient(100% 70% at 50% 30%,#1b1c20,#050506 70%);display:grid;place-items:center;position:relative;overflow:hidden}
.phone .scr:before{content:"";position:absolute;top:9px;left:50%;width:46px;height:14px;margin-left:-23px;border-radius:10px;background:#000}
.phone img{width:52%}
.stand{position:absolute;right:calc(-2% + 20px);top:478px;width:96px;height:56px;border-radius:4px;
  background:linear-gradient(180deg,rgba(200,205,215,.35),rgba(200,205,215,.08));border:1px solid var(--glass-edge);transform:skewX(-8deg)}

/* STRIP */
.strip{border-top:1px solid var(--line);border-bottom:1px solid var(--line);overflow:hidden;white-space:nowrap;padding:22px 0}
.strip .track{display:inline-flex;gap:48px;animation:slide 40s linear infinite;font-size:14px;font-weight:600;letter-spacing:.22em;color:var(--muted);text-transform:uppercase}
.strip .track span:nth-child(even){color:var(--line);font-weight:400;letter-spacing:0}
@keyframes slide{to{transform:translateX(-50%)}}

/* SECTIONS */
section.block{padding:130px 0}
.head{display:flex;justify-content:space-between;align-items:end;gap:40px;margin-bottom:64px}
h2{font-size:clamp(32px,3.6vw,50px);line-height:1.08;font-weight:800;letter-spacing:-.02em;margin-top:20px;max-width:640px}
.head p{color:var(--muted);font-size:17px;line-height:1.6;max-width:420px}

/* services */
.cards{display:grid;grid-template-columns:repeat(3,1fr);gap:24px}
.card{background:var(--card);border:1px solid var(--line);border-radius:24px;padding:40px 36px;box-shadow:var(--shadow);transition:transform .3s,border-color .3s;display:flex;flex-direction:column}
.card:hover{transform:translateY(-6px);border-color:var(--glass-edge)}
.card .ic{width:58px;height:58px;border-radius:16px;border:1px solid var(--line);display:grid;place-items:center;margin-bottom:34px}
.card .ic svg{width:28px;height:28px;stroke:var(--ink);fill:none;stroke-width:1.4}
.card h3{font-size:22px;font-weight:700;letter-spacing:-.01em;margin-bottom:14px}
.card p{color:var(--muted);line-height:1.65;font-size:15px;margin-bottom:26px}
.card ul{list-style:none;border-top:1px solid var(--line);padding-top:22px;margin-top:auto}
.card li{font-size:14px;color:var(--ink2);padding:7px 0;display:flex;gap:12px;align-items:center}
.card li:before{content:"";width:14px;height:1px;background:var(--ink)}

/* process */
.process{background:var(--bg2)}
.steps{display:grid;grid-template-columns:repeat(4,1fr);border-top:1px solid var(--line)}
.step{padding:40px 30px 10px 0;border-right:1px solid var(--line);margin-right:30px}
.step:last-child{border-right:0;margin-right:0}
.step .n{font-size:13px;font-weight:600;letter-spacing:.2em;color:var(--muted)}
.step h3{font-size:20px;font-weight:700;margin:18px 0 12px}
.step p{font-size:15px;line-height:1.65;color:var(--muted)}

/* projects */
.projects{display:grid;grid-template-columns:repeat(2,1fr);gap:24px}
.proj{border-radius:24px;overflow:hidden;border:1px solid var(--line);background:var(--card);box-shadow:var(--shadow);text-decoration:none;transition:transform .3s}
.proj:hover{transform:translateY(-6px)}
.cover{aspect-ratio:16/10;position:relative;overflow:hidden;background:radial-gradient(120% 100% at 30% 20%,#232327,#09090a 70%);display:grid;place-items:center}
.cover svg.lines{position:absolute;inset:0;width:100%;height:100%}
.cover svg.lines path{fill:none;stroke:rgba(255,255,255,.08)}
.meta{display:flex;justify-content:space-between;align-items:center;padding:26px 30px}
.meta h3{font-size:19px;font-weight:700}
.meta span{font-size:12px;letter-spacing:.18em;color:var(--muted);text-transform:uppercase}
.meta i{width:42px;height:42px;border-radius:50%;border:1px solid var(--line);display:grid;place-items:center;font-style:normal;flex:none}
/* cover mini-mockups */
.cv-brand{display:flex;gap:18px;align-items:center}
.cv-brand .tile{width:120px;height:150px;border-radius:12px;background:#f5f5f2;display:grid;place-items:center;box-shadow:0 30px 50px -20px #000}
.cv-brand .tile.d{background:#0b0b0c;border:1px solid rgba(255,255,255,.15)}
.cv-brand img{width:62%}
.cv-browser{width:72%;border-radius:12px;overflow:hidden;background:#0b0b0c;border:1px solid rgba(255,255,255,.14);box-shadow:0 40px 60px -25px #000}
.cv-browser .bar{height:26px;background:#18181b;display:flex;gap:6px;align-items:center;padding:0 12px}
.cv-browser .bar b{width:8px;height:8px;border-radius:50%;background:#3a3a3f}
.cv-browser .bd{padding:26px 28px}
.sk{height:10px;border-radius:6px;background:rgba(255,255,255,.14);margin-bottom:10px}
.sk.t{height:18px;width:70%;background:rgba(255,255,255,.85)}
.sk.w60{width:60%}.sk.w40{width:40%}
.sk.btn{width:90px;height:22px;border-radius:12px;background:#f5f5f2;margin-top:18px}
.cv-feed{display:grid;grid-template-columns:repeat(3,70px);gap:8px;padding:16px;border-radius:26px;background:#0b0b0c;border:1px solid rgba(255,255,255,.14);box-shadow:0 40px 60px -25px #000}
.cv-feed div{width:70px;height:70px;border-radius:6px;background:linear-gradient(135deg,#2a2a2f,#121214);display:grid;place-items:center}
.cv-feed div:nth-child(3n+2){background:#f5f5f2}
.cv-feed img{width:50%}
.cv-shop{display:flex;gap:16px}
.cv-shop .p{width:110px;border-radius:12px;background:#0b0b0c;border:1px solid rgba(255,255,255,.14);padding:10px;box-shadow:0 30px 50px -22px #000}
.cv-shop .p .im{height:90px;border-radius:8px;background:linear-gradient(160deg,#2c2c31,#111113);margin-bottom:10px}
.note{font-size:13px;color:var(--muted);margin-top:26px}

/* about */
.about{display:grid;grid-template-columns:1fr 1fr;gap:80px;align-items:center}
.about .visual{aspect-ratio:1/1;border-radius:28px;border:1px solid var(--line);background:radial-gradient(80% 80% at 50% 40%,var(--bg2),var(--bg));display:grid;place-items:center;position:relative;overflow:hidden}
.about .visual img{width:40%}
.about .visual .dark,[data-theme="dark"] .about .visual .light{display:none}
[data-theme="dark"] .about .visual .dark{display:block}
.about p.txt{font-size:17px;line-height:1.75;color:var(--muted);margin:26px 0 36px}
.values{display:grid;gap:0;border-top:1px solid var(--line)}
.values>div{display:flex;gap:24px;padding:22px 0;border-bottom:1px solid var(--line)}
.values b{font-size:13px;color:var(--muted);letter-spacing:.15em;width:34px;flex:none;padding-top:3px}
.values h4{font-size:17px;font-weight:700;margin-bottom:6px}
.values span{font-size:15px;color:var(--muted);line-height:1.55}

/* CTA band */
.band{border-radius:32px;padding:90px 60px;text-align:center;position:relative;overflow:hidden;
  background:#0B0B0C;color:#F5F5F2;border:1px solid var(--line)}
.band svg{position:absolute;inset:0;width:100%;height:100%}
.band svg path{fill:none;stroke:rgba(255,255,255,.06)}
.band h2{margin:20px auto 18px;max-width:760px;color:#F5F5F2}
.band p{color:#9A9AA0;font-size:17px;margin-bottom:38px}
.band .eyebrow{justify-content:center;color:#D2D2D6}
.band .eyebrow:before{background:#F5F5F2}
.band .btn{background:#F5F5F2;color:#0B0B0C;border-color:#F5F5F2;position:relative}

/* contact */
.contact{display:grid;grid-template-columns:.9fr 1.1fr;gap:80px}
.info{display:grid;gap:0;margin-top:40px;border-top:1px solid var(--line)}
.info a,.info div{display:flex;justify-content:space-between;padding:22px 0;border-bottom:1px solid var(--line);text-decoration:none;font-size:16px}
.info small{color:var(--muted);font-size:13px;letter-spacing:.15em;text-transform:uppercase}
form{background:var(--card);border:1px solid var(--line);border-radius:28px;padding:44px;box-shadow:var(--shadow);display:grid;grid-template-columns:1fr 1fr;gap:20px}
form .full{grid-column:1/-1}
label{display:block;font-size:12px;font-weight:600;letter-spacing:.15em;text-transform:uppercase;color:var(--ink2);margin-bottom:10px}
input,select,textarea{width:100%;font:inherit;font-size:15px;color:var(--ink);background:transparent;border:0;border-bottom:1px solid var(--line);padding:12px 0;outline:none;border-radius:0}
select{appearance:none;cursor:pointer}
select option{color:#0B0B0C}
textarea{resize:vertical;min-height:110px}
input:focus,select:focus,textarea:focus{border-color:var(--ink)}
form{align-self:start;align-content:start}
form .btn{justify-self:start;margin-top:10px}
.ok{display:none;font-size:14px;color:var(--ink2)}

/* footer */
footer{border-top:1px solid var(--line);padding:70px 0 40px;margin-top:130px}
.fgrid{display:grid;grid-template-columns:1.4fr 1fr 1fr 1fr;gap:40px}
.fgrid p{color:var(--muted);font-size:14px;line-height:1.7;margin-top:22px;max-width:320px}
.fgrid h5{font-size:12px;letter-spacing:.2em;text-transform:uppercase;color:var(--muted);font-weight:600;margin-bottom:20px}
.fgrid a{display:block;text-decoration:none;font-size:14px;color:var(--ink2);padding:6px 0}
.fgrid a:hover{color:var(--ink)}
.fnote{display:block;font-size:13px;line-height:1.7;color:var(--muted);margin-top:12px}
.info a span,.info div span{text-align:right}
.social{display:flex;gap:10px;margin-top:24px}
.social a{width:42px;height:42px;border-radius:50%;border:1px solid var(--line);display:grid;place-items:center;padding:0}
.social svg{width:17px;height:17px;fill:none;stroke:var(--ink);stroke-width:1.5}
.legal{display:flex;justify-content:space-between;border-top:1px solid var(--line);margin-top:56px;padding-top:28px;font-size:13px;color:var(--muted)}

.social a{transition:transform .25s,background .25s,border-color .25s}
.social a:hover{transform:translateY(-2px);border-color:var(--ink)}
.info small{display:inline-flex;align-items:center;gap:10px}
.info small svg{width:15px;height:15px;fill:none;stroke:currentColor;stroke-width:1.6;flex:none}
.info a:hover span{color:var(--ink)}
.info span{color:var(--ink2);transition:color .2s}

/* CONFIANZA — caso destacado */
.trust{background:var(--bg2)}
.case{display:grid;grid-template-columns:1.25fr 1fr;border-radius:32px;overflow:hidden;background:var(--card);border:1px solid var(--line);box-shadow:var(--shadow)}
.case-shot{position:relative;display:flex;align-items:center;justify-content:center;overflow:hidden;padding:44px 40px;
  background:radial-gradient(70% 60% at 50% 62%,rgba(214,96,38,.20),transparent 70%),radial-gradient(120% 100% at 30% 0%,#1c1c1f,#070708 70%)}
.case-shot .frame{position:relative;width:100%;border-radius:14px;overflow:hidden;border:1px solid rgba(255,255,255,.14);box-shadow:0 50px 90px -30px #000,0 0 0 6px rgba(255,255,255,.03);background:#000}
.case-shot .bar{height:30px;display:flex;align-items:center;gap:7px;padding:0 14px;background:#161618;border-bottom:1px solid rgba(255,255,255,.08)}
.case-shot .bar b{width:9px;height:9px;border-radius:50%;background:#3a3a3f}
.case-shot .bar em{min-width:0;white-space:nowrap;overflow:hidden;text-overflow:ellipsis;margin-left:14px;font-style:normal;font-size:11px;letter-spacing:.02em;color:#8E8E93;background:#0e0e10;border-radius:6px;padding:4px 12px}
.case-shot img{display:block;width:100%;height:auto;transition:transform 1.2s cubic-bezier(.2,.7,.2,1)}
.case:hover .case-shot img{transform:scale(1.03)}
.case-body{padding:52px 48px;display:flex;flex-direction:column}
.live{display:inline-flex;align-items:center;gap:10px;font-size:11px;font-weight:600;letter-spacing:.22em;text-transform:uppercase;color:var(--ink2)}
.live i{width:8px;height:8px;border-radius:50%;background:#22c55e;box-shadow:0 0 0 0 rgba(34,197,94,.5);animation:pulse 2.2s infinite}
@keyframes pulse{70%{box-shadow:0 0 0 9px rgba(34,197,94,0)}100%{box-shadow:0 0 0 0 rgba(34,197,94,0)}}
.case-body .client{margin-top:26px;font-size:13px;font-weight:600;letter-spacing:.16em;text-transform:uppercase;color:var(--muted)}
.case-body h3{font-size:clamp(24px,2.2vw,30px);line-height:1.18;font-weight:800;letter-spacing:-.015em;margin:12px 0 18px}
.case-body p{color:var(--muted);font-size:15px;line-height:1.7}
.deliv{list-style:none;margin:28px 0 34px;border-top:1px solid var(--line)}
.deliv li{display:flex;gap:14px;align-items:center;font-size:14px;color:var(--ink2);padding:13px 0;border-bottom:1px solid var(--line)}
.deliv li:before{content:"";width:14px;height:1px;background:var(--ink);flex:none}
.case-body .btn{align-self:flex-start;margin-top:auto}
.sectors{display:grid;grid-template-columns:repeat(3,1fr);gap:24px;margin-top:24px}
.sector{border:1px solid var(--line);border-radius:24px;padding:30px 30px 28px;background:var(--card);display:flex;gap:18px;align-items:flex-start}
.sector .ic{width:46px;height:46px;border-radius:14px;border:1px solid var(--line);display:grid;place-items:center;flex:none}
.sector svg{width:22px;height:22px;stroke:var(--ink);fill:none;stroke-width:1.4}
.sector h4{font-size:16px;font-weight:700;margin-bottom:6px}
.sector p{font-size:14px;line-height:1.55;color:var(--muted)}

/* MODAL DE COTIZACIÓN — Liquid Glass */
html.locked{overflow:hidden}
dialog.quote{position:fixed;inset:0;margin:auto;width:min(640px,calc(100% - 32px));max-height:min(92vh,860px);overflow:auto;overscroll-behavior:contain;
  padding:0;border-radius:32px;color:var(--ink);font-family:inherit;
  background:var(--modal-bg);border:1px solid var(--dock-edge);
  -webkit-backdrop-filter:blur(28px) saturate(180%);backdrop-filter:blur(28px) saturate(180%);
  box-shadow:inset 0 1px 0 var(--dock-spec),0 40px 120px -30px rgba(0,0,0,.55)}
dialog.quote::backdrop{background:rgba(5,5,6,.38);-webkit-backdrop-filter:blur(6px);backdrop-filter:blur(6px)}
dialog.quote[open]{animation:qin .45s cubic-bezier(.2,.8,.2,1)}
dialog.quote[open]::backdrop{animation:fade .35s ease}
@keyframes qin{from{opacity:0;transform:translateY(18px) scale(.98)}}
@keyframes fade{from{opacity:0}}
form.q-in{padding:34px 38px 28px;display:grid;grid-template-columns:minmax(0,1fr);gap:20px;background:none;border:0;border-radius:0;box-shadow:none}
.pills-wrap{border:0;padding:0;margin:0;min-width:0}
label.pill{display:inline-block;margin:0;font-size:inherit;font-weight:inherit;letter-spacing:0;text-transform:none;color:inherit}
.q-head{display:flex;justify-content:space-between;align-items:flex-start;gap:20px}
.q-head h3{font-size:28px;font-weight:800;letter-spacing:-.02em;line-height:1.1;margin-top:12px}
.q-head p{font-size:14px;color:var(--muted);line-height:1.6;margin-top:10px;max-width:420px}
.q-x{width:40px;height:40px;flex:none;border-radius:50%;border:1px solid var(--line);background:var(--pill);color:var(--ink);cursor:pointer;display:grid;place-items:center;font-size:20px;line-height:1;transition:transform .25s}
.q-x:hover{transform:rotate(90deg)}
.q-label{display:block;font-size:12px;font-weight:600;letter-spacing:.15em;text-transform:uppercase;color:var(--ink2);margin-bottom:12px}
.q-label em{font-style:normal;font-weight:500;letter-spacing:.05em;text-transform:none;color:var(--muted)}
.pills{display:flex;flex-wrap:wrap;gap:10px;border:0}
.pill{position:relative}
.pill input{position:absolute;opacity:0;width:1px;height:1px}
.pill span{display:inline-flex;align-items:center;gap:9px;padding:10px 16px;border-radius:999px;font-size:14px;font-weight:500;color:var(--ink2);
  background:var(--pill);border:1px solid var(--pill-b);cursor:pointer;transition:background .25s,color .25s,border-color .25s,transform .2s;user-select:none}
.pill span:before{content:"";width:14px;height:14px;border-radius:50%;border:1.5px solid currentColor;opacity:.5;transition:.25s;flex:none}
.pill:hover span{transform:translateY(-1px);border-color:var(--ink)}
.pill input:checked+span{background:var(--ink);color:var(--bg);border-color:var(--ink)}
.pill input:checked+span:before{opacity:1;background:currentColor;box-shadow:inset 0 0 0 3px var(--ink)}
.pill input:focus-visible+span{outline:2px solid var(--ink);outline-offset:2px}
.q-row{display:grid;grid-template-columns:1fr 1fr;gap:20px}
.q-field input,.q-field select,.q-field textarea{border-bottom-color:var(--line)}
.q-field textarea{min-height:76px}
.q-err{font-size:13px;color:#d4483b;margin:-8px 0}
.q-err:empty{display:none}
.q-foot{display:flex;align-items:center;justify-content:space-between;gap:18px;flex-wrap:wrap;padding-top:6px;border-top:1px solid var(--line)}
.q-foot small{font-size:12px;color:var(--muted);line-height:1.5;max-width:240px;padding-top:14px}
.q-foot .btn{margin-top:14px;padding:14px 24px;background:var(--ink);color:var(--bg);border-color:var(--ink)}
.q-foot .btn svg{width:18px;height:18px;fill:currentColor}

/* BOTÓN FLOTANTE WHATSAPP — inverso premium */
.wa-fab{position:fixed;right:24px;bottom:24px;z-index:55;width:56px;height:56px;border-radius:50%;display:grid;place-items:center;
  background:#0A0A0A;color:#FFFFFF;border:1px solid rgba(255,255,255,.14);
  box-shadow:0 14px 34px -10px rgba(0,0,0,.45),inset 0 1px 0 rgba(255,255,255,.12);
  transition:background .45s ease,color .45s ease,border-color .45s ease,transform .3s cubic-bezier(.2,.8,.2,1),box-shadow .3s}
.wa-fab svg{width:24px;height:24px;fill:currentColor}
.wa-fab:hover{transform:translateY(-3px) scale(1.04);box-shadow:0 20px 40px -12px rgba(0,0,0,.5),inset 0 1px 0 rgba(255,255,255,.12)}
[data-theme="dark"] .wa-fab{background:#F5F5F7;color:#0A0A0A;border-color:rgba(255,255,255,.6);box-shadow:0 14px 34px -10px rgba(0,0,0,.7),inset 0 1px 0 #fff}

/* reveal */
.rv{opacity:0;transform:translateY(24px);transition:opacity .8s ease,transform .8s ease}
.rv.in{opacity:1;transform:none}
@media (prefers-reduced-motion:reduce){.rv{opacity:1;transform:none}.strip .track{animation:none}html{scroll-behavior:auto}}
@media (max-width:1080px){
  .hero-video video{width:160%;right:-30%;top:40%;opacity:.5}
  .hero-video:after{background:linear-gradient(180deg,rgba(5,5,6,.55) 0,rgba(5,5,6,.3) 40%,#050506 100%)}
}

@media (max-width:1080px){
  .menu{display:none}
  .grid,.about,.contact{grid-template-columns:1fr}
  .stage{height:440px;transform:scale(.8);transform-origin:top center;margin-bottom:-80px}
  .mini{display:none}
  .cards{grid-template-columns:1fr}
  .steps{grid-template-columns:1fr 1fr}
  .step{border-right:0;margin-right:0;border-bottom:1px solid var(--line);padding-bottom:30px}
  .head{flex-direction:column;align-items:start}
  .about{gap:50px}
  .fgrid{grid-template-columns:1fr 1fr}
  .case{grid-template-columns:1fr}
  .case-shot{padding:32px 24px}
  .sectors{grid-template-columns:1fr}
}
@media (max-width:640px){
  .wrap{padding:0 18px}
  header{padding:0 12px;top:12px}
  .dock{padding:7px 7px 7px 16px;gap:10px}
  .dock .brand img{height:30px}
  .dock .cta{padding:10px 14px;font-size:13px}
  .cta .lg{display:none}
  .right{gap:8px}
  .toggle{width:38px;height:38px}
  .case-body{padding:34px 24px}
  .sector{padding:24px 22px}
  dialog.quote{width:100%;max-width:100%;max-height:92vh;margin:auto 0 0;border-radius:28px 28px 0 0;border-bottom:0}
  @keyframes qin{from{opacity:0;transform:translateY(40px)}}
  form.q-in{padding:28px 22px 26px;gap:22px}
  .q-head h3{font-size:24px}
  .q-row{grid-template-columns:1fr}
  .q-foot .btn{width:100%;justify-content:center}
  .wa-fab{right:16px;bottom:16px;width:52px;height:52px}
  h1{font-size:40px}
  .lead{font-size:16px}
  .actions{gap:18px;margin:28px 0 40px}
  .btn{padding:14px 22px}
  .stage{transform:none;height:300px;margin:10px 0 0;overflow:hidden}
  .arc{width:280px;height:280px;left:-20px;top:10px}
  .laptop{left:0;top:40px;width:270px}
  .lid{padding:8px 8px 12px;border-radius:14px 14px 6px 6px}
  .phone{right:4px;top:110px;width:80px;border-radius:18px;padding:4px}
  .phone .scr{border-radius:14px}
  .phone .scr:before{width:26px;height:8px;margin-left:-13px;top:6px}
  .stand{display:none}
  .floor{bottom:30px}
  .stats{flex-wrap:wrap;gap:16px}
  .stat{padding:0 18px}
  section.block{padding:90px 0}
  .head{margin-bottom:40px}
  .steps,.projects{grid-template-columns:1fr}
  .card{padding:32px 26px}
  .cv-brand .tile{width:84px;height:106px}
  .cv-feed{grid-template-columns:repeat(3,50px)}.cv-feed div{width:50px;height:50px}
  .cv-shop .p{width:80px}.cv-shop .p .im{height:64px}
  .band{padding:64px 24px;border-radius:24px}
  form{grid-template-columns:1fr;padding:30px 22px}
  .fgrid{grid-template-columns:1fr}
  .legal{flex-direction:column;gap:10px}
  footer{margin-top:90px}
}
</style>
</head>
<body>
<header id="top" class="dz">
  <nav class="dock" aria-label="Principal">
    <a class="brand" href="#inicio"><img class="light" src="assets/logo-negro.png" alt="JL Novus Studio"><img class="dark" src="assets/logo-blanco.png" alt="JL Novus Studio"></a>
    <div class="menu">
      <a class="on" href="#inicio">Inicio</a><a href="#servicios">Servicios</a><a href="#proyectos">Proyectos</a><a href="#nosotros">Nosotros</a><a href="#contacto">Contacto</a>
    </div>
    <div class="right">
      <button class="toggle" id="toggle" aria-label="Cambiar modo claro u oscuro">
        <svg class="moon" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="1.6"><path d="M21 12.8A9 9 0 1 1 11.2 3a7 7 0 0 0 9.8 9.8z"/></svg>
        <svg class="sun" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="1.6" stroke-linecap="round"><circle cx="12" cy="12" r="4.2"/><path d="M12 2.5v2M12 19.5v2M2.5 12h2M19.5 12h2M5.3 5.3l1.4 1.4M17.3 17.3l1.4 1.4M5.3 18.7l1.4-1.4M17.3 6.7l1.4-1.4"/></svg>
      </button>
      <a class="cta solid" href="https://wa.me/51938437193" target="_blank" rel="noopener noreferrer" data-quote>Cotiza<span class="lg"> tu proyecto</span> <span>↗</span></a>
    </div>
  </nav>
</header>

<section class="hero dz" id="inicio">
  <div class="hero-video" aria-hidden="true">
    <video id="heroVideo" autoplay muted loop playsinline preload="auto" poster="assets/novus-hero-poster.jpg">
      <source src="novus-hero-web.mp4" type="video/mp4">
    </video>
  </div>
  <div class="wrap">
    <div class="grid">
      <div>
        <div class="eyebrow">Estudio creativo digital</div>
        <h1>Diseñamos marcas que <span class="grad">venden</span> como líderes</h1>
        <p class="lead">Marketing digital, branding y desarrollo web para negocios que quieren proyectar una imagen premium y crecer con estrategia.</p>
        <div class="actions">
          <a class="btn" href="#servicios">Nuestros servicios <span>→</span></a>
          <a class="play" href="#proyectos"><i></i>Ver portafolio</a>
        </div>
        <div class="stats">
          <div class="stat"><b>360°</b><small>Marketing integral</small></div>
          <div class="stat"><b>100%</b><small>Diseño a medida</small></div>
          <div class="mini">
            <svg viewBox="0 0 32 32"><path d="M16 4 29 10 16 16 3 10z"/><path d="M3 16l13 6 13-6"/><path d="M3 22l13 6 13-6"/></svg>
            <p>Branding, web y marketing en un solo estudio.</p>
          </div>
        </div>
      </div>
    </div>
  </div>
</section>

<div class="strip" aria-hidden="true"><div class="track" id="track"></div></div>

<!-- SERVICIOS -->
<section class="block" id="servicios">
  <div class="wrap">
    <div class="head rv">
      <div><div class="eyebrow">Servicios</div><h2>Todo lo que tu marca necesita para crecer</h2></div>
      <p>Unimos estrategia, diseño y tecnología para que tu negocio se vea profesional y atraiga a los clientes correctos.</p>
    </div>
    <div class="cards">
      <article class="card rv">
        <div class="ic"><svg viewBox="0 0 32 32"><rect x="4" y="6" width="24" height="16" rx="2"/><path d="M16 22v4M11 26h10"/></svg></div>
        <h3>Marketing Digital</h3>
        <p>Estrategias y campañas que convierten seguidores en clientes, con contenido que refleja la calidad de tu marca.</p>
        <ul><li>Gestión de redes sociales</li><li>Publicidad en Meta y Google</li><li>Contenido y fotografía</li><li>Reportes de resultados</li></ul>
      </article>
      <article class="card rv">
        <div class="ic"><svg viewBox="0 0 32 32"><path d="M16 4 29 10 16 16 3 10z"/><path d="M3 16l13 6 13-6"/><path d="M3 22l13 6 13-6"/></svg></div>
        <h3>Branding</h3>
        <p>Identidades visuales sólidas y memorables que transmiten confianza desde el primer vistazo.</p>
        <ul><li>Logotipo e identidad visual</li><li>Manual de marca</li><li>Papelería y aplicaciones</li><li>Kit para redes sociales</li></ul>
      </article>
      <article class="card rv">
        <div class="ic"><svg viewBox="0 0 32 32"><path d="M11 9 4 16l7 7M21 9l7 7-7 7M18 6l-4 20"/></svg></div>
        <h3>Desarrollo Web</h3>
        <p>Sitios rápidos, elegantes y optimizados para celular, pensados para vender y posicionarse en Google.</p>
        <ul><li>Páginas web corporativas</li><li>Landing pages</li><li>Tiendas online</li><li>SEO y mantenimiento</li></ul>
      </article>
    </div>
  </div>
</section>

<!-- PROCESO -->
<section class="block process" id="proceso">
  <div class="wrap">
    <div class="head rv">
      <div><div class="eyebrow">Proceso</div><h2>Un método claro, de la idea al resultado</h2></div>
      <p>Trabajamos por etapas para que siempre sepas en qué punto está tu proyecto.</p>
    </div>
    <div class="steps">
      <div class="step rv"><div class="n">01</div><h3>Descubrimiento</h3><p>Conocemos tu negocio, tu público y tus objetivos.</p></div>
      <div class="step rv"><div class="n">02</div><h3>Estrategia</h3><p>Definimos el camino: mensaje, estilo y canales.</p></div>
      <div class="step rv"><div class="n">03</div><h3>Diseño y desarrollo</h3><p>Creamos tu marca, tu web o tus campañas con atención al detalle.</p></div>
      <div class="step rv"><div class="n">04</div><h3>Lanzamiento</h3><p>Publicamos, medimos y optimizamos para que sigas creciendo.</p></div>
    </div>
  </div>
</section>

<!-- PROYECTOS -->
<section class="block" id="proyectos">
  <div class="wrap">
    <div class="head rv">
      <div><div class="eyebrow">Proyectos</div><h2>Trabajo con detalle en cada pieza</h2></div>
      <p>Una muestra de lo que creamos para nuestros clientes.</p>
    </div>
    <div class="projects">
      <a class="proj rv" href="#contacto">
        <div class="cover"><svg class="lines" viewBox="0 0 400 250" preserveAspectRatio="none"></svg>
          <div class="cv-brand"><div class="tile"><img src="assets/icono-negro.png" alt=""></div><div class="tile d"><img src="assets/icono-blanco.png" alt=""></div></div></div>
        <div class="meta"><div><span>Branding</span><h3>Identidad de marca</h3></div><i>↗</i></div>
      </a>
      <a class="proj rv" href="#contacto">
        <div class="cover"><svg class="lines" viewBox="0 0 400 250" preserveAspectRatio="none"></svg>
          <div class="cv-browser"><div class="bar"><b></b><b></b><b></b></div><div class="bd"><div class="sk t"></div><div class="sk w60"></div><div class="sk w40"></div><div class="sk btn"></div></div></div></div>
        <div class="meta"><div><span>Desarrollo web</span><h3>Sitio web corporativo</h3></div><i>↗</i></div>
      </a>
      <a class="proj rv" href="#contacto">
        <div class="cover"><svg class="lines" viewBox="0 0 400 250" preserveAspectRatio="none"></svg>
          <div class="cv-feed"><div></div><div><img src="assets/icono-negro.png" alt=""></div><div></div><div><img src="assets/icono-blanco.png" alt=""></div><div></div><div></div></div></div>
        <div class="meta"><div><span>Marketing digital</span><h3>Campaña en redes</h3></div><i>↗</i></div>
      </a>
      <a class="proj rv" href="#contacto">
        <div class="cover"><svg class="lines" viewBox="0 0 400 250" preserveAspectRatio="none"></svg>
          <div class="cv-shop"><div class="p"><div class="im"></div><div class="sk w60"></div><div class="sk w40"></div></div><div class="p"><div class="im"></div><div class="sk w60"></div><div class="sk w40"></div></div><div class="p"><div class="im"></div><div class="sk w60"></div><div class="sk w40"></div></div></div></div>
        <div class="meta"><div><span>E-commerce</span><h3>Tienda online</h3></div><i>↗</i></div>
      </a>
    </div>
  </div>
</section>

<!-- NOSOTROS -->
<section class="block process" id="nosotros">
  <div class="wrap about">
    <div class="visual rv"><img class="light" src="assets/icono-negro.png" alt="Novus Studio"><img class="dark" src="assets/icono-blanco.png" alt="Novus Studio"></div>
    <div class="rv">
      <div class="eyebrow">Nosotros</div>
      <h2>Un estudio pequeño, con estándares de marca grande</h2>
      <p class="txt">En Novus Studio creemos que una marca bien construida abre puertas. Por eso cuidamos cada detalle: desde la estrategia hasta el último píxel, para que tu negocio se vea y se sienta premium.</p>
      <div class="values">
        <div><b>01</b><div><h4>Estrategia primero</h4><span>Cada decisión de diseño responde a un objetivo de negocio.</span></div></div>
        <div><b>02</b><div><h4>Diseño con intención</h4><span>Limpio, elegante y coherente en todos tus canales.</span></div></div>
        <div><b>03</b><div><h4>Trato cercano</h4><span>Comunicación directa y acompañamiento en todo el proceso.</span></div></div>
      </div>
    </div>
  </div>
</section>

<!-- CONFIANZA -->
<section class="block" id="clientes">
  <div class="wrap">
    <div class="head rv">
      <div><div class="eyebrow">Confianza</div><h2>Marcas y proyectos que confían en nosotros</h2></div>
      <p>Negocios reales que ya venden con una presencia digital a la altura de su calidad.</p>
    </div>
    <article class="case rv">
      <a class="case-shot" href="https://polleria-donde-hernan.github.io/" target="_blank" rel="noopener noreferrer" aria-label="Abrir la web de Pollería &amp; Parrillas Donde Hernan">
        <div class="frame">
          <div class="bar"><b></b><b></b><b></b><em>polleria-donde-hernan.github.io</em></div>
          <img src="assets/caso-donde-hernan.jpg" alt="Página de inicio de la web de Pollería &amp; Parrillas Donde Hernan" loading="lazy" width="1280" height="723">
        </div>
      </a>
      <div class="case-body">
        <span class="live"><i></i>Caso real · En vivo</span>
        <div class="client">Pollería &amp; Parrillas “Donde Hernan” · Cajamarca</div>
        <h3>Experiencia Web Cinematográfica &amp; Carta Digital Interactiva con Pedidos por WhatsApp</h3>
        <p>Una web inmersiva que transmite el sabor de la brasa desde el primer segundo y convierte visitas en pedidos directos.</p>
        <ul class="deliv">
          <li>Web cinematográfica con animaciones al deslizar</li>
          <li>Carta digital interactiva por categorías</li>
          <li>Pedidos armados y enviados por WhatsApp</li>
          <li>Optimizada para celular</li>
        </ul>
        <a class="btn" href="https://polleria-donde-hernan.github.io/" target="_blank" rel="noopener noreferrer">Ver proyecto en vivo <span>↗</span></a>
      </div>
    </article>
    <div class="sectors">
      <div class="sector rv"><div class="ic"><svg viewBox="0 0 32 32"><path d="M8 4v10a3 3 0 0 0 6 0V4M11 4v24M22 28V4c-3 2-4 6-4 10h4"/></svg></div><div><h4>Gastronomía</h4><p>Restaurantes, pollerías y cafeterías con carta digital y pedidos.</p></div></div>
      <div class="sector rv"><div class="ic"><svg viewBox="0 0 32 32"><path d="M5 11h22l-2 15H7z"/><path d="M11 11V8a5 5 0 0 1 10 0v3"/></svg></div><div><h4>Comercio</h4><p>Tiendas y emprendimientos que venden mejor en redes y en web.</p></div></div>
      <div class="sector rv"><div class="ic"><svg viewBox="0 0 32 32"><rect x="4" y="10" width="24" height="16" rx="3"/><path d="M12 10V7a2 2 0 0 1 2-2h4a2 2 0 0 1 2 2v3M4 17h24"/></svg></div><div><h4>Servicios Profesionales</h4><p>Consultorios, estudios y profesionales que necesitan transmitir confianza.</p></div></div>
    </div>
  </div>
</section>

<!-- CTA -->
<section class="block" style="padding-bottom:0">
  <div class="wrap">
    <div class="band rv">
      <svg viewBox="0 0 1200 420" preserveAspectRatio="none" id="bandwaves" aria-hidden="true"></svg>
      <div class="eyebrow">Hablemos</div>
      <h2>¿Listo para que tu marca se vea premium?</h2>
      <p>Cuéntanos tu idea y te enviamos una propuesta a medida.</p>
      <a class="btn" href="https://wa.me/51938437193" target="_blank" rel="noopener noreferrer" data-quote>Cotiza tu proyecto <span>↗</span></a>
    </div>
  </div>
</section>

<!-- CONTACTO -->
<section class="block" id="contacto">
  <div class="wrap contact">
    <div class="rv">
      <div class="eyebrow">Contacto</div>
      <h2>Empecemos tu proyecto</h2>
      <p class="lead" style="margin-top:20px">Completa el formulario y te respondemos lo antes posible.</p>
      <div class="info">
        <a href="https://wa.me/51938437193" target="_blank" rel="noopener" id="waLink"><small>WhatsApp</small><span id="waText">+51 938 437 193</span></a>
        <a href="mailto:7.jhuliniolopez@gmail.com" id="mailLink"><small>Email</small><span id="mailText">7.jhuliniolopez@gmail.com</span></a>
        <a href="https://www.instagram.com/jlnovusstudio" target="_blank" rel="noopener noreferrer"><small><svg viewBox="0 0 24 24" aria-hidden="true"><rect x="3" y="3" width="18" height="18" rx="5"/><circle cx="12" cy="12" r="4"/><circle cx="17.3" cy="6.7" r=".9" fill="currentColor" stroke="none"/></svg>Instagram</small><span>@jlnovusstudio</span></a>
        <a href="https://www.facebook.com/share/1CuWkR24iw/" target="_blank" rel="noopener noreferrer"><small><svg viewBox="0 0 24 24" aria-hidden="true"><path d="M14.5 21v-7.5h2.6l.4-3.2h-3V8.4c0-.9.3-1.6 1.6-1.6h1.6V4c-.3 0-1.2-.1-2.3-.1-2.3 0-3.9 1.4-3.9 4v2.4H8.9v3.2h2.6V21"/></svg>Facebook</small><span>JL Novus Studio</span></a>
        <a href="https://www.linkedin.com/in/nilson-jhulinio-lopez-verastegui-5a494a190?utm_source=share_via&amp;utm_content=profile&amp;utm_medium=member_android" target="_blank" rel="noopener noreferrer"><small><svg viewBox="0 0 24 24" aria-hidden="true"><rect x="3" y="3" width="18" height="18" rx="4"/><path d="M7.8 10.5v6M7.8 7.6v.1M11.3 16.5v-6M11.3 13.4c0-1.8 1-2.9 2.5-2.9s2.4 1 2.4 2.9v3.1"/></svg>LinkedIn</small><span>Nilson Jhulinio Lopez Verastegui</span></a>
        <div><small>Ubicación</small><span>Cajamarca, Perú</span></div>
        <div><small>Horario</small><span>Lunes a sábado, 9:00 a. m. – 7:00 p. m.</span></div>
      </div>
    </div>
    <form class="rv" id="form">
      <div><label for="f-name">Nombre</label><input id="f-name" required></div>
      <div><label for="f-mail">Email</label><input id="f-mail" type="email" required></div>
      <div><label for="f-phone">WhatsApp</label><input id="f-phone" type="tel"></div>
      <div><label for="f-svc">Servicio</label><select id="f-svc"><option>Marketing Digital</option><option>Branding</option><option>Desarrollo Web</option><option>Paquete completo</option></select></div>
      <div class="full"><label for="f-msg">Cuéntanos tu proyecto</label><textarea id="f-msg"></textarea></div>
      <button class="btn full" type="submit">Enviar mensaje <span>→</span></button>
      <p class="ok full" id="ok"></p>
    </form>
  </div>
</section>

<footer>
  <div class="wrap">
    <div class="fgrid">
      <div>
        <a class="brand" href="#inicio"><img class="light" src="assets/logo-negro.png" alt="Novus Studio"><img class="dark" src="assets/logo-blanco.png" alt="Novus Studio"></a>
        <p>Estudio creativo digital. Marketing digital, branding y desarrollo web para marcas que quieren destacar.</p>
        <div class="social">
          <a href="https://www.instagram.com/jlnovusstudio" target="_blank" rel="noopener noreferrer" aria-label="Instagram @jlnovusstudio"><svg viewBox="0 0 24 24"><rect x="3" y="3" width="18" height="18" rx="5"/><circle cx="12" cy="12" r="4"/><circle cx="17.3" cy="6.7" r=".9" fill="currentColor" stroke="none"/></svg></a>
          <a href="https://www.facebook.com/share/1CuWkR24iw/" target="_blank" rel="noopener noreferrer" aria-label="Facebook JL Novus Studio"><svg viewBox="0 0 24 24"><path d="M14.5 21v-7.5h2.6l.4-3.2h-3V8.4c0-.9.3-1.6 1.6-1.6h1.6V4c-.3 0-1.2-.1-2.3-.1-2.3 0-3.9 1.4-3.9 4v2.4H8.9v3.2h2.6V21"/></svg></a>
          <a href="https://www.linkedin.com/in/nilson-jhulinio-lopez-verastegui-5a494a190?utm_source=share_via&amp;utm_content=profile&amp;utm_medium=member_android" target="_blank" rel="noopener noreferrer" aria-label="LinkedIn Nilson Jhulinio Lopez Verastegui"><svg viewBox="0 0 24 24"><rect x="3" y="3" width="18" height="18" rx="4"/><path d="M7.8 10.5v6M7.8 7.6v.1M11.3 16.5v-6M11.3 13.4c0-1.8 1-2.9 2.5-2.9s2.4 1 2.4 2.9v3.1"/></svg></a>
        </div>
      </div>
      <div><h5>Navegación</h5><a href="#inicio">Inicio</a><a href="#servicios">Servicios</a><a href="#proyectos">Proyectos</a><a href="#nosotros">Nosotros</a><a href="#contacto">Contacto</a></div>
      <div><h5>Servicios</h5><a href="#servicios">Marketing Digital</a><a href="#servicios">Branding</a><a href="#servicios">Desarrollo Web</a><a href="#servicios">Tiendas online</a></div>
      <div><h5>Contacto</h5><a href="https://wa.me/51938437193" target="_blank" rel="noopener noreferrer" data-quote>Cotiza tu proyecto ↗</a><a href="https://wa.me/51938437193" target="_blank" rel="noopener noreferrer" id="waFoot">+51 938 437 193</a><a href="mailto:7.jhuliniolopez@gmail.com" id="mailFoot">7.jhuliniolopez@gmail.com</a><a href="https://www.instagram.com/jlnovusstudio" target="_blank" rel="noopener noreferrer">Instagram · @jlnovusstudio</a><a href="https://www.facebook.com/share/1CuWkR24iw/" target="_blank" rel="noopener noreferrer">Facebook · JL Novus Studio</a><a href="https://www.linkedin.com/in/nilson-jhulinio-lopez-verastegui-5a494a190?utm_source=share_via&amp;utm_content=profile&amp;utm_medium=member_android" target="_blank" rel="noopener noreferrer">LinkedIn · Nilson Lopez V.</a><span class="fnote">Cajamarca, Perú<br>Lun – Sáb · 9:00 a. m. – 7:00 p. m.</span></div>
    </div>
    <div class="legal"><span>© <span id="yr">2026</span> Novus Studio. Todos los derechos reservados.</span><span>Estudio creativo digital</span></div>
  </div>
</footer>

<!-- MODAL DE COTIZACIÓN -->
<dialog class="quote" id="quote" aria-labelledby="q-title">
  <form class="q-in" id="qform" method="dialog" novalidate>
    <div class="q-head">
      <div>
        <div class="eyebrow">Cotización rápida</div>
        <h3 id="q-title">Arma tu proyecto en 1 minuto</h3>
        <p>Elige lo que necesitas y te enviamos una propuesta a medida por WhatsApp.</p>
      </div>
      <button type="button" class="q-x" id="qclose" aria-label="Cerrar">×</button>
    </div>
    <fieldset class="pills-wrap" style="border:0">
      <legend class="q-label">¿Qué necesitas? <em>(puedes elegir varios)</em></legend>
      <div class="pills">
        <label class="pill"><input type="checkbox" name="svc" value="Página Web / Landing Cinematográfica"><span>Página Web / Landing Cinematográfica</span></label>
        <label class="pill"><input type="checkbox" name="svc" value="Sistema Web / Software a Medida"><span>Sistema Web / Software a Medida</span></label>
        <label class="pill"><input type="checkbox" name="svc" value="Branding & Identidad Visual"><span>Branding &amp; Identidad Visual</span></label>
        <label class="pill"><input type="checkbox" name="svc" value="Marketing Digital & Contenido"><span>Marketing Digital &amp; Contenido</span></label>
        <label class="pill"><input type="checkbox" name="svc" value="Otro proyecto"><span>Otro proyecto</span></label>
      </div>
    </fieldset>
    <div class="q-row">
      <div class="q-field"><label class="q-label" for="q-name">Nombre o empresa</label><input id="q-name" autocomplete="organization" placeholder="Tu nombre o el de tu negocio"></div>
      <div class="q-field"><label class="q-label" for="q-budget">Presupuesto <em>(opcional)</em></label>
        <select id="q-budget">
          <option value="">Prefiero conversarlo</option>
          <option>Menos de S/ 1,000</option>
          <option>S/ 1,000 – S/ 3,000</option>
          <option>S/ 3,000 – S/ 6,000</option>
          <option>Más de S/ 6,000</option>
        </select>
      </div>
    </div>
    <div class="q-field"><label class="q-label" for="q-idea">Cuéntanos tu idea</label><textarea id="q-idea" placeholder="¿Qué te gustaría lograr? Fechas, referencias, lo que tengas en mente."></textarea></div>
    <p class="q-err" id="qerr" role="alert"></p>
    <div class="q-foot">
      <small>Se abrirá WhatsApp con tu mensaje listo. Solo tienes que enviarlo.</small>
      <button class="btn" type="submit"><svg viewBox="0 0 24 24" aria-hidden="true"><use href="#ico-wa"/></svg>Enviar cotización por WhatsApp</button>
    </div>
  </form>
</dialog>

<!-- BOTÓN FLOTANTE WHATSAPP -->
<a class="wa-fab" href="https://wa.me/51938437193" target="_blank" rel="noopener noreferrer" aria-label="Escríbenos por WhatsApp">
  <svg viewBox="0 0 24 24" aria-hidden="true"><use href="#ico-wa"/></svg>
</a>
<svg width="0" height="0" style="position:absolute" aria-hidden="true">
  <symbol id="ico-wa" viewBox="0 0 24 24"><path d="M17.47 14.38c-.3-.15-1.76-.87-2.03-.97-.27-.1-.47-.15-.67.15-.2.3-.77.97-.94 1.16-.17.2-.35.22-.64.07-.3-.15-1.26-.46-2.39-1.47-.88-.79-1.48-1.76-1.65-2.06-.17-.3-.02-.46.13-.6.13-.14.3-.35.44-.52.15-.18.2-.3.3-.5.1-.2.05-.37-.02-.52-.08-.15-.67-1.61-.92-2.2-.24-.58-.49-.5-.67-.51h-.57c-.2 0-.52.07-.79.37-.27.3-1.04 1.02-1.04 2.48s1.06 2.88 1.21 3.07c.15.2 2.1 3.2 5.08 4.49.71.31 1.26.49 1.7.63.71.22 1.36.19 1.87.12.57-.09 1.76-.72 2-1.42.25-.69.25-1.29.18-1.41-.08-.13-.28-.2-.57-.35m-5.42 7.4h-.01a9.87 9.87 0 0 1-5.03-1.38l-.36-.21-3.74.98 1-3.65-.24-.37a9.86 9.86 0 0 1-1.51-5.26c0-5.45 4.44-9.88 9.89-9.88 2.64 0 5.12 1.03 6.99 2.9a9.82 9.82 0 0 1 2.89 6.99c0 5.45-4.44 9.88-9.88 9.88m8.41-18.3A11.82 11.82 0 0 0 12.05 0C5.5 0 .16 5.34.16 11.89c0 2.1.55 4.14 1.59 5.95L.06 24l6.3-1.65a11.88 11.88 0 0 0 5.68 1.45h.01c6.55 0 11.89-5.34 11.89-11.89a11.82 11.82 0 0 0-3.48-8.41z"/></symbol>
</svg>

<script>
/* ====== CONFIGURA AQUÍ TUS DATOS ====== */
const CONFIG = {
  whatsapp: "51938437193",           // código de país + número, sin + ni espacios
  email: "7.jhuliniolopez@gmail.com"
};
/* ===================================== */

function waves(svg,w,h,n,y0,amp,spread,ph){
  if(!svg) return; let d='';
  for(let i=0;i<n;i++){
    const k=i/(n-1); let p='';
    for(let x=0;x<=w;x+=w/80){
      const u=x/w, y=y0+amp*Math.sin(u*Math.PI*1.6+ph)+spread*(k-.5)*Math.sin(u*Math.PI*1.1+ph*.7);
      p+=(x?'L':'M')+x.toFixed(1)+' '+y.toFixed(1);
    }
    d+='<path d="'+p+'"/>';
  }
  svg.innerHTML=d;
}
waves(document.getElementById('bgwaves'),1600,900,28,640,90,240,0.6);
waves(document.getElementById('scrwaves'),400,250,22,175,22,70,1.2);
waves(document.getElementById('bandwaves'),1200,420,26,300,50,200,0.4);
document.querySelectorAll('.cover svg.lines').forEach((s,i)=>waves(s,400,250,18,190,20,90,i*1.3));

// strip
const words=['Marketing Digital','Branding','Desarrollo Web','Estrategia','Contenido','Identidad Visual','Tiendas Online'];
let html=''; for(let r=0;r<2;r++) words.forEach(w=>html+='<span>'+w+'</span><span>/</span>');
document.getElementById('track').innerHTML=html;

// theme
const root=document.documentElement;
const q=new URLSearchParams(location.search).get('theme');
try{ const s=q||localStorage.getItem('novus-theme'); if(s) root.dataset.theme=s; }catch(e){ if(q) root.dataset.theme=q; }
document.getElementById('toggle').onclick=()=>{
  root.dataset.theme = root.dataset.theme==='dark'?'light':'dark';
  try{localStorage.setItem('novus-theme',root.dataset.theme)}catch(e){}
};

// sticky header + active link
const header=document.getElementById('top');
const links=[...document.querySelectorAll('.menu a')];
const secs=links.map(a=>document.querySelector(a.getAttribute('href')));
function onScroll(){
  header.classList.toggle('scrolled', scrollY>20);
  const heroBottom=document.getElementById('inicio').getBoundingClientRect().bottom;
  header.classList.toggle('dz', heroBottom>80);
  let cur=0; secs.forEach((s,i)=>{ if(s && s.getBoundingClientRect().top<200) cur=i; });
  links.forEach((a,i)=>a.classList.toggle('on',i===cur));
}
addEventListener('scroll',onScroll,{passive:true}); onScroll();

// reveal
const io=new IntersectionObserver(es=>es.forEach(e=>{ if(e.isIntersecting){ e.target.classList.add('in'); io.unobserve(e.target);} }),{threshold:.12});
document.querySelectorAll('.rv').forEach(el=>io.observe(el));
if(q) document.querySelectorAll('.rv').forEach(el=>el.classList.add('in')); // capturas

// hero video: respect reduced motion
const hv=document.getElementById('heroVideo');
if(hv && matchMedia('(prefers-reduced-motion: reduce)').matches){ hv.removeAttribute('autoplay'); hv.pause(); }

// contact data
document.getElementById('yr').textContent=new Date().getFullYear();
if(CONFIG.whatsapp){
  const wa='https://wa.me/'+CONFIG.whatsapp;
  ['waLink','waFoot'].forEach(id=>{const a=document.getElementById(id); a.href=wa; a.target='_blank'; a.rel='noopener';});
}
if(CONFIG.email){
  ['mailLink','mailFoot'].forEach(id=>document.getElementById(id).href='mailto:'+CONFIG.email);
  document.getElementById('mailText').textContent=CONFIG.email;
}
// ====== MODAL DE COTIZACIÓN ======
const dlg=document.getElementById('quote'), qform=document.getElementById('qform'), qerr=document.getElementById('qerr');
function openQuote(e){
  if(!dlg || typeof dlg.showModal!=='function') return;      // sin soporte: sigue el enlace a WhatsApp
  e.preventDefault(); qerr.textContent='';
  dlg.showModal(); root.classList.add('locked');
}
document.querySelectorAll('[data-quote]').forEach(a=>a.addEventListener('click',openQuote));
document.getElementById('qclose').onclick=()=>dlg.close();
dlg.addEventListener('close',()=>root.classList.remove('locked'));
dlg.addEventListener('click',e=>{ if(e.target===dlg) dlg.close(); });   // clic fuera del panel
qform.addEventListener('submit',e=>{
  e.preventDefault();
  const svcs=[...qform.querySelectorAll('input[name=svc]:checked')].map(i=>i.value);
  const name=document.getElementById('q-name').value.trim();
  const budget=document.getElementById('q-budget').value;
  const idea=document.getElementById('q-idea').value.trim();
  if(!svcs.length){ qerr.textContent='Elige al menos un servicio.'; return; }
  if(!name){ qerr.textContent='Escribe tu nombre o el de tu empresa.'; document.getElementById('q-name').focus(); return; }
  let msg='Hola JL Novus Studio, quiero cotizar un proyecto.\n\n';
  msg+='*Cliente:* '+name+'\n';
  msg+='*Servicios:*\n'+svcs.map(s=>'• '+s).join('\n')+'\n';
  msg+='*Presupuesto estimado:* '+(budget||'Por conversar')+'\n';
  if(idea) msg+='*Mi idea:* '+idea+'\n';
  window.open('https://wa.me/'+CONFIG.whatsapp+'?text='+encodeURIComponent(msg),'_blank','noopener');
  dlg.close();
});

document.getElementById('form').addEventListener('submit',e=>{
  e.preventDefault();
  const v=id=>document.getElementById(id).value.trim();
  const msg=`Hola Novus Studio, soy ${v('f-name')}.\nServicio: ${v('f-svc')}\nEmail: ${v('f-mail')}\nWhatsApp: ${v('f-phone')}\n\n${v('f-msg')}`;
  const ok=document.getElementById('ok'); ok.style.display='block';
  if(CONFIG.whatsapp){ window.open('https://wa.me/'+CONFIG.whatsapp+'?text='+encodeURIComponent(msg),'_blank'); ok.textContent='Abriendo WhatsApp…'; }
  else if(CONFIG.email){ location.href='mailto:'+CONFIG.email+'?subject='+encodeURIComponent('Nuevo proyecto - '+v('f-svc'))+'&body='+encodeURIComponent(msg); ok.textContent='Abriendo tu correo…'; }
  else { ok.textContent='Formulario de prueba: falta configurar el WhatsApp o el email en el código.'; }
});
</script>
</body>
</html>
