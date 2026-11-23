# -Mercedes-AMG-E63
A modern and interactive website showcasing the history of the Mercedes-Benz E63 AMG, featuring its generations, engine specifications, performance, exterior and interior design, and photo gallery. Built with a luxurious AMG-inspired design
<!DOCTYPE html>
<html lang="ar" dir="rtl">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1">
<meta name="description" content="Mercedes-AMG E63 — The Power of a Legend. تاريخ سيارة مرسيدس AMG E63 من جيل W211 حتى W213، مواصفاتها، محركاتها، تصميمها وأدائها.">
<title>Mercedes-AMG E63 | The Power of a Legend</title>
<link rel="preconnect" href="https://fonts.googleapis.com">
<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
<link href="https://fonts.googleapis.com/css2?family=Tajawal:wght@300;400;500;700;800;900&family=Rajdhani:wght@400;500;600;700&display=swap" rel="stylesheet">
<style>
  :root{
    --black:#070707;
    --carbon:#0f0f10;
    --graphite:#161618;
    --panel:#1b1b1e;
    --line:#2a2a2e;
    --red:#e2001a;
    --red-bright:#ff1f2e;
    --red-deep:#8a0010;
    --silver:#c8ccd0;
    --silver-dim:#8b9096;
    --white:#f4f5f7;
    --gold:#b08d57;
    --ease:cubic-bezier(.16,.84,.3,1);
    --maxw:1280px;
  }
  *{margin:0;padding:0;box-sizing:border-box}
  html{scroll-behavior:smooth;-webkit-text-size-adjust:100%}
  body{
    font-family:'Tajawal',system-ui,sans-serif;
    background:var(--black);
    color:var(--silver);
    line-height:1.8;
    overflow-x:hidden;
    font-weight:400;
  }
  img{display:block;max-width:100%;height:auto}
  a{color:inherit;text-decoration:none}
  ::selection{background:var(--red);color:#fff}

  /* ---------- Scrollbar ---------- */
  ::-webkit-scrollbar{width:10px}
  ::-webkit-scrollbar-track{background:var(--carbon)}
  ::-webkit-scrollbar-thumb{background:linear-gradient(var(--red),var(--red-deep));border-radius:6px}

  /* ---------- Layout ---------- */
  .wrap{max-width:var(--maxw);margin:0 auto;padding:0 24px}
  .lat{font-family:'Rajdhani',sans-serif;letter-spacing:.06em}

  /* ---------- Header / Nav ---------- */
  header{
    position:fixed;top:0;left:0;right:0;z-index:1000;
    transition:background .4s var(--ease),backdrop-filter .4s,box-shadow .4s;
    padding:18px 0;
  }
  header.scrolled{
    background:rgba(7,7,7,.82);
    backdrop-filter:blur(14px);
    box-shadow:0 1px 0 rgba(226,0,26,.35),0 12px 40px rgba(0,0,0,.6);
    padding:12px 0;
  }
  .nav{display:flex;align-items:center;justify-content:space-between;gap:20px}
  .brand{display:flex;align-items:center;gap:12px;flex-shrink:0}
  .brand-star{
    width:30px;height:30px;border:1.5px solid var(--silver);border-radius:50%;
    display:grid;place-items:center;position:relative;
  }
  .brand-star::before{
    content:"";position:absolute;inset:0;border-radius:50%;
    background:radial-gradient(circle at 50% 50%,var(--red),transparent 60%);
    opacity:.55;
  }
  .brand-star svg{position:relative;z-index:1;width:14px;height:14px;fill:var(--silver)}
  .brand-txt{display:flex;flex-direction:column;line-height:1.1}
  .brand-txt b{font-family:'Rajdhani',sans-serif;font-weight:700;font-size:17px;letter-spacing:.12em;color:var(--white)}
  .brand-txt small{font-size:10px;letter-spacing:.22em;color:var(--red-bright);font-weight:700}
  .menu{display:flex;align-items:center;gap:6px}
  .menu a{
    font-size:13.5px;font-weight:500;color:var(--silver-dim);
    padding:8px 13px;border-radius:6px;transition:.25s;position:relative;
  }
  .menu a:hover,.menu a.active{color:var(--white);background:rgba(255,255,255,.04)}
  .menu a.active::after{
    content:"";position:absolute;bottom:2px;left:13px;right:13px;height:2px;
    background:linear-gradient(90deg,var(--red),transparent);border-radius:2px;
  }
  .nav-cta{
    font-family:'Rajdhani',sans-serif;font-weight:600;font-size:13px;letter-spacing:.1em;
    color:var(--white);padding:9px 18px;border:1px solid var(--red);
    background:linear-gradient(180deg,rgba(226,0,26,.18),rgba(226,0,26,.02));
    border-radius:3px;transition:.3s;cursor:pointer;white-space:nowrap;
  }
  .nav-cta:hover{background:var(--red);box-shadow:0 0 26px rgba(226,0,26,.6)}
  .burger{display:none;flex-direction:column;gap:5px;cursor:pointer;padding:6px}
  .burger span{width:26px;height:2px;background:var(--silver);transition:.3s}
  .burger.active span:nth-child(1){transform:translateY(7px) rotate(45deg)}
  .burger.active span:nth-child(2){opacity:0}
  .burger.active span:nth-child(3){transform:translateY(-7px) rotate(-45deg)}

  /* ---------- Hero ---------- */
  .hero{
    position:relative;min-height:100vh;display:flex;align-items:center;
    overflow:hidden;
  }
  .hero-bg{
    position:absolute;inset:0;z-index:0;
    background:url('https://z-cdn.chatglm.cn/image-search-mcp/images-ppt/76fe09763dc6.jpg') center/cover no-repeat;
    transform:scale(1.05);
  }
  .hero-bg::after{
    content:"";position:absolute;inset:0;
    background:
      radial-gradient(ellipse 60% 50% at 70% 40%,rgba(226,0,26,.22),transparent 60%),
      linear-gradient(90deg,rgba(7,7,7,.96) 0%,rgba(7,7,7,.7) 35%,rgba(7,7,7,.2) 65%,rgba(7,7,7,.55) 100%),
      linear-gradient(0deg,rgba(7,7,7,1) 2%,transparent 30%);
  }
  .hero-grid{
    position:absolute;inset:0;z-index:1;opacity:.18;
    background-image:linear-gradient(rgba(200,204,208,.07) 1px,transparent 1px),
                     linear-gradient(90deg,rgba(200,204,208,.07) 1px,transparent 1px);
    background-size:60px 60px;
    mask-image:radial-gradient(ellipse 80% 60% at 50% 50%,#000,transparent 75%);
  }
  .hero-content{position:relative;z-index:2;max-width:760px;padding-top:60px}
  .eyebrow{
    display:inline-flex;align-items:center;gap:10px;
    font-family:'Rajdhani',sans-serif;font-size:13px;font-weight:600;letter-spacing:.28em;
    color:var(--silver);text-transform:uppercase;margin-bottom:22px;
    padding:7px 16px;border:1px solid var(--line);border-radius:40px;
    background:rgba(15,15,16,.6);backdrop-filter:blur(6px);
  }
  .eyebrow .dot{width:7px;height:7px;border-radius:50%;background:var(--red);box-shadow:0 0 12px var(--red)}
  .hero h1{
    font-family:'Tajawal',sans-serif;font-weight:900;
    font-size:clamp(2.8rem,8vw,5.4rem);line-height:.98;color:var(--white);
    letter-spacing:-.01em;margin-bottom:8px;
  }
  .hero h1 .lat-name{display:block;font-family:'Rajdhani',sans-serif;font-weight:700;letter-spacing:.04em}
  .hero h1 .accent{color:var(--red-bright);text-shadow:0 0 40px rgba(255,31,46,.5)}
  .hero-tagline{
    font-family:'Rajdhani',sans-serif;font-weight:500;font-size:clamp(1.1rem,3vw,1.7rem);
    letter-spacing:.04em;color:var(--silver);margin:18px 0 14px;
  }
  .hero-tagline em{font-style:normal;color:var(--white);font-weight:600}
  .hero-sub{font-size:clamp(1rem,2.2vw,1.15rem);color:var(--silver-dim);max-width:540px;margin-bottom:34px;line-height:1.9}
  .hero-btns{display:flex;gap:14px;flex-wrap:wrap}
  .btn-primary{
    display:inline-flex;align-items:center;gap:12px;
    font-family:'Tajdhani',sans-serif;font-weight:600;font-size:15px;letter-spacing:.1em;
    color:#fff;padding:15px 30px;background:var(--red);
    border:none;border-radius:3px;cursor:pointer;transition:.3s;position:relative;overflow:hidden;
  }
  .btn-primary::before{content:"";position:absolute;inset:0;background:linear-gradient(120deg,transparent,rgba(255,255,255,.25),transparent);transform:translateX(-120%);transition:.6s}
  .btn-primary:hover{box-shadow:0 0 30px rgba(226,0,26,.7),0 0 60px rgba(226,0,26,.3);transform:translateY(-2px)}
  .btn-primary:hover::before{transform:translateX(120%)}
  .btn-primary svg{width:16px;height:16px}
  .btn-ghost{
    display:inline-flex;align-items:center;gap:10px;
    font-family:'Rajdhani',sans-serif;font-weight:500;font-size:14px;letter-spacing:.1em;
    color:var(--silver);padding:14px 26px;border:1px solid var(--line);
    background:rgba(15,15,16,.4);border-radius:3px;cursor:pointer;transition:.3s;
  }
  .btn-ghost:hover{border-color:var(--silver);color:var(--white);background:rgba(255,255,255,.06)}
  .scroll-cue{
    position:absolute;bottom:26px;left:50%;transform:translateX(-50%);z-index:3;
    display:flex;flex-direction:column;align-items:center;gap:8px;
    color:var(--silver-dim);font-family:'Rajdhani',sans-serif;font-size:11px;letter-spacing:.3em;
  }
  .scroll-cue .mouse{width:22px;height:36px;border:1.5px solid var(--silver-dim);border-radius:12px;position:relative}
  .scroll-cue .mouse::before{content:"";position:absolute;top:6px;left:50%;transform:translateX(-50%);width:3px;height:7px;background:var(--red);border-radius:2px;animation:scrollDot 1.8s infinite}
  @keyframes scrollDot{0%{opacity:0;transform:translate(-50%,0)}40%{opacity:1}80%{opacity:0;transform:translate(-50%,14px)}100%{opacity:0}}

  /* ---------- Section base ---------- */
  section{position:relative;padding:100px 0}
  .sec-head{margin-bottom:54px;text-align:center}
  .sec-kicker{
    font-family:'Rajdhani',sans-serif;font-size:13px;font-weight:600;letter-spacing:.32em;
    color:var(--red-bright);text-transform:uppercase;margin-bottom:14px;display:inline-block;
  }
  .sec-kicker::before,.sec-kicker::after{content:"";display:inline-block;width:34px;height:1px;background:var(--red);vertical-align:middle;margin:0 12px;opacity:.6}
  .sec-title{
    font-family:'Tajawal',sans-serif;font-weight:800;
    font-size:clamp(2rem,5vw,3.2rem);color:var(--white);line-height:1.1;letter-spacing:-.01em;
  }
  .sec-title .lat{display:block;font-family:'Rajdhani',sans-serif;font-weight:700;letter-spacing:.04em;color:var(--silver-dim);font-size:.5em;margin-top:8px}
  .sec-lead{max-width:720px;margin:18px auto 0;color:var(--silver-dim);font-size:1.05rem;line-height:1.9}

  /* ---------- History ---------- */
  #history{background:linear-gradient(180deg,var(--black),var(--carbon))}
  .history-grid{display:grid;grid-template-columns:1.1fr 1fr;gap:56px;align-items:center}
  .history-text h3{font-size:1.7rem;font-weight:800;color:var(--white);margin-bottom:18px;line-height:1.3}
  .history-text p{color:var(--silver);margin-bottom:18px;font-size:1.05rem;line-height:1.95}
  .history-text p strong{color:var(--white)}
  .history-text .red{color:var(--red-bright);font-weight:700}
  .history-img{position:relative;border-radius:6px;overflow:hidden;box-shadow:0 30px 70px rgba(0,0,0,.7)}
  .history-img img{width:100%;height:420px;object-fit:cover;transition:transform 1.2s var(--ease)}
  .history-img:hover img{transform:scale(1.06)}
  .history-img::after{content:"";position:absolute;inset:0;border:1px solid rgba(226,0,26,.3);border-radius:6px;pointer-events:none}
  .history-badge{
    position:absolute;top:18px;right:18px;z-index:2;
    font-family:'Rajdhani',sans-serif;font-weight:700;font-size:12px;letter-spacing:.18em;
    color:#fff;background:rgba(226,0,26,.85);padding:7px 14px;border-radius:2px;backdrop-filter:blur(4px);
  }
  .timeline-mini{display:flex;gap:0;margin-top:30px;border:1px solid var(--line);border-radius:6px;overflow:hidden}
  .timeline-mini .t{flex:1;padding:16px 14px;text-align:center;background:var(--panel);border-left:1px solid var(--line)}
  .timeline-mini .t:first-child{border-left:none}
  .timeline-mini .y{font-family:'Rajdhani',sans-serif;font-weight:700;font-size:1.3rem;color:var(--red-bright)}
  .timeline-mini .g{font-size:13px;color:var(--silver);margin-top:4px}

  /* ---------- Generations ---------- */
  #generations{background:var(--carbon)}
  .gen-block{display:grid;grid-template-columns:1fr 1fr;gap:50px;align-items:center;margin-bottom:90px}
  .gen-block:last-child{margin-bottom:0}
  .gen-block.flip .gen-media{order:2}
  .gen-media{position:relative;border-radius:6px;overflow:hidden;box-shadow:0 26px 60px rgba(0,0,0,.65)}
  .gen-media img{width:100%;height:360px;object-fit:cover;transition:transform 1.1s var(--ease)}
  .gen-media:hover img{transform:scale(1.05)}
  .gen-media::after{content:"";position:absolute;inset:0;box-shadow:inset 0 0 80px rgba(0,0,0,.6);pointer-events:none}
  .gen-year-tag{
    position:absolute;top:16px;right:16px;z-index:2;
    font-family:'Rajdhani',sans-serif;font-weight:700;font-size:13px;letter-spacing:.16em;
    color:#fff;background:rgba(7,7,7,.78);border:1px solid var(--red);padding:7px 13px;border-radius:2px;
  }
  .gen-info .gen-code{
    font-family:'Rajdhani',sans-serif;font-weight:700;font-size:clamp(2.2rem,5vw,3rem);
    color:var(--white);letter-spacing:.02em;line-height:1;
  }
  .gen-info .gen-code span{color:var(--red-bright)}
  .gen-info .gen-period{font-family:'Rajdhani',sans-serif;color:var(--silver-dim);letter-spacing:.14em;margin:6px 0 18px;font-size:15px}
  .gen-info .gen-engine{font-size:1.15rem;color:var(--silver);margin-bottom:20px;font-weight:500}
  .gen-info .gen-engine b{color:var(--white)}
  .gen-info p.desc{color:var(--silver-dim);font-size:1rem;line-height:1.95;margin-bottom:22px}
  .gen-specs{display:grid;grid-template-columns:repeat(3,1fr);gap:12px}
  .gen-specs .sp{
    background:var(--panel);border:1px solid var(--line);border-radius:5px;padding:14px 12px;text-align:center;
    transition:.3s;
  }
  .gen-specs .sp:hover{border-color:var(--red);transform:translateY(-3px)}
  .gen-specs .v{font-family:'Rajdhani',sans-serif;font-weight:700;font-size:1.5rem;color:var(--white);line-height:1}
  .gen-specs .v small{font-size:.62em;color:var(--silver-dim);font-weight:500}
  .gen-specs .l{font-size:11px;color:var(--silver-dim);margin-top:6px;letter-spacing:.02em}

  /* ---------- Performance ---------- */
  #performance{
    background:
      radial-gradient(ellipse 70% 50% at 50% 0%,rgba(226,0,26,.12),transparent 60%),
      linear-gradient(180deg,var(--carbon),var(--black));
  }
  .perf-layout{display:grid;grid-template-columns:1fr 1.1fr;gap:54px;align-items:center;margin-bottom:60px}
  .perf-img{position:relative;border-radius:6px;overflow:hidden;box-shadow:0 26px 60px rgba(0,0,0,.6)}
  .perf-img img{width:100%;height:420px;object-fit:cover}
  .perf-img::after{content:"";position:absolute;inset:0;border:1px solid rgba(255,255,255,.06);border-radius:6px}
  .perf-img .live-tag{
    position:absolute;bottom:14px;right:14px;
    font-family:'Rajdhani',sans-serif;font-size:12px;letter-spacing:.18em;color:#fff;
    background:rgba(226,0,26,.85);padding:6px 12px;border-radius:2px;
  }
  .perf-text h3{font-size:1.7rem;font-weight:800;color:var(--white);margin-bottom:16px}
  .perf-text p{color:var(--silver);margin-bottom:16px;line-height:1.95}
  .perf-text p b{color:var(--white)}
  .perf-text .red{color:var(--red-bright);font-weight:700}
  .stat-grid{display:grid;grid-template-columns:repeat(4,1fr);gap:18px;margin-top:8px}
  .stat-card{
    background:linear-gradient(180deg,var(--panel),var(--carbon));
    border:1px solid var(--line);border-radius:6px;padding:28px 16px;text-align:center;
    position:relative;overflow:hidden;transition:.35s;
  }
  .stat-card::before{content:"";position:absolute;top:0;left:0;right:0;height:2px;background:linear-gradient(90deg,var(--red),transparent)}
  .stat-card:hover{border-color:var(--red);transform:translateY(-4px);box-shadow:0 14px 40px rgba(226,0,26,.18)}
  .stat-card .num{font-family:'Rajdhani',sans-serif;font-weight:700;font-size:clamp(2rem,5vw,2.8rem);color:var(--white);line-height:1}
  .stat-card .num small{font-size:.42em;color:var(--red-bright);font-weight:600;margin-right:3px}
  .stat-card .lab{font-size:13px;color:var(--silver-dim);margin-top:10px;letter-spacing:.02em}
  .feat-row{display:grid;grid-template-columns:repeat(3,1fr);gap:20px;margin-top:64px}
  .feat-card{
    background:var(--panel);border:1px solid var(--line);border-radius:6px;padding:28px;
    transition:.35s;position:relative;
  }
  .feat-card:hover{border-color:var(--red);transform:translateY(-4px)}
  .feat-card .ico{
    width:48px;height:48px;border-radius:6px;display:grid;place-items:center;margin-bottom:16px;
    background:linear-gradient(135deg,rgba(226,0,26,.2),rgba(226,0,26,.04));border:1px solid rgba(226,0,26,.4);
  }
  .feat-card .ico svg{width:24px;height:24px;fill:var(--red-bright)}
  .feat-card h4{font-size:1.2rem;font-weight:800;color:var(--white);margin-bottom:10px}
  .feat-card p{color:var(--silver-dim);font-size:.96rem;line-height:1.85}

  /* ---------- Exterior ---------- */
  #exterior{background:var(--black)}
  .ext-hero{position:relative;border-radius:6px;overflow:hidden;margin-bottom:40px;box-shadow:0 26px 60px rgba(0,0,0,.6)}
  .ext-hero img{width:100%;height:clamp(280px,42vw,560px);object-fit:cover}
  .ext-hero::after{content:"";position:absolute;inset:0;background:linear-gradient(180deg,transparent 50%,rgba(7,7,7,.85))}
  .ext-hero .cap{
    position:absolute;bottom:24px;right:28px;z-index:2;max-width:60%;
  }
  .ext-hero .cap h3{font-size:clamp(1.4rem,3.5vw,2rem);color:#fff;font-weight:800}
  .ext-hero .cap p{color:var(--silver);font-size:.98rem;margin-top:6px}
  .ext-grid{display:grid;grid-template-columns:repeat(3,1fr);gap:20px}
  .ext-card{background:var(--panel);border:1px solid var(--line);border-radius:6px;overflow:hidden;transition:.35s}
  .ext-card:hover{border-color:var(--red);transform:translateY(-5px);box-shadow:0 18px 44px rgba(0,0,0,.5)}
  .ext-card .img{height:200px;overflow:hidden;position:relative}
  .ext-card .img img{width:100%;height:100%;object-fit:cover;transition:transform .8s var(--ease)}
  .ext-card:hover .img img{transform:scale(1.08)}
  .ext-card .body{padding:22px}
  .ext-card h4{font-size:1.15rem;font-weight:800;color:var(--white);margin-bottom:8px}
  .ext-card h4 .lat{font-family:'Rajdhani',sans-serif;color:var(--red-bright);font-size:.78em;letter-spacing:.04em;margin-right:6px}
  .ext-card p{color:var(--silver-dim);font-size:.95rem;line-height:1.85}

  /* ---------- Interior ---------- */
  #interior{
    background:
      radial-gradient(ellipse 60% 40% at 80% 30%,rgba(226,0,26,.1),transparent 60%),
      var(--carbon);
  }
  .int-layout{display:grid;grid-template-columns:1.3fr 1fr;gap:48px;align-items:center}
  .int-main{position:relative;border-radius:6px;overflow:hidden;box-shadow:0 26px 60px rgba(0,0,0,.6)}
  .int-main img{width:100%;height:480px;object-fit:cover}
  .int-main::after{content:"";position:absolute;inset:0;border:1px solid rgba(255,255,255,.05)}
  .int-text h3{font-size:1.7rem;font-weight:800;color:var(--white);margin-bottom:16px}
  .int-text>p{color:var(--silver);margin-bottom:22px;line-height:1.95}
  .int-list{list-style:none}
  .int-list li{
    display:flex;gap:14px;padding:14px 0;border-bottom:1px solid var(--line);
  }
  .int-list li:last-child{border-bottom:none}
  .int-list .mk{
    flex-shrink:0;width:30px;height:30px;border-radius:5px;
    background:rgba(226,0,26,.12);border:1px solid rgba(226,0,26,.4);
    display:grid;place-items:center;color:var(--red-bright);font-family:'Rajdhani',sans-serif;font-weight:700;font-size:14px;
  }
  .int-list .ct b{display:block;color:var(--white);font-size:1.05rem;margin-bottom:3px}
  .int-list .ct span{color:var(--silver-dim);font-size:.94rem;line-height:1.8}
  .int-strip{display:grid;grid-template-columns:1fr 1fr;gap:18px;margin-top:36px}
  .int-strip .ph{border-radius:5px;overflow:hidden;height:180px;border:1px solid var(--line)}
  .int-strip .ph img{width:100%;height:100%;object-fit:cover;transition:transform .8s var(--ease)}
  .int-strip .ph:hover img{transform:scale(1.06)}

  /* ---------- Gallery ---------- */
  #gallery{background:var(--black)}
  .gallery-grid{display:grid;grid-template-columns:repeat(4,1fr);gap:14px}
  .gitem{position:relative;overflow:hidden;border-radius:5px;cursor:pointer;background:var(--panel);border:1px solid var(--line)}
  .gitem img{width:100%;height:100%;object-fit:cover;transition:transform .9s var(--ease),filter .4s;filter:brightness(.9)}
  .gitem:hover img{transform:scale(1.08);filter:brightness(1.05)}
  .gitem::after{
    content:"";position:absolute;inset:0;background:linear-gradient(180deg,transparent 55%,rgba(7,7,7,.7));
    opacity:.7;transition:.4s;
  }
  .gitem:hover::after{opacity:.3}
  .gitem .zoom{
    position:absolute;top:50%;left:50%;transform:translate(-50%,-50%) scale(.6);
    width:46px;height:46px;border-radius:50%;border:1.5px solid #fff;display:grid;place-items:center;
    opacity:0;transition:.4s;z-index:2;background:rgba(226,0,26,.4);
  }
  .gitem:hover .zoom{opacity:1;transform:translate(-50%,-50%) scale(1)}
  .gitem .zoom svg{width:20px;height:20px;fill:#fff}
  .gitem .gl-label{
    position:absolute;bottom:12px;right:14px;z-index:2;
    font-family:'Rajdhani',sans-serif;font-size:12px;letter-spacing:.12em;color:var(--silver);
  }
  .gitem.tall{grid-row:span 2}
  .gitem.wide{grid-column:span 2}

  /* Lightbox */
  .lightbox{
    position:fixed;inset:0;z-index:2000;background:rgba(5,5,5,.95);backdrop-filter:blur(10px);
    display:none;align-items:center;justify-content:center;padding:40px;
  }
  .lightbox.open{display:flex;animation:fadeIn .3s}
  @keyframes fadeIn{from{opacity:0}to{opacity:1}}
  .lightbox img{max-width:92vw;max-height:86vh;border-radius:4px;box-shadow:0 0 80px rgba(226,0,26,.25);border:1px solid rgba(255,255,255,.08)}
  .lb-close{position:absolute;top:24px;left:24px;width:44px;height:44px;border-radius:50%;border:1px solid var(--silver-dim);background:rgba(15,15,16,.6);color:#fff;font-size:24px;cursor:pointer;display:grid;place-items:center;transition:.3s}
  .lb-close:hover{background:var(--red);border-color:var(--red);transform:rotate(90deg)}
  .lb-nav{position:absolute;top:50%;transform:translateY(-50%);width:50px;height:50px;border-radius:50%;border:1px solid var(--silver-dim);background:rgba(15,15,16,.6);color:#fff;cursor:pointer;display:grid;place-items:center;transition:.3s}
  .lb-nav:hover{background:var(--red);border-color:var(--red)}
  .lb-nav.prev{right:24px}
  .lb-nav.next{left:24px}
  .lb-nav svg{width:22px;height:22px;fill:#fff}
  .lb-counter{position:absolute;bottom:24px;left:50%;transform:translateX(-50%);font-family:'Rajdhani',sans-serif;color:var(--silver-dim);letter-spacing:.1em;font-size:14px}

  /* ---------- Conclusion ---------- */
  #conclusion{
    position:relative;text-align:center;padding:130px 0;overflow:hidden;
    background:
      radial-gradient(ellipse 50% 60% at 50% 50%,rgba(226,0,26,.18),transparent 65%),
      linear-gradient(180deg,var(--black),var(--carbon));
  }
  .conc-line{width:60px;height:2px;background:var(--red);margin:0 auto 26px}
  .conc-title{
    font-family:'Rajdhani',sans-serif;font-weight:700;
    font-size:clamp(2rem,6vw,4rem);color:var(--white);letter-spacing:.02em;line-height:1.1;
  }
  .conc-title .red{color:var(--red-bright);text-shadow:0 0 50px rgba(255,31,46,.5)}
  .conc-sub{font-size:1.1rem;color:var(--silver);max-width:680px;margin:24px auto 0;line-height:1.95}
  .conc-stars{display:flex;justify-content:center;gap:6px;margin-top:34px}
  .conc-stars svg{width:22px;height:22px;fill:var(--silver-dim);opacity:.5}

  /* ---------- Footer ---------- */
  footer{background:#050505;padding:50px 0 30px;border-top:1px solid var(--line)}
  .foot-grid{display:flex;justify-content:space-between;align-items:center;flex-wrap:wrap;gap:20px}
  .foot-brand{display:flex;align-items:center;gap:12px}
  .foot-brand b{font-family:'Rajdhani',sans-serif;font-weight:700;letter-spacing:.1em;color:var(--white);font-size:15px}
  .foot-brand small{color:var(--silver-dim);font-size:12px}
  .foot-note{color:var(--silver-dim);font-size:12.5px;text-align:left;line-height:1.7}
  .foot-note a{color:var(--red-bright)}
  .foot-copy{color:var(--silver-dim);font-size:12px;letter-spacing:.04em;border-top:1px solid var(--line);margin-top:24px;padding-top:20px;text-align:center}

  /* ---------- Reveal animation ---------- */
  .reveal{opacity:0;transform:translateY(36px);transition:opacity .9s var(--ease),transform .9s var(--ease)}
  .reveal.visible{opacity:1;transform:none}
  .reveal.d1{transition-delay:.12s}
  .reveal.d2{transition-delay:.24s}
  .reveal.d3{transition-delay:.36s}
  .reveal.d4{transition-delay:.48s}

  /* ---------- Responsive ---------- */
  @media (max-width:980px){
    .history-grid,.gen-block,.perf-layout,.int-layout{grid-template-columns:1fr;gap:34px}
    .gen-block.flip .gen-media{order:0}
    .stat-grid{grid-template-columns:repeat(2,1fr)}
    .feat-row{grid-template-columns:1fr}
    .ext-grid{grid-template-columns:repeat(2,1fr)}
    .int-strip{grid-template-columns:1fr 1fr}
    .gallery-grid{grid-template-columns:repeat(3,1fr)}
    section{padding:70px 0}
  }
  @media (max-width:680px){
    .menu{
      position:fixed;top:0;right:-100%;height:100vh;width:78%;max-width:320px;
      flex-direction:column;align-items:flex-start;justify-content:flex-start;gap:4px;
      background:rgba(7,7,7,.97);backdrop-filter:blur(16px);padding:90px 24px 24px;
      transition:right .4s var(--ease);box-shadow:-20px 0 60px rgba(0,0,0,.6);z-index:999;
    }
    .menu.open{right:0}
    .menu a{width:100%;padding:14px 16px;font-size:15px;border-bottom:1px solid var(--line);border-radius:0}
    .menu a.active::after{display:none}
    .nav-cta{display:none}
    .burger{display:flex;z-index:1001}
    .ext-grid{grid-template-columns:1fr}
    .int-strip{grid-template-columns:1fr}
    .gallery-grid{grid-template-columns:repeat(2,1fr);gap:10px}
    .gitem.wide{grid-column:span 2}
    .gitem.tall{grid-row:span 1}
    .gen-specs{grid-template-columns:repeat(3,1fr)}
    .timeline-mini .t{padding:12px 6px}
    .timeline-mini .g{font-size:11px}
    .hero-content{padding-top:80px}
    .lb-nav.prev{right:10px}
    .lb-nav.next{left:10px}
    .foot-grid{flex-direction:column;text-align:center}
    .foot-note{text-align:center}
  }
  @media (max-width:420px){
    .stat-grid{grid-template-columns:1fr 1fr}
    .gen-specs{grid-template-columns:1fr 1fr 1fr}
    .gallery-grid{grid-template-columns:1fr}
    .gitem.wide{grid-column:span 1}
  }
</style>
</head>
<body>

<!-- ============ HEADER ============ -->
<header id="header">
  <div class="wrap nav">
    <a href="#hero" class="brand" aria-label="Mercedes-AMG">
      <span class="brand-star">
        <svg viewBox="0 0 24 24"><path d="M12 2l2.4 7.6L22 12l-7.6 2.4L12 22l-2.4-7.6L2 12l7.6-2.4z"/></svg>
      </span>
      <span class="brand-txt"><b>MERCEDES-AMG</b><small>E63 · THE LEGEND</small></span>
    </a>
    <nav class="menu" id="menu">
      <a href="#hero">الرئيسية</a>
      <a href="#history">التاريخ</a>
      <a href="#generations">الأجيال</a>
      <a href="#performance">الأداء والمحرك</a>
      <a href="#exterior">التصميم الخارجي</a>
      <a href="#interior">التصميم الداخلي</a>
      <a href="#gallery">المعرض</a>
    </nav>
    <a href="#conclusion" class="nav-cta lat">EXPLORE</a>
    <div class="burger" id="burger" aria-label="القائمة"><span></span><span></span><span></span></div>
  </div>
</header>

<!-- ============ HERO ============ -->
<section class="hero" id="hero">
  <div class="hero-bg"></div>
  <div class="hero-grid"></div>
  <div class="wrap hero-content">
    <span class="eyebrow reveal"><span class="dot"></span> MERCEDES-AMG · E-CLASS · PERFORMANCE SALOON</span>
    <h1 class="reveal d1">
      <span class="lat-name">Mercedes-AMG <span class="accent">E63</span></span>
      قوةٌ تُورِث الأساطير
    </h1>
    <p class="hero-tagline reveal d2">More Than Power. <em>It's a Legacy.</em></p>
    <p class="hero-sub reveal d3">من انطلاقة الجيل W211 عام 2006 بمحرك V8 سعة 6.2 لتر، مروراً بتطور التيربو المزدوج، وصولاً إلى W213 بنظام AMG 4MATIC+ — رحلة سيارةٍ أعادت تعريف مفهوم الصالون الرياضي الفاخر.</p>
    <div class="hero-btns reveal d4">
      <a href="#history" class="btn-primary lat">EXPLORE THE LEGEND <svg viewBox="0 0 24 24"><path d="M5 12h14M13 6l6 6-6 6" fill="none" stroke="#fff" stroke-width="2.4" stroke-linecap="round" stroke-linejoin="round"/></svg></a>
      <a href="#gallery" class="btn-ghost lat">VIEW GALLERY</a>
    </div>
  </div>
  <div class="scroll-cue lat"><span class="mouse"></span>SCROLL</div>
</section>

<!-- ============ HISTORY ============ -->
<section id="history">
  <div class="wrap">
    <div class="sec-head reveal">
      <span class="sec-kicker">OUR STORY · التاريخ</span>
      <h2 class="sec-title">قصةُ اسمٍ صارَ تُراثاً<span class="lat">The Story of E63 AMG</span></h2>
    </div>
    <div class="history-grid">
      <div class="history-text reveal">
        <h3>من الاسم إلى الأسطورة</h3>
        <p>وُلِد اسم <strong>E63</strong> عام <span class="red">2006</span> حين قرّرت AMG استبدال محرك E55 السابق فائق الشحن بمحركٍ جديد بالكامل طبيعي التنفّس سعة <strong>6.2 لتر</strong> من تصميم AMG (M156). لم تكن التسمية مجرد رقم، بل إعلانٌ عن فلسفةٍ جديدة: قوةٌ عالية النقاء منخرطٌ من دون تيربو، بصوتٍ صار توقيعاً صوتياً للماركة.</p>
        <p>توالى التطور عبر الجيل <strong>W212</strong>، حيث قدّمت AMG أول محرك V8 مُزوّد بتيربوين سعة <strong>5.5 لتر</strong> (M157)، رافعاً عزم الدوران إلى مستوياتٍ غير مسبوقة، ثم أطلقت نسخة <strong>S</strong> الأكثر قوةً. وبلغت الرحلة ذروتها في الجيل <strong>W213</strong> بمحرك <strong>4.0 لتر V8 بتيربوين</strong> (M177) ونظام الدفع الرباعي الذكي <span class="red">AMG 4MATIC+</span> مع وضع الانجراف (Drift Mode).</p>
        <p>على مدى ما يزيد عن <strong>17 عاماً</strong> وأجيالٍ ثلاثة، صارت E63 المرجعَ الذي تُقاس عليه سيارات الصالون الرياضية الفاخرة في العالم: توازنٌ بين فخامة الفئة E وغضب قسم AMG، بين راحةِ الرحلات الطويلة وقدرةِ حلبة السباق.</p>
        <div class="timeline-mini lat">
          <div class="t"><div class="y">2006</div><div class="g">W211 · 6.2 V8</div></div>
          <div class="t"><div class="y">2009</div><div class="g">W212 · 5.5 BiTurbo</div></div>
          <div class="t"><div class="y">2017</div><div class="g">W213 · 4.0 BiTurbo</div></div>
          <div class="t"><div class="y">2023</div><div class="g">نهاية الحقبة</div></div>
        </div>
      </div>
      <div class="history-img reveal d2">
        <span class="history-badge lat">SINCE 2006</span>
        <img src="https://z-cdn.chatglm.cn/image-search-mcp/images-ppt/c0fc6f45bbf3.jpg" alt="Mercedes-AMG E63 أمامية بإضاءة درامية" loading="lazy">
      </div>
    </div>
  </div>
</section>

<!-- ============ GENERATIONS ============ -->
<section id="generations">
  <div class="wrap">
    <div class="sec-head reveal">
      <span class="sec-kicker">GENERATIONS · الأجيال</span>
      <h2 class="sec-title">ثلاثة أجيالٍ، إرثٌ واحد<span class="lat">The Evolution of E63</span></h2>
      <p class="sec-lead">كل جيلٍ كان قفزةً نوعية: من التنفّس الطبيعي إلى التيربو المزدوج، ومن الدفع الخلفي إلى 4MATIC+ الذكي. تالياً المواصفات الرسمية لكل جيل وفترة إنتاجه.</p>
    </div>

    <!-- W211 -->
    <div class="gen-block reveal">
      <div class="gen-media">
        <span class="gen-year-tag lat">2006 — 2009</span>
        <img src="https://z-cdn.chatglm.cn/image-search-mcp/images-ppt/59fe1d988e68.jpg" alt="Mercedes-AMG E63 W211" loading="lazy">
      </div>
      <div class="gen-info">
        <div class="gen-code lat">W211 <span>E63</span></div>
        <div class="gen-period lat">PRODUCTION · 2006 – 2009</div>
        <p class="gen-engine">محرك <b>6.2 لتر V8</b> طبيعي التنفّس (M156)</p>
        <p class="desc">الجيل الذي وَلَدَ اسم E63. محركٌ صُمّم وصُنِّع يدوياً وفق فلسفة "رجلٌ واحد، محركٌ واحد" (One Man, One Engine)، بصوتٍ عاصفٍ وبساطٍ هادئ. قدّم أداءً فائق النقاء في زمنٍ كانت فيه التيربو نادرةً في هذه الفئة، وثبّت مكانة AMG كصانعةِ محركات طبيعية التنفّس من الطراز الرفيع.</p>
        <div class="gen-specs">
          <div class="sp"><div class="v">507<small>hp</small></div><div class="l">القدرة</div></div>
          <div class="sp"><div class="v">630<small>Nm</small></div><div class="l">العزم</div></div>
          <div class="sp"><div class="v">4.5<small>s</small></div><div class="l">0-100 كم/س</div></div>
        </div>
      </div>
    </div>

    <!-- W212 -->
    <div class="gen-block flip reveal">
      <div class="gen-media">
        <span class="gen-year-tag lat">2009 — 2016</span>
        <img src="https://z-cdn.chatglm.cn/image-search-mcp/images-ppt/2c1b5c3df646.jpg" alt="Mercedes-AMG E63 W212" loading="lazy">
      </div>
      <div class="gen-info">
        <div class="gen-code lat">W212 <span>E63</span></div>
        <div class="gen-period lat">PRODUCTION · 2009 – 2016</div>
        <p class="gen-engine">محرك <b>5.5 لتر V8 بتيربوين</b> (M157) — نسخة S</p>
        <p class="desc">الجيل الذي نقل E63 إلى عصر التيربو المزدوج. خفّضت AMG السعة ورفعت القوة والعزم بشكلٍ جذري بفضل التيربوين، وطرحت نسخة <b>S</b> الأعلى أداءً. كما قدّمت ناقل الحركة الرياضية AMG SPEEDSHIFT MCT، ومكابحَ أكبر، وهيكلَ سعرٍ أكثر صلابةً للتحكّم الأمثل.</p>
        <div class="gen-specs">
          <div class="sp"><div class="v">577<small>hp</small></div><div class="l">القدرة (S)</div></div>
          <div class="sp"><div class="v">800<small>Nm</small></div><div class="l">العزم (S)</div></div>
          <div class="sp"><div class="v">3.6<small>s</small></div><div class="l">0-100 كم/س</div></div>
        </div>
      </div>
    </div>

    <!-- W213 -->
    <div class="gen-block reveal">
      <div class="gen-media">
        <span class="gen-year-tag lat">2017 — 2023</span>
        <img src="https://z-cdn.chatglm.cn/image-search-mcp/images-ppt/26bd1d88c7c5.jpg" alt="Mercedes-AMG E63 S W213" loading="lazy">
      </div>
      <div class="gen-info">
        <div class="gen-code lat">W213 <span>E63</span></div>
        <div class="gen-period lat">PRODUCTION · 2017 – 2023</div>
        <p class="gen-engine">محرك <b>4.0 لتر V8 بتيربوين</b> (M177) — نسخة S</p>
        <p class="desc">ذروة التطور: محركٌ مُحمّلٌ بالكامل داخل الـV، نظام الدفع الرباعي الذكي <b>AMG 4MATIC+</b> القابل للتحويل بالكامل إلى دفعٍ خلفي عبر وضع الانجراف، وناقل حركة رياضي 9 سرعات. صارت E63 بهذا الجيل قادرةً على منافسة السيارات الخارقة (Supercars) في التسارع، مع احتفاظها بهوية الصالون الفاخر.</p>
        <div class="gen-specs">
          <div class="sp"><div class="v">603<small>hp</small></div><div class="l">القدرة (S)</div></div>
          <div class="sp"><div class="v">850<small>Nm</small></div><div class="l">العزم (S)</div></div>
          <div class="sp"><div class="v">3.3<small>s</small></div><div class="l">0-100 كم/س</div></div>
        </div>
      </div>
    </div>
  </div>
</section>

<!-- ============ PERFORMANCE ============ -->
<section id="performance">
  <div class="wrap">
    <div class="sec-head reveal">
      <span class="sec-kicker">PERFORMANCE · الأداء</span>
      <h2 class="sec-title">هندسةُ الغضب المنضبط<span class="lat">Powertrain &amp; Dynamics</span></h2>
    </div>

    <div class="perf-layout">
      <div class="perf-img reveal">
        <img src="https://z-cdn.chatglm.cn/image-search-mcp/images-ppt/c08d59e8cc3e.jpg" alt="محرك AMG 4.0L V8 Biturbo M177" loading="lazy">
        <span class="live-tag lat">M177 · HAND-BUILT</span>
      </div>
      <div class="perf-text reveal d2">
        <h3>محركٌ يُصنع يدوياً، نظامٌ يفكّر بسرعةِ ومضة</h3>
        <p>في قلب E63 S ينبض محرك <b>M177</b>: V8 سعة 4.0 لتر بتيربوين موضوعين داخل زاوية الـV (inside the V) لتقليل التأخير (turbo lag) إلى الحدّ الأدنى. يُجمَّع كل محركٍ يدوياً وفق مبدأ AMG العريق <span class="red">"رجلٌ واحد، محركٌ واحد"</span>، ويوقّع عليه المهندس المسؤول — شهادةٌ على المسؤولية الفردية في دقة الصناعة.</p>
        <p>ينقل القوة ناقل الحركة الرياضي <b>AMG SPEEDSHIFT MCT 9G</b> بتسعة نسبٍ، مزوّد بقابضٍ متعدد الأقراص رطبٍ يتيح تبديلاً فائقاً للسرعة دون انقطاع العزم. ويُدار كل ذلك عبر نظام الدفع الذكي <b>AMG 4MATIC+</b> المتغيّر باستمرار، القادر على توزيع العزم بين المحورين أو تحويله بالكامل إلى الخلف.</p>
      </div>
    </div>

    <div class="stat-grid reveal">
      <div class="stat-card"><div class="num" data-target="612"><small>+</small>0</div><div class="lab">حصاناً (E63 S)</div></div>
      <div class="stat-card"><div class="num" data-target="850"><small>Nm</small>0</div><div class="lab">عزم الدوران</div></div>
      <div class="stat-card"><div class="num" data-target="3.3" data-decimal="1"><small>s</small>0.0</div><div class="lab">0 إلى 100 كم/س</div></div>
      <div class="stat-card"><div class="num" data-target="300"><small>km/h</small>0</div><div class="lab">سرعة قصوى (مع باقة السائق)</div></div>
    </div>

    <div class="feat-row">
      <div class="feat-card reveal">
        <div class="ico"><svg viewBox="0 0 24 24"><path d="M12 2l3 7h7l-5.5 4.5L18 21l-6-4-6 4 1.5-7.5L2 9h7z"/></svg></div>
        <h4>AMG 4MATIC+ <span class="lat" style="font-size:.7em;color:var(--silver-dim)">Variable AWD</span></h4>
        <p>نظام دفعٍ رباعيٍّ ذكيٌّ قابل للتغيير بالكامل، يوزّع العزم باستمرار بين المحورين، ويتيح وضع الانجراف (Drift Mode) بتحويل القوة بالكامل إلى العجلات الخلفية.</p>
      </div>
      <div class="feat-card reveal d1">
        <div class="ico"><svg viewBox="0 0 24 24"><path d="M5 4h14v3H5zm0 5h14v3H5zm0 5h14v3H5zm2 4h10v2H7z"/></svg></div>
        <h4>AMG SPEEDSHIFT MCT <span class="lat" style="font-size:.7em;color:var(--silver-dim)">9-Speed</span></h4>
        <p>ناقل حركةٍ رياضي بتسعة نسبٍ مع قابضٍ متعدد الأقراص رطب، يبدّل في أجزاءٍ من الثانية دون انقطاع العزم، مع وضع Sport+ للتبديل الأكثر هجوميةً.</p>
      </div>
      <div class="feat-card reveal d2">
        <div class="ico"><svg viewBox="0 0 24 24"><path d="M3 18v-6a4 4 0 014-4h10a4 4 0 014 4v6h-3v-2H6v2H3zm3-7v3h12v-3H6z"/></svg></div>
        <h4>AMG RIDE CONTROL+ <span class="lat" style="font-size:.7em;color:var(--silver-dim)">Adaptive Suspension</span></h4>
        <p>تعليقٌ هوائيٌّ متكيّفٌ متعدد الحجرات، مع تحكّمٍ مستمرٍّ في مُخمّدات الصدمات الكهرومغناطيسية، يوازن بين ثبات الحلبة وراحة السفر.</p>
      </div>
    </div>
  </div>
</section>

<!-- ============ EXTERIOR ============ -->
<section id="exterior">
  <div class="wrap">
    <div class="sec-head reveal">
      <span class="sec-kicker">DESIGN · التصميم الخارجي</span>
      <h2 class="sec-title">حضورٌ لا يُخطئه النظر<span class="lat">Exterior Design</span></h2>
    </div>

    <div class="ext-hero reveal">
      <img src="https://z-cdn.chatglm.cn/image-search-mcp/images-ppt/dac8c59537f8.jpg" alt="Mercedes-AMG E63 الواجهة الأمامية" loading="lazy">
      <div class="cap">
        <h3>كل تفصيلةٍ تخدم الأداء</h3>
        <p>ليست مجرد خطوطٍ جميلة، بل فوهاتٌ هوائية أوسع، وتوزيعٌ دقيقٌ للكتلة، وتمريرٌ مدروسٌ للهواء.</p>
      </div>
    </div>

    <div class="ext-grid">
      <div class="ext-card reveal">
        <div class="img"><img src="https://z-cdn.chatglm.cn/image-search-mcp/images-ppt/503060960e24.png" alt="الشبك الأمامي Panamericana" loading="lazy"></div>
        <div class="body">
          <h4><span class="lat">01</span>الشبك الأمامي</h4>
          <p>شبك AMG Panamericana بأعمدةٍ عمودية فضية، توقيعٌ بصريٌّ يعكس هوية قسم الأداء، ويتوسّطه نجمة الثلاث نقاط فاخرة.</p>
        </div>
      </div>
      <div class="ext-card reveal d1">
        <div class="img"><img src="https://z-cdn.chatglm.cn/image-search-mcp/images-ppt/64c223413ef8.jpg" alt="المصابيح الأمامية LED Multibeam" loading="lazy"></div>
        <div class="body">
          <h4><span class="lat">02</span>المصابيح الأمامية</h4>
          <p>مصابيح LED MULTIBEAM / Digital Light التكيّفية، بإضاءةٍ ديناميكية تتبع مسار الطريق، وتوقيعٍ نهاريٍّ مميّز.</p>
        </div>
      </div>
      <div class="ext-card reveal d2">
        <div class="img"><img src="https://z-cdn.chatglm.cn/image-search-mcp/images-ppt/bf78b699f017.jpg" alt="الجنوط الرياضية والعادم الرباعي" loading="lazy"></div>
        <div class="body">
          <h4><span class="lat">03</span>الجنوط والعادم</h4>
          <p>جنوطُ AMG مسبوكةٌ خفيفة التصميمات المتعددة، وعادمٌ رباعيٌّ بفتحاتٍ شبه منحرفة يصدح بصوت V8 المميّز.</p>
        </div>
      </div>
    </div>
  </div>
</section>

<!-- ============ INTERIOR ============ -->
<section id="interior">
  <div class="wrap">
    <div class="sec-head reveal">
      <span class="sec-kicker">CABIN · التصميم الداخلي</span>
      <h2 class="sec-title">مقصورةٌ بين الحلبةِ والقمة<span class="lat">Interior &amp; Craftsmanship</span></h2>
    </div>

    <div class="int-layout">
      <div class="int-main reveal">
        <img src="https://z-cdn.chatglm.cn/image-search-mcp/images-ppt/539f72760692.jpg" alt="مقصورة Mercedes-AMG E63 الداخلية" loading="lazy">
      </div>
      <div class="int-text reveal d2">
        <h3>حيث تلتقي الفخامةُ بالغرضية</h3>
        <p>داخل E63 تجد مقصورةً صُمّمت لتكون امتداداً للسائق: خاماتٌ فاخرة، تقنيةٌ محيطة، وعناصرُ تُلمّس بها روح AMG في كل لمسة. توازنٌ نادرٌ بين الراحةِ في الرحلات الطويلة والإحساسِ الرياضي في الحلبة.</p>
        <ul class="int-list">
          <li><span class="mk lat">A</span><span class="ct"><b>مقاعد AMG الرياضية</b><span>بجلد Nappa و DINAMICA، بتدفئةٍ وتبريدٍ وتثبيتٍ جانبيٍّ متعدد المستويات.</span></span></li>
          <li><span class="mk lat">B</span><span class="ct"><b>مقود AMG Performance</b><span>مكسوٌّ بـ DINAMICA، يضمّ وحدة التحكّم بالأنماط وأزرار الدوّارات مباشرةً.</span></span></li>
          <li><span class="mk lat">C</span><span class="ct"><b>شاشتا القيادة الواسعتان</b><span>اثنتان مقاس 12.3 بوصة بتصميمٍ متّصل، مع عرض AMG الخاص بمؤشرات الأداء.</span></span></li>
          <li><span class="mk lat">D</span><span class="ct"><b>الخامات الكربونية</b><span>تطعيماتٌ من ألياف الكربون اللامع والمطفأ، وعتباتُ أبواب AMG مضيئة.</span></span></li>
        </ul>
      </div>
    </div>

    <div class="int-strip reveal">
      <div class="ph"><img src="https://z-cdn.chatglm.cn/image-search-mcp/images-ppt/7f0cba029010.jpg" alt="مقود AMG وأزرار التحكم" loading="lazy"></div>
      <div class="ph"><img src="https://z-cdn.chatglm.cn/image-search-mcp/images-ppt/95155689a47e.jpg" alt="شاشات القيادة في E63" loading="lazy"></div>
    </div>
  </div>
</section>

<!-- ============ GALLERY ============ -->
<section id="gallery">
  <div class="wrap">
    <div class="sec-head reveal">
      <span class="sec-kicker">GALLERY · المعرض</span>
      <h2 class="sec-title">معرضُ الأسطورة<span class="lat">A Visual Tribute</span></h2>
      <p class="sec-lead">مجموعةٌ من الصور عالية الجودة لأجيال E63 — انقر أي صورةٍ لمشاهدتها بحجمٍ أكبر.</p>
    </div>

    <div class="gallery-grid reveal" id="galleryGrid">
      <div class="gitem wide" data-full="https://z-cdn.chatglm.cn/image-search-mcp/images-ppt/9d4579bbefcb.jpg">
        <img src="https://z-cdn.chatglm.cn/image-search-mcp/images-ppt/9d4579bbefcb.jpg" alt="E63 على الطريق" loading="lazy">
        <span class="zoom"><svg viewBox="0 0 24 24"><path d="M15 3h6v6M21 3l-7 7M9 21H3v-6M3 21l7-7"/></svg></span>
        <span class="gl-label lat">ON THE ROAD</span>
      </div>
      <div class="gitem" data-full="https://z-cdn.chatglm.cn/image-search-mcp/images-ppt/b20b0a412eb2.jpg">
        <img src="https://z-cdn.chatglm.cn/image-search-mcp/images-ppt/b20b0a412eb2.jpg" alt="E63 في الحركة" loading="lazy">
        <span class="zoom"><svg viewBox="0 0 24 24"><path d="M15 3h6v6M21 3l-7 7M9 21H3v-6M3 21l7-7"/></svg></span>
        <span class="gl-label lat">MOTION</span>
      </div>
      <div class="gitem tall" data-full="https://z-cdn.chatglm.cn/image-search-mcp/images-ppt/7a27531c768b.jpg">
        <img src="https://z-cdn.chatglm.cn/image-search-mcp/images-ppt/7a27531c768b.jpg" alt="E63 تفاصيل" loading="lazy">
        <span class="zoom"><svg viewBox="0 0 24 24"><path d="M15 3h6v6M21 3l-7 7M9 21H3v-6M3 21l7-7"/></svg></span>
        <span class="gl-label lat">DETAIL</span>
      </div>
      <div class="gitem" data-full="https://z-cdn.chatglm.cn/image-search-mcp/images-ppt/dcfed0968adf.jpg">
        <img src="https://z-cdn.chatglm.cn/image-search-mcp/images-ppt/dcfed0968adf.jpg" alt="E63 أمامية" loading="lazy">
        <span class="zoom"><svg viewBox="0 0 24 24"><path d="M15 3h6v6M21 3l-7 7M9 21H3v-6M3 21l7-7"/></svg></span>
        <span class="gl-label lat">FRONT</span>
      </div>
      <div class="gitem" data-full="https://z-cdn.chatglm.cn/image-search-mcp/images-ppt/11c7c2279362.jpg">
        <img src="https://z-cdn.chatglm.cn/image-search-mcp/images-ppt/11c7c2279362.jpg" alt="E63 جانبية" loading="lazy">
        <span class="zoom"><svg viewBox="0 0 24 24"><path d="M15 3h6v6M21 3l-7 7M9 21H3v-6M3 21l7-7"/></svg></span>
        <span class="gl-label lat">PROFILE</span>
      </div>
      <div class="gitem wide" data-full="https://z-cdn.chatglm.cn/image-search-mcp/images-ppt/cdae68b14373.jpg">
        <img src="https://z-cdn.chatglm.cn/image-search-mcp/images-ppt/cdae68b14373.jpg" alt="E63 S W213" loading="lazy">
        <span class="zoom"><svg viewBox="0 0 24 24"><path d="M15 3h6v6M21 3l-7 7M9 21H3v-6M3 21l7-7"/></svg></span>
        <span class="gl-label lat">E63 S · W213</span>
      </div>
      <div class="gitem" data-full="https://z-cdn.chatglm.cn/image-search-mcp/images-ppt/f2d3c213d23b.jpeg">
        <img src="https://z-cdn.chatglm.cn/image-search-mcp/images-ppt/f2d3c213d23b.jpeg" alt="E63 W211" loading="lazy">
        <span class="zoom"><svg viewBox="0 0 24 24"><path d="M15 3h6v6M21 3l-7 7M9 21H3v-6M3 21l7-7"/></svg></span>
        <span class="gl-label lat">W211</span>
      </div>
      <div class="gitem" data-full="https://z-cdn.chatglm.cn/image-search-mcp/images-ppt/181875fbfb36.jpg">
        <img src="https://z-cdn.chatglm.cn/image-search-mcp/images-ppt/181875fbfb36.jpg" alt="E63 W212" loading="lazy">
        <span class="zoom"><svg viewBox="0 0 24 24"><path d="M15 3h6v6M21 3l-7 7M9 21H3v-6M3 21l7-7"/></svg></span>
        <span class="gl-label lat">W212</span>
      </div>
      <div class="gitem" data-full="https://z-cdn.chatglm.cn/image-search-mcp/images-ppt/fe9db9c9fe55.jpg">
        <img src="https://z-cdn.chatglm.cn/image-search-mcp/images-ppt/fe9db9c9fe55.jpg" alt="E63 خلفية وعادم" loading="lazy">
        <span class="zoom"><svg viewBox="0 0 24 24"><path d="M15 3h6v6M21 3l-7 7M9 21H3v-6M3 21l7-7"/></svg></span>
        <span class="gl-label lat">REAR</span>
      </div>
      <div class="gitem" data-full="https://z-cdn.chatglm.cn/image-search-mcp/images-ppt/5033482b2f78.jpg">
        <img src="https://z-cdn.chatglm.cn/image-search-mcp/images-ppt/5033482b2f78.jpg" alt="E63 في الحلبة" loading="lazy">
        <span class="zoom"><svg viewBox="0 0 24 24"><path d="M15 3h6v6M21 3l-7 7M9 21H3v-6M3 21l7-7"/></svg></span>
        <span class="gl-label lat">TRACK</span>
      </div>
    </div>
  </div>
</section>

<!-- ============ CONCLUSION ============ -->
<section id="conclusion">
  <div class="wrap">
    <div class="conc-line reveal"></div>
    <h2 class="conc-title reveal d1">Mercedes-AMG E63 <span class="red">— A Legend That Never Fades.</span></h2>
    <p class="conc-sub reveal d2">من انطلاقتها الأولى عام 2006 حتى نهاية حقبتها، لم تكتفِ E63 بأن تكون سيارةً سريعة، بل صارت معياراً تُقاس عليه سيارات الصالون الرياضية الفاخرة. إرثٌ من المحركات الطبيعية التنفّس، مرّ بالتيربو المزدوج، وبلغ ذروته بدفعٍ ذكيٍّ رباعي. اسمٌ لن يُنسى في تاريخ صناعة السيارات.</p>
    <div class="conc-stars reveal d3">
      <svg viewBox="0 0 24 24"><path d="M12 2l2.4 7.6L22 12l-7.6 2.4L12 22l-2.4-7.6L2 12l7.6-2.4z"/></svg>
      <svg viewBox="0 0 24 24"><path d="M12 2l2.4 7.6L22 12l-7.6 2.4L12 22l-2.4-7.6L2 12l7.6-2.4z"/></svg>
      <svg viewBox="0 0 24 24"><path d="M12 2l2.4 7.6L22 12l-7.6 2.4L12 22l-2.4-7.6L2 12l7.6-2.4z"/></svg>
    </div>
  </div>
</section>

<!-- ============ FOOTER ============ -->
<footer>
  <div class="wrap">
    <div class="foot-grid">
      <div class="foot-brand">
        <span class="brand-star"><svg viewBox="0 0 24 24"><path d="M12 2l2.4 7.6L22 12l-7.6 2.4L12 22l-2.4-7.6L2 12l7.6-2.4z"/></svg></span>
        <span><b>MERCEDES-AMG E63</b><br><small>THE POWER OF A LEGEND</small></span>
      </div>
      <div class="foot-note">
        موقعٌ تعريفيٌّ مستقلٌّ يحتفي بتاريخ سيارة Mercedes-AMG E63.<br>
        المصدر التاريخي والمواصفات: <a href="https://www.mercedes-amg.com" target="_blank" rel="noopener">Mercedes-Benz Media / Mercedes-AMG الرسمي</a>.<br>
        جميع العلامات التجارية ملكٌ لأصحابها. الصور لأغراض العرض التوثيقي.
      </div>
    </div>
    <div class="foot-copy lat">© 2026 · MERCEDES-AMG E63 — A LEGEND THAT NEVER FADES</div>
  </div>
</footer>

<!-- ============ LIGHTBOX ============ -->
<div class="lightbox" id="lightbox" aria-hidden="true">
  <button class="lb-close" id="lbClose" aria-label="إغلاق">&times;</button>
  <button class="lb-nav prev" id="lbPrev" aria-label="السابق"><svg viewBox="0 0 24 24"><path d="M15 6l-6 6 6 6" fill="none" stroke="#fff" stroke-width="2.4" stroke-linecap="round" stroke-linejoin="round"/></svg></button>
  <img id="lbImg" src="" alt="معاينة">
  <button class="lb-nav next" id="lbNext" aria-label="التالي"><svg viewBox="0 0 24 24"><path d="M9 6l6 6-6 6" fill="none" stroke="#fff" stroke-width="2.4" stroke-linecap="round" stroke-linejoin="round"/></svg></button>
  <div class="lb-counter lat" id="lbCounter">01 / 10</div>
</div>

<script>
(function(){
  "use strict";

  /* ---- Header scroll state ---- */
  var header = document.getElementById('header');
  function onScroll(){
    if(window.scrollY > 60){ header.classList.add('scrolled'); }
    else{ header.classList.remove('scrolled'); }
  }
  window.addEventListener('scroll', onScroll, {passive:true});
  onScroll();

  /* ---- Mobile menu ---- */
  var burger = document.getElementById('burger');
  var menu = document.getElementById('menu');
  burger.addEventListener('click', function(){
    burger.classList.toggle('active');
    menu.classList.toggle('open');
  });
  menu.querySelectorAll('a').forEach(function(a){
    a.addEventListener('click', function(){
      burger.classList.remove('active');
      menu.classList.remove('open');
    });
  });

  /* ---- Active nav on scroll (IntersectionObserver) ---- */
  var sections = document.querySelectorAll('section[id]');
  var navLinks = menu.querySelectorAll('a');
  var navMap = {};
  navLinks.forEach(function(a){ navMap[a.getAttribute('href').slice(1)] = a; });
  var spyObs = new IntersectionObserver(function(entries){
    entries.forEach(function(e){
      if(e.isIntersecting){
        navLinks.forEach(function(a){ a.classList.remove('active'); });
        if(navMap[e.target.id]){ navMap[e.target.id].classList.add('active'); }
      }
    });
  }, {rootMargin:'-45% 0px -50% 0px', threshold:0});
  sections.forEach(function(s){ spyObs.observe(s); });

  /* ---- Reveal on scroll ---- */
  var revealEls = document.querySelectorAll('.reveal');
  var revObs = new IntersectionObserver(function(entries){
    entries.forEach(function(e){
      if(e.isIntersecting){
        e.target.classList.add('visible');
        revObs.unobserve(e.target);
      }
    });
  }, {threshold:0.12, rootMargin:'0px 0px -8% 0px'});
  revealEls.forEach(function(el){ revObs.observe(el); });

  /* ---- Animated counters ---- */
  function animateCount(el){
    var target = parseFloat(el.getAttribute('data-target'));
    var decimal = parseInt(el.getAttribute('data-decimal')||'0',10);
    var suffixEl = el.querySelector('small');
    var suffixText = suffixEl ? suffixEl.textContent : '';
    var start = 0, dur = 1600, t0 = null;
    function fmt(v){ return decimal>0 ? v.toFixed(decimal) : Math.round(v).toString(); }
    function render(v){ el.innerHTML = fmt(v) + (suffixText ? '<small>'+suffixText+'</small>' : ''); }
    function step(ts){
      if(!t0) t0 = ts;
      var p = Math.min((ts - t0)/dur, 1);
      var eased = 1 - Math.pow(1 - p, 3);
      render(start + (target - start)*eased);
      if(p < 1){ requestAnimationFrame(step); }
      else { render(target); }
    }
    requestAnimationFrame(step);
  }
  var statObs = new IntersectionObserver(function(entries){
    entries.forEach(function(e){
      if(e.isIntersecting){
        animateCount(e.target);
        statObs.unobserve(e.target);
      }
    });
  }, {threshold:0.5});
  document.querySelectorAll('.stat-card .num[data-target]').forEach(function(el){ statObs.observe(el); });

  /* ---- Lightbox gallery ---- */
  var items = Array.prototype.slice.call(document.querySelectorAll('.gitem'));
  var lb = document.getElementById('lightbox');
  var lbImg = document.getElementById('lbImg');
  var lbCounter = document.getElementById('lbCounter');
  var current = 0;

  function openLb(i){
    current = i;
    var full = items[i].getAttribute('data-full');
    lbImg.src = full;
    lbCounter.textContent = String(i+1).padStart(2,'0') + ' / ' + String(items.length).padStart(2,'0');
    lb.classList.add('open');
    lb.setAttribute('aria-hidden','false');
    document.body.style.overflow = 'hidden';
  }
  function closeLb(){
    lb.classList.remove('open');
    lb.setAttribute('aria-hidden','true');
    document.body.style.overflow = '';
  }
  function nav(dir){
    current = (current + dir + items.length) % items.length;
    openLb(current);
  }
  items.forEach(function(it, i){
    it.addEventListener('click', function(){ openLb(i); });
  });
  document.getElementById('lbClose').addEventListener('click', closeLb);
  document.getElementById('lbPrev').addEventListener('click', function(){ nav(-1); });
  document.getElementById('lbNext').addEventListener('click', function(){ nav(1); });
  lb.addEventListener('click', function(e){ if(e.target === lb){ closeLb(); } });
  document.addEventListener('keydown', function(e){
    if(!lb.classList.contains('open')) return;
    if(e.key === 'Escape') closeLb();
    else if(e.key === 'ArrowRight') nav(-1); // RTL: right arrow = previous
    else if(e.key === 'ArrowLeft') nav(1);   // RTL: left arrow = next
  });

  /* ---- Hero subtle parallax ---- */
  var heroBg = document.querySelector('.hero-bg');
  if(heroBg){
    window.addEventListener('scroll', function(){
      var y = window.scrollY;
      if(y < window.innerHeight){
        heroBg.style.transform = 'scale(1.05) translateY(' + (y*0.18) + 'px)';
      }
    }, {passive:true});
  }
})();
</script>
</body>
</html>
