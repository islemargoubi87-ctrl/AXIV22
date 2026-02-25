<!DOCTYPE html>
<html lang="ar" dir="rtl">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>AXI GAMING — بوابة الألعاب التونسية</title>
<link href="https://fonts.googleapis.com/css2?family=Tajawal:wght@300;400;700;900&family=Bebas+Neue&display=swap" rel="stylesheet">
<style>
:root{--gold:#c9a84c;--gold2:#f0d080;--gold3:#a07828;--black:#080808;--black2:#0f0f0f;--black3:#181818;--black4:#222;--white:#fff;--muted:rgba(255,255,255,.45);--border:rgba(201,168,76,.15);--border2:rgba(201,168,76,.3);--r:14px;--r2:20px;}
*,*::before,*::after{margin:0;padding:0;box-sizing:border-box;}
html{scroll-behavior:smooth;background:var(--black);}
body{font-family:'Tajawal',sans-serif;background:var(--black);color:var(--white);overflow-x:hidden;}
button,input,textarea{font-family:'Tajawal',sans-serif;}
::-webkit-scrollbar{width:3px;}::-webkit-scrollbar-thumb{background:var(--gold3);border-radius:2px;}
body::after{content:'';position:fixed;inset:0;pointer-events:none;z-index:9999;opacity:.025;background-image:url("data:image/svg+xml,%3Csvg xmlns='http://www.w3.org/2000/svg' width='300' height='300'%3E%3Cfilter id='n'%3E%3CfeTurbulence type='fractalNoise' baseFrequency='.85' numOctaves='4' stitchTiles='stitch'/%3E%3C/filter%3E%3Crect width='300' height='300' filter='url(%23n)'/%3E%3C/svg%3E");}
.nav{position:fixed;top:0;left:0;right:0;z-index:1000;transition:all .3s;}
.nav.scrolled{background:rgba(8,8,8,.96);backdrop-filter:blur(20px);border-bottom:1px solid var(--border);}
.nav-inner{display:flex;align-items:center;justify-content:space-between;padding:18px 40px;max-width:1400px;margin:0 auto;}
.logo{display:flex;align-items:center;gap:10px;cursor:pointer;text-decoration:none;}
.logo-text{font-family:'Bebas Neue',sans-serif;font-size:1.9rem;letter-spacing:5px;color:var(--white);}
.logo-text span{color:var(--gold);}
.logo-dot{width:8px;height:8px;background:var(--gold);border-radius:50%;animation:pulse 2s infinite;}
@keyframes pulse{0%,100%{opacity:1;transform:scale(1)}50%{opacity:.4;transform:scale(.8)}}
.nav-links{display:flex;gap:6px;list-style:none;}
.nav-links a{color:var(--muted);font-size:.8rem;font-weight:700;letter-spacing:1.5px;text-transform:uppercase;text-decoration:none;padding:8px 14px;border-radius:8px;transition:all .25s;border:1px solid transparent;}
.nav-links a:hover,.nav-links a.on{color:var(--gold);border-color:var(--border);background:rgba(201,168,76,.06);}
.nav-end{display:flex;align-items:center;gap:8px;}
.nav-cart{position:relative;width:40px;height:40px;background:rgba(201,168,76,.08);border:1px solid var(--border);border-radius:10px;display:flex;align-items:center;justify-content:center;cursor:pointer;font-size:1rem;transition:all .25s;}
.nav-cart:hover{border-color:var(--gold);background:rgba(201,168,76,.14);}
.cart-badge{position:absolute;top:-6px;right:-6px;background:var(--gold);color:#000;font-size:.58rem;font-weight:900;min-width:17px;height:17px;border-radius:9px;display:none;align-items:center;justify-content:center;}
.nav-cta{background:linear-gradient(135deg,var(--gold),var(--gold2));color:#000;border:none;padding:9px 22px;border-radius:9px;font-weight:900;font-size:.82rem;cursor:pointer;letter-spacing:.5px;transition:all .3s;}
.nav-cta:hover{transform:translateY(-2px);box-shadow:0 6px 24px rgba(201,168,76,.4);}
.pg{display:none;}.pg.on{display:block;}
.hero{min-height:100vh;display:flex;align-items:center;justify-content:center;text-align:center;position:relative;overflow:hidden;padding:120px 24px 80px;}
.hero-bg{position:absolute;inset:0;z-index:0;}
.hero-bg-grad{position:absolute;inset:0;background:radial-gradient(ellipse 80% 70% at 50% 0%,rgba(201,168,76,.12) 0%,transparent 60%),radial-gradient(ellipse 60% 50% at 80% 80%,rgba(201,168,76,.06) 0%,transparent 55%),linear-gradient(180deg,var(--black) 0%,#0c0900 100%);}
.hero-grid{position:absolute;inset:0;background-image:linear-gradient(rgba(201,168,76,.04) 1px,transparent 1px),linear-gradient(90deg,rgba(201,168,76,.04) 1px,transparent 1px);background-size:60px 60px;}
.hero-line{position:absolute;background:linear-gradient(90deg,transparent,rgba(201,168,76,.3),transparent);height:1px;width:100%;animation:lineScan 4s ease-in-out infinite;}
.hero-line:nth-child(1){top:25%;animation-delay:0s;}.hero-line:nth-child(2){top:55%;animation-delay:1.5s;}.hero-line:nth-child(3){top:80%;animation-delay:3s;}
@keyframes lineScan{0%{opacity:0;transform:translateX(-100%)}50%{opacity:1;transform:translateX(0)}100%{opacity:0;transform:translateX(100%)}}
.hero-inner{position:relative;z-index:2;max-width:750px;margin:0 auto;}
.hero-pill{display:inline-flex;align-items:center;gap:8px;background:rgba(201,168,76,.08);border:1px solid var(--border2);padding:6px 18px;border-radius:100px;font-size:.72rem;font-weight:700;color:var(--gold);letter-spacing:2px;text-transform:uppercase;margin-bottom:28px;animation:fadeUp .8s ease both;}
.pill-dot{width:6px;height:6px;background:var(--gold);border-radius:50%;animation:pulse 1.5s infinite;}
.hero h1{font-family:'Bebas Neue',sans-serif;font-size:clamp(4.5rem,13vw,10rem);line-height:.85;letter-spacing:3px;animation:fadeUp .8s ease .1s both;}
.h1-line1{display:block;color:var(--white);}
.h1-line2{display:block;background:linear-gradient(120deg,var(--gold3),var(--gold),var(--gold2));-webkit-background-clip:text;-webkit-text-fill-color:transparent;background-clip:text;}
.hero-sub{color:var(--muted);font-size:1rem;line-height:1.8;max-width:500px;margin:20px auto 0;animation:fadeUp .8s ease .2s both;}
.hero-socials{display:flex;align-items:center;justify-content:center;gap:10px;margin-top:22px;animation:fadeUp .8s ease .3s both;}
.soc{display:flex;align-items:center;gap:8px;padding:9px 18px;border-radius:9px;font-weight:700;font-size:.85rem;text-decoration:none;transition:all .3s;border:1px solid rgba(255,255,255,.1);color:var(--white);}
.soc:hover{transform:translateY(-3px);}
.soc-tik:hover{background:#000;border-color:rgba(255,255,255,.3);}
.soc-yt{border-color:rgba(255,0,0,.2);}.soc-yt:hover{background:rgba(255,0,0,.15);border-color:#f00;}
.hero-btns{display:flex;gap:12px;justify-content:center;flex-wrap:wrap;margin-top:30px;animation:fadeUp .8s ease .4s both;}
.btn-gold{background:linear-gradient(135deg,var(--gold),var(--gold2));color:#000;border:none;padding:14px 36px;border-radius:10px;font-weight:900;font-size:.95rem;cursor:pointer;transition:all .35s;letter-spacing:.5px;}
.btn-gold:hover{transform:translateY(-3px);box-shadow:0 10px 32px rgba(201,168,76,.45);}
.btn-outline{background:transparent;border:1px solid rgba(255,255,255,.18);color:var(--white);padding:14px 36px;border-radius:10px;font-weight:700;font-size:.95rem;cursor:pointer;transition:all .35s;}
.btn-outline:hover{border-color:var(--gold);color:var(--gold);transform:translateY(-3px);}
.hero-stats{display:flex;align-items:center;justify-content:center;gap:40px;margin-top:50px;animation:fadeUp .8s ease .5s both;flex-wrap:wrap;}
.hstat{text-align:center;}.hstat-num{font-family:'Bebas Neue',sans-serif;font-size:2.5rem;color:var(--gold);letter-spacing:2px;line-height:1;}.hstat-lbl{font-size:.7rem;color:var(--muted);letter-spacing:2px;text-transform:uppercase;margin-top:4px;}.hstat-div{width:1px;height:40px;background:var(--border2);}
@keyframes fadeUp{from{opacity:0;transform:translateY(22px)}to{opacity:1;transform:translateY(0)}}
.section{padding:88px 40px;max-width:1400px;margin:0 auto;}
.sec-label{font-size:.68rem;font-weight:700;letter-spacing:3px;text-transform:uppercase;color:var(--gold);margin-bottom:10px;}
.sec-title{font-family:'Bebas Neue',sans-serif;font-size:clamp(2rem,4vw,3.2rem);letter-spacing:1px;line-height:.95;margin-bottom:6px;}
.sec-sub{color:var(--muted);font-size:.9rem;margin-bottom:44px;}
.sec-head{display:flex;align-items:flex-end;justify-content:space-between;gap:20px;flex-wrap:wrap;margin-bottom:40px;}
.gold-divider{height:1px;background:linear-gradient(90deg,transparent,var(--gold3),transparent);margin:0 40px;}
.svc-grid{display:grid;grid-template-columns:repeat(4,1fr);gap:1px;background:var(--border);border:1px solid var(--border);border-radius:20px;overflow:hidden;}
.svc{background:var(--black2);padding:38px 24px;transition:background .3s;}.svc:hover{background:#0d0b00;}
.svc-ico{font-size:1.8rem;margin-bottom:14px;display:block;}
.svc-name{font-family:'Bebas Neue',sans-serif;font-size:1.3rem;letter-spacing:1px;margin-bottom:7px;}
.svc-desc{color:var(--muted);font-size:.82rem;line-height:1.6;}
.store-tabs{display:flex;gap:4px;background:var(--black3);border:1px solid var(--border);border-radius:12px;padding:4px;width:fit-content;margin-bottom:28px;}
.stab{padding:9px 22px;border-radius:9px;cursor:pointer;font-weight:700;font-size:.8rem;color:var(--muted);border:none;background:transparent;transition:all .25s;letter-spacing:.5px;}
.stab.on{background:linear-gradient(135deg,var(--gold),var(--gold2));color:#000;}
.games-grid{display:grid;grid-template-columns:repeat(auto-fill,minmax(200px,1fr));gap:14px;}
.g-card{background:var(--black3);border:1px solid var(--border);border-radius:var(--r2);overflow:hidden;cursor:pointer;transition:all .38s;}
.g-card:hover{border-color:var(--gold3);transform:translateY(-6px);box-shadow:0 16px 40px rgba(0,0,0,.6);}
.g-thumb{height:155px;display:flex;align-items:center;justify-content:center;font-size:3.5rem;position:relative;overflow:hidden;}
.g-thumb-bg{position:absolute;inset:0;opacity:.85;}.g-thumb-overlay{position:absolute;inset:0;background:linear-gradient(0deg,rgba(8,8,8,.85) 0%,transparent 60%);}
.g-ico{position:relative;z-index:2;filter:drop-shadow(0 4px 12px rgba(0,0,0,.8));}
.g-badge{position:absolute;top:10px;right:10px;z-index:3;font-size:.58rem;font-weight:900;padding:3px 9px;border-radius:5px;letter-spacing:1px;text-transform:uppercase;background:linear-gradient(135deg,var(--gold),var(--gold2));color:#000;}
.g-body{padding:14px;}.g-name{font-weight:700;font-size:.88rem;margin-bottom:3px;}.g-plat{color:var(--muted);font-size:.72rem;margin-bottom:8px;}
.g-footer{display:flex;align-items:center;justify-content:space-between;}
.g-price{font-family:'Bebas Neue',sans-serif;font-size:1.3rem;color:var(--gold);letter-spacing:1px;}.g-price small{font-family:'Tajawal';font-size:.65rem;color:var(--muted);}
.g-btn{background:rgba(201,168,76,.1);border:1px solid var(--border);color:var(--gold);padding:6px 14px;border-radius:7px;font-size:.74rem;font-weight:700;cursor:pointer;transition:all .25s;}
.g-btn:hover{background:linear-gradient(135deg,var(--gold),var(--gold2));color:#000;border-color:transparent;}
.charge-layout{display:grid;grid-template-columns:1fr 1.1fr;gap:60px;align-items:start;}
.charge-info h2{font-family:'Bebas Neue',sans-serif;font-size:2.8rem;letter-spacing:1px;margin-bottom:14px;}
.charge-info p{color:var(--muted);line-height:1.8;margin-bottom:28px;}
.feats{display:flex;flex-direction:column;gap:10px;}
.feat{display:flex;align-items:center;gap:12px;padding:14px;border:1px solid var(--border);border-radius:12px;background:var(--black3);transition:border-color .3s;}
.feat:hover{border-color:var(--border2);}
.feat-ico{width:40px;height:40px;border-radius:10px;display:flex;align-items:center;justify-content:center;font-size:1.1rem;flex-shrink:0;}
.feat-title{font-weight:700;font-size:.88rem;margin-bottom:2px;}.feat-sub{color:var(--muted);font-size:.74rem;}
.charge-form{background:var(--black3);border:1px solid var(--border);border-radius:var(--r2);padding:32px;}
.charge-form h3{font-size:1.1rem;font-weight:900;margin-bottom:24px;}
.ops{display:grid;grid-template-columns:repeat(3,1fr);gap:10px;margin-bottom:22px;}
.op{border:2px solid var(--border);border-radius:12px;padding:16px 8px;text-align:center;cursor:pointer;transition:all .28s;background:rgba(255,255,255,.02);}
.op:hover,.op.sel{border-color:var(--gold);background:rgba(201,168,76,.07);}
.op-em{font-size:1.8rem;display:block;margin-bottom:6px;}.op-name{font-weight:900;font-size:.78rem;}.op-sub{font-size:.62rem;color:var(--muted);margin-top:2px;}
.flabel{display:block;font-size:.65rem;font-weight:700;letter-spacing:2px;text-transform:uppercase;color:var(--muted);margin-bottom:7px;}
.finput{width:100%;background:rgba(255,255,255,.04);border:1px solid var(--border);border-radius:10px;padding:12px 14px;color:var(--white);font-size:.92rem;outline:none;transition:border-color .3s;margin-bottom:14px;}
.finput:focus{border-color:var(--gold);}
.amts{display:grid;grid-template-columns:repeat(3,1fr);gap:8px;margin-bottom:18px;}
.amt{background:var(--black4);border:1px solid var(--border);border-radius:9px;padding:10px 6px;text-align:center;cursor:pointer;transition:all .22s;}
.amt:hover,.amt.sel{border-color:var(--gold);background:rgba(201,168,76,.08);}
.amt-val{font-family:'Bebas Neue',sans-serif;font-size:1.1rem;color:var(--gold);}.amt-bonus{font-size:.6rem;color:#e04040;font-weight:700;margin-top:1px;}
.charge-btn{width:100%;background:linear-gradient(135deg,var(--gold),var(--gold2));border:none;padding:14px;border-radius:11px;color:#000;font-weight:900;font-size:.95rem;cursor:pointer;transition:all .3s;letter-spacing:.5px;}
.charge-btn:hover{transform:translateY(-2px);box-shadow:0 8px 28px rgba(201,168,76,.45);}
.comm-box{background:var(--black3);border:1px solid var(--border);border-radius:var(--r2);overflow:hidden;}
.comm-header{padding:22px 28px;border-bottom:1px solid var(--border);display:flex;align-items:center;justify-content:space-between;}
.comm-header h3{font-size:1rem;font-weight:900;}
.online-pill{display:flex;align-items:center;gap:6px;font-size:.72rem;color:var(--muted);}
.online-dot{width:7px;height:7px;background:#22c55e;border-radius:50%;animation:pulse 2s infinite;}
.comm-body{padding:24px 28px;}
.post-box{background:rgba(255,255,255,.03);border:1px solid var(--border);border-radius:12px;padding:16px;margin-bottom:18px;}
.post-box textarea{width:100%;background:transparent;border:none;outline:none;color:var(--white);resize:none;min-height:70px;line-height:1.7;font-size:.9rem;}
.post-box textarea::placeholder{color:var(--muted);}
.post-actions{display:flex;align-items:center;justify-content:space-between;margin-top:10px;padding-top:10px;border-top:1px solid var(--border);}
.emoji-btns{display:flex;gap:7px;}
.emo{background:none;border:none;font-size:1.1rem;cursor:pointer;padding:3px;transition:transform .2s;}.emo:hover{transform:scale(1.3);}
.post-btn{background:linear-gradient(135deg,var(--gold),var(--gold2));color:#000;border:none;padding:8px 20px;border-radius:8px;font-weight:900;font-size:.8rem;cursor:pointer;transition:all .25s;}
.post-btn:hover{box-shadow:0 4px 18px rgba(201,168,76,.4);}
.posts-feed{display:flex;flex-direction:column;gap:12px;max-height:500px;overflow-y:auto;padding-left:2px;}
.posts-feed::-webkit-scrollbar{width:3px;}.posts-feed::-webkit-scrollbar-thumb{background:var(--gold3);}
.post{background:rgba(255,255,255,.025);border:1px solid var(--border);border-radius:12px;padding:14px;transition:border-color .25s;}.post:hover{border-color:var(--border2);}
.post-head{display:flex;align-items:center;gap:10px;margin-bottom:10px;}
.post-av{width:36px;height:36px;border-radius:9px;display:flex;align-items:center;justify-content:center;font-size:1rem;flex-shrink:0;border:1px solid var(--border);}
.post-name{font-weight:700;font-size:.85rem;}.post-time{color:var(--muted);font-size:.7rem;}
.post-role{background:rgba(201,168,76,.1);border:1px solid var(--border2);color:var(--gold);font-size:.58rem;font-weight:700;padding:2px 7px;border-radius:4px;}
.post-text{color:rgba(255,255,255,.75);font-size:.88rem;line-height:1.65;margin-bottom:10px;}
.post-btns{display:flex;gap:12px;}
.post-action{background:none;border:none;color:var(--muted);font-size:.76rem;cursor:pointer;display:flex;align-items:center;gap:4px;transition:color .2s;padding:0;}.post-action:hover{color:var(--gold);}
.vid-grid{display:grid;grid-template-columns:repeat(auto-fill,minmax(280px,1fr));gap:16px;}
.vid-card{background:var(--black3);border:1px solid var(--border);border-radius:var(--r2);overflow:hidden;cursor:pointer;transition:all .35s;}
.vid-card:hover{border-color:var(--gold3);transform:translateY(-5px);box-shadow:0 14px 36px rgba(0,0,0,.5);}
.vid-thumb{height:175px;display:flex;align-items:center;justify-content:center;font-size:4rem;position:relative;background:var(--black4);}
.vid-play{position:absolute;width:54px;height:54px;background:rgba(201,168,76,.9);border-radius:50%;display:flex;align-items:center;justify-content:center;font-size:1.2rem;transition:all .3s;}
.vid-card:hover .vid-play{background:var(--gold2);transform:scale(1.12);}
.vid-body{padding:15px;}.vid-name{font-weight:700;font-size:.9rem;margin-bottom:5px;}.vid-meta{color:var(--muted);font-size:.74rem;}
.vid-upload{border:2px dashed var(--border2);border-radius:var(--r2);padding:50px;text-align:center;cursor:pointer;transition:all .3s;background:rgba(201,168,76,.02);margin-bottom:28px;}
.vid-upload:hover{border-color:var(--gold);background:rgba(201,168,76,.05);}
.admin-gate{background:var(--black3);border:1px solid var(--border);border-radius:var(--r2);padding:48px;max-width:420px;margin:0 auto;text-align:center;}
.admin-pin{width:100%;background:rgba(201,168,76,.05);border:1px solid var(--border2);border-radius:12px;padding:16px;color:var(--gold);font-family:'Bebas Neue',sans-serif;font-size:1.6rem;font-weight:700;letter-spacing:6px;text-align:center;outline:none;transition:all .3s;margin-bottom:16px;}
.admin-pin:focus{border-color:var(--gold);}
.admin-pin.err{border-color:#e04040;animation:shake .3s;}
@keyframes shake{0%,100%{transform:translateX(0)}25%{transform:translateX(-7px)}75%{transform:translateX(7px)}}
.admin-enter{width:100%;background:linear-gradient(135deg,var(--gold),var(--gold2));border:none;padding:14px;border-radius:11px;color:#000;font-weight:900;font-size:1rem;cursor:pointer;transition:all .3s;margin-bottom:10px;}
.admin-enter:hover{box-shadow:0 6px 24px rgba(201,168,76,.45);}
.admin-dash{display:none;}.admin-dash.show{display:block;}
.kpi-row{display:grid;grid-template-columns:repeat(4,1fr);gap:14px;margin-bottom:24px;}
.kpi{background:var(--black3);border:1px solid var(--border);border-radius:var(--r2);padding:22px;}
.kpi-lbl{font-size:.66rem;font-weight:700;letter-spacing:2px;text-transform:uppercase;color:var(--muted);margin-bottom:8px;}
.kpi-val{font-family:'Bebas Neue',sans-serif;font-size:2.3rem;letter-spacing:1px;line-height:1;}.kpi-sub{color:var(--muted);font-size:.72rem;margin-top:5px;}
.kpi.gold .kpi-val{color:var(--gold);}.kpi.green .kpi-val{color:#22c55e;}.kpi.blue .kpi-val{color:#38bdf8;}.kpi.red .kpi-val{color:#f87171;}
.adm-table{background:var(--black3);border:1px solid var(--border);border-radius:var(--r2);overflow:hidden;}
.adm-thead{padding:16px 22px;border-bottom:1px solid var(--border);font-size:.68rem;font-weight:700;letter-spacing:2px;text-transform:uppercase;color:var(--muted);}
.adm-row{display:flex;align-items:center;gap:14px;padding:13px 22px;border-bottom:1px solid var(--border);transition:background .2s;}.adm-row:last-child{border-bottom:none;}.adm-row:hover{background:rgba(255,255,255,.02);}
.adm-ico{width:34px;height:34px;border-radius:8px;display:flex;align-items:center;justify-content:center;font-size:.95rem;flex-shrink:0;background:rgba(201,168,76,.1);}
.adm-name{flex:1;font-weight:700;font-size:.84rem;}.adm-sub{color:var(--muted);font-size:.7rem;margin-top:1px;}
.adm-price{font-family:'Bebas Neue',sans-serif;font-size:1rem;color:var(--gold);}
.adm-status{font-size:.64rem;font-weight:700;padding:3px 9px;border-radius:5px;background:rgba(34,197,94,.12);color:#22c55e;border:1px solid rgba(34,197,94,.2);}
.adm-chart{background:var(--black3);border:1px solid var(--border);border-radius:var(--r2);padding:22px;margin-bottom:18px;}
.chart-lbl{font-size:.68rem;font-weight:700;letter-spacing:2px;text-transform:uppercase;color:var(--muted);margin-bottom:16px;}
.chart-bars{display:flex;align-items:flex-end;gap:8px;height:90px;}
.cbar-wrap{flex:1;display:flex;flex-direction:column;align-it