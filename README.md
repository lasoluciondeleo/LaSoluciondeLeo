[index.html](https://github.com/user-attachments/files/32888425/index.html)
<!DOCTYPE html>
<html lang="es">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>La Solución de Leo | Notary Public · Documentos · Impuestos | Sacramento, CA</title>
<meta name="description" content="Servicio móvil de documentos, impuestos y traducciones en el área de Sacramento. Notary Public licenciado y afianzado. Se habla español. Llame o textee: (408) 613-4713">
<!-- Times New Roman is a native system font — no web font needed -->
<style>
  :root{
    --navy:#16324E;
    --navy-dark:#071322;
    --gold:#C9972E;
    --gold-light:#F3D276;
    --cream:#F5EFE0;
    --charcoal:#24272B;
    --muted:#5B5F63;
    --line:#E4DCC9;
  }
  *{box-sizing:border-box;}
  html{scroll-behavior:smooth;}
  body{
    margin:0;
    font-family:'Times New Roman',Times,Georgia,serif;
    background:var(--cream);
    color:var(--charcoal);
    -webkit-font-smoothing:antialiased;
  }
  a{color:inherit;}
  img,svg{display:block;max-width:100%;}
  .wrap{max-width:1120px;margin:0 auto;padding:0 24px;}
  .eyebrow{
    font-family:'Times New Roman',Times,serif;font-weight:700;letter-spacing:.14em;text-transform:uppercase;
    font-size:14px;color:var(--gold);
  }

  /* ---------- Top bar ---------- */
  .topbar{
    position:sticky;top:0;z-index:50;
    background:var(--navy);
    color:var(--cream);
    border-bottom:3px solid var(--gold);
  }
  .topbar-inner{
    display:flex;align-items:center;justify-content:space-between;
    padding:10px 24px;max-width:1120px;margin:0 auto;
  }
  .brand{display:flex;align-items:center;gap:10px;text-decoration:none;color:var(--cream);}
  .brand svg,.brand img{width:40px;height:40px;flex:none;border-radius:50%;}
  .brand-name{font-family:'Times New Roman',Times,serif;font-weight:700;font-size:16px;line-height:1.15;}
  .brand-name span{display:block;color:var(--gold);font-size:12px;font-weight:600;letter-spacing:.05em;}
  .call-btn{
    background:var(--gold);color:var(--navy-dark);
    font-weight:700;font-size:14px;
    padding:9px 18px;border-radius:999px;text-decoration:none;
    white-space:nowrap;
  }
  .call-btn:hover{background:var(--gold-light);}
  @media (max-width:520px){
    .topbar-inner{padding:9px 14px;gap:8px;}
    .brand svg,.brand img{width:32px;height:32px;}
    .brand-name{font-size:12px;}
    .brand-name span{font-size:10px;}
    .call-btn{font-size:12px;padding:8px 11px;white-space:nowrap;}
  }
  @media (max-width:360px){
    .brand-name span{display:none;}
  }

  /* ---------- Hero ---------- */
  .hero{
    position:relative;
    background:radial-gradient(1100px 500px at 85% -10%, #2a5480 0%, var(--navy) 55%, var(--navy-dark) 100%);
    color:var(--cream);
    padding:74px 0 96px;
    overflow:hidden;
  }
  .hero::after{
    content:"";position:absolute;right:-90px;top:-90px;width:420px;height:420px;
    border:2px solid rgba(214,162,51,.18);border-radius:50%;
  }
  .hero::before{
    content:"";position:absolute;right:-40px;top:-40px;width:300px;height:300px;
    border:2px solid rgba(214,162,51,.14);border-radius:50%;
  }
  .hero-grid{
    display:grid;grid-template-columns:1.15fr .85fr;gap:48px;align-items:center;position:relative;z-index:2;
  }
  @media (max-width:860px){ .hero-grid{grid-template-columns:1fr;} }
  .hero h1{
    font-family:'Times New Roman',Times,serif;
    font-size:clamp(32px,5vw,50px);line-height:1.08;font-weight:800;margin:14px 0 6px;
  }
  .hero h1 em{color:var(--gold);font-style:normal;}
  .hero .sub-en{
    font-size:16px;color:#CBD8E6;margin:0 0 22px;font-weight:500;
  }
  .hero p.lead{font-size:16.5px;color:#E7EDF3;max-width:52ch;margin:0 0 28px;}
  .hero-ctas{display:flex;gap:14px;flex-wrap:wrap;}
  .btn{
    display:inline-flex;align-items:center;gap:8px;
    padding:14px 24px;border-radius:10px;font-weight:700;font-size:15px;text-decoration:none;
  }
  .btn-primary{background:var(--gold);color:var(--navy-dark);}
  .btn-primary:hover{background:var(--gold-light);}
  .btn-ghost{border:1.5px solid rgba(250,246,238,.45);color:var(--cream);}
  .btn-ghost:hover{border-color:var(--gold);color:var(--gold);}

  .hero-badges{display:flex;flex-wrap:wrap;gap:10px;margin-top:30px;}
  .pill{
    font-size:11.5px;font-weight:700;letter-spacing:.03em;
    background:rgba(250,246,238,.08);border:1px solid rgba(214,162,51,.45);
    color:var(--gold-light);padding:7px 12px;border-radius:999px;
  }

  /* seal graphic */
  .seal-wrap{display:flex;justify-content:center;position:relative;}
  .seal-wrap svg,.seal-wrap img{width:min(340px,80%);height:auto;filter:drop-shadow(0 18px 30px rgba(0,0,0,.35));}

  /* ---------- Trust strip ---------- */
  .trust-strip{
    background:var(--gold);color:var(--navy-dark);
    padding:14px 0;
  }
  .trust-strip .wrap{
    display:flex;justify-content:center;gap:34px;flex-wrap:wrap;
    font-weight:700;font-size:13px;letter-spacing:.02em;text-align:center;
  }
  .trust-strip .item{display:flex;align-items:center;gap:7px;}

  /* ---------- Section shell ---------- */
  section{padding:76px 0;}
  .section-head{max-width:640px;margin:0 auto 44px;text-align:center;}
  .section-head h2{font-family:'Times New Roman',Times,serif;font-size:clamp(26px,3.4vw,36px);margin:8px 0 10px;font-weight:800;color:var(--navy);}
  .section-head p{color:var(--muted);font-size:15.5px;margin:0;}

  /* ---------- Services ---------- */
  .services-grid{
    display:grid;grid-template-columns:repeat(auto-fit,minmax(240px,1fr));
    gap:20px;
  }
  .svc-card{
    background:#fff;border:1px solid var(--line);border-radius:14px;
    padding:24px 22px;
  }
  .svc-card .num{
    font-family:'Times New Roman',Times,serif;font-style:italic;color:var(--gold);
    font-size:13px;font-weight:600;margin-bottom:10px;display:block;
  }
  .svc-card h3{font-family:'Times New Roman',Times,serif;margin:0 0 4px;font-size:18px;color:var(--navy);font-weight:700;}
  .svc-card .en{font-size:12px;color:var(--muted);margin:0 0 14px;font-style:italic;}
  .svc-card ul{margin:0;padding:0;list-style:none;}
  .svc-card li{
    font-size:13.7px;padding:7px 0 7px 22px;position:relative;color:var(--charcoal);
    border-top:1px dashed var(--line);
  }
  .svc-card li:first-child{border-top:none;padding-top:0;}
  .svc-card li:before{
    content:"✓";position:absolute;left:0;top:7px;color:var(--gold);font-weight:700;
  }
  .li-en{color:var(--muted);font-size:12px;font-style:italic;}

  .soon-banner{
    margin-top:36px;background:var(--navy);color:var(--cream);
    border-radius:14px;padding:20px 26px;
    display:flex;align-items:center;justify-content:space-between;gap:16px;flex-wrap:wrap;
    border:1px dashed rgba(214,162,51,.5);
  }
  .soon-banner strong{color:var(--gold);display:block;font-size:15px;}
  .soon-banner span{font-size:12.5px;color:#CBD8E6;}

  /* ---------- Why us ---------- */
  .why{background:var(--navy);color:var(--cream);}
  .why .section-head h2{color:#fff;}
  .why .section-head p{color:#C7D3E0;}
  .why-grid{display:grid;grid-template-columns:repeat(auto-fit,minmax(220px,1fr));gap:26px;}
  .why-item{text-align:center;padding:0 8px;}
  .why-item .ic{
    width:56px;height:56px;border-radius:50%;
    background:rgba(214,162,51,.14);border:1.5px solid var(--gold);
    display:flex;align-items:center;justify-content:center;margin:0 auto 14px;
    color:var(--gold);font-size:22px;font-weight:800;
  }
  .why-item h3{font-family:'Times New Roman',Times,serif;font-size:16.5px;margin:0 0 4px;color:#fff;}
  .why-item p{font-size:13px;color:#B9C7D6;margin:0;}
  .why-item .why-en{font-size:11.5px;color:#7E93AA;font-style:italic;margin-top:5px;}

  /* ---------- Service area ---------- */
  .area{display:grid;grid-template-columns:1fr 1fr;gap:44px;align-items:center;}
  @media (max-width:820px){.area{grid-template-columns:1fr;}}
  .area-list{display:flex;flex-wrap:wrap;gap:10px;margin-top:18px;}
  .area-list span{
    background:#fff;border:1px solid var(--line);color:var(--navy);
    font-weight:600;font-size:13px;padding:8px 14px;border-radius:999px;
  }
  .area-list span.main{background:var(--navy);color:var(--gold-light);border-color:var(--navy);}
  .radius-card{
    background:#fff;border:1px solid var(--line);border-radius:16px;padding:30px;text-align:center;
  }
  .radius-card .miles{font-size:56px;font-weight:800;color:var(--navy);line-height:1;}
  .radius-card .miles sup{font-size:20px;top:-1.6em;color:var(--gold);}
  .radius-card p{color:var(--muted);font-size:13.5px;margin:8px 0 0;}

  /* ---------- CTA / contact ---------- */
  .cta{
    background:linear-gradient(180deg,var(--navy) 0%, var(--navy-dark) 100%);
    color:var(--cream);text-align:center;position:relative;
  }
  .cta h2{font-family:'Times New Roman',Times,serif;font-size:clamp(26px,4vw,38px);font-weight:800;margin:0 0 8px;}
  .cta .sub-en{color:#CBD8E6;margin:0 0 30px;font-size:15px;}
  .phone-big{
    font-family:'Times New Roman',Times,serif;
    font-size:clamp(34px,6vw,54px);font-weight:800;color:var(--gold);
    text-decoration:none;letter-spacing:.01em;
  }
  .email-big{
    display:block;
    font-family:'Times New Roman',Times,serif;
    font-size:clamp(17px,2.6vw,23px);font-weight:800;color:var(--cream);
    text-decoration:none;letter-spacing:.01em;margin-top:8px;
  }
  .email-big:hover{color:var(--gold-light);}
  .cta-row{display:flex;gap:14px;justify-content:center;flex-wrap:wrap;margin-top:26px;}

  /* ---------- Footer ---------- */
  footer{background:var(--navy-dark);color:#B9C7D6;padding:34px 0;font-size:13px;}
  .footer-grid{display:flex;justify-content:space-between;gap:20px;flex-wrap:wrap;align-items:center;}
  footer .brand{color:var(--cream);}
  footer .brand svg,footer .brand img{width:30px;height:30px;border-radius:50%;}
  .footer-links{display:flex;gap:18px;flex-wrap:wrap;}
  .footer-links a{text-decoration:none;color:#B9C7D6;}
  .footer-links a:hover{color:var(--gold);}
  .lic{color:#8FA1B4;font-size:12px;margin-top:10px;}
  .disclaimer{color:#6E8098;font-size:10.5px;margin-top:12px;line-height:1.6;max-width:520px;}
</style>
</head>
<body>

<!-- ================= TOP BAR ================= -->
<div class="topbar">
  <div class="topbar-inner">
    <a class="brand" href="#top">
      <svg viewBox="0 0 400 400" xmlns="http://www.w3.org/2000/svg">
  <defs>
    <linearGradient id="goldRingtb" x1="15%" y1="10%" x2="85%" y2="95%">
      <stop offset="0%" stop-color="#FCEBB6"/>
      <stop offset="14%" stop-color="#F3D276"/>
      <stop offset="30%" stop-color="#C9972E"/>
      <stop offset="42%" stop-color="#8F6A1D"/>
      <stop offset="50%" stop-color="#FCEBB6"/>
      <stop offset="64%" stop-color="#E8BE5E"/>
      <stop offset="80%" stop-color="#B5872A"/>
      <stop offset="100%" stop-color="#6B4E15"/>
    </linearGradient>
    <linearGradient id="goldTexttb" x1="0%" y1="0%" x2="0%" y2="100%">
      <stop offset="0%" stop-color="#FCEBB6"/>
      <stop offset="45%" stop-color="#E0B454"/>
      <stop offset="100%" stop-color="#9C7420"/>
    </linearGradient>
    <radialGradient id="navyFieldtb" cx="42%" cy="32%" r="78%">
      <stop offset="0%" stop-color="#16324E"/>
      <stop offset="60%" stop-color="#0B2036"/>
      <stop offset="100%" stop-color="#071322"/>
    </radialGradient>
    <path id="arcTop3tb" d="M 59.0,148.7 A 150,150 0 0 1 341.0,148.7" />
    <path id="arcBottom3tb" d="M 70.6,290.6 A 158,158 0 0 0 329.4,290.6" />
  </defs>

  <!-- outer gold ring (embossed, coin-edge style) -->
  <circle cx="200" cy="200" r="194" fill="url(#goldRingtb)"/>
  <circle cx="200" cy="200" r="194" fill="none" stroke="#4A3410" stroke-width="1"/>
  <!-- fluted / reeded texture -->
  <g>
    <line x1="381.00" y1="200.00" x2="392.00" y2="200.00" stroke="#4A3410" stroke-width="1.1" opacity="0.55"/>
    <line x1="380.56" y1="212.63" x2="391.53" y2="213.39" stroke="#4A3410" stroke-width="1.1" opacity="0.55"/>
    <line x1="379.24" y1="225.19" x2="390.13" y2="226.72" stroke="#4A3410" stroke-width="1.1" opacity="0.55"/>
    <line x1="377.04" y1="237.63" x2="387.80" y2="239.92" stroke="#4A3410" stroke-width="1.1" opacity="0.55"/>
    <line x1="373.99" y1="249.89" x2="384.56" y2="252.92" stroke="#4A3410" stroke-width="1.1" opacity="0.55"/>
    <line x1="370.08" y1="261.91" x2="380.42" y2="265.67" stroke="#4A3410" stroke-width="1.1" opacity="0.55"/>
    <line x1="365.35" y1="273.62" x2="375.40" y2="278.09" stroke="#4A3410" stroke-width="1.1" opacity="0.55"/>
    <line x1="359.81" y1="284.97" x2="369.53" y2="290.14" stroke="#4A3410" stroke-width="1.1" opacity="0.55"/>
    <line x1="353.50" y1="295.92" x2="362.83" y2="301.74" stroke="#4A3410" stroke-width="1.1" opacity="0.55"/>
    <line x1="346.43" y1="306.39" x2="355.33" y2="312.85" stroke="#4A3410" stroke-width="1.1" opacity="0.55"/>
    <line x1="338.65" y1="316.34" x2="347.08" y2="323.42" stroke="#4A3410" stroke-width="1.1" opacity="0.55"/>
    <line x1="330.20" y1="325.73" x2="338.11" y2="333.37" stroke="#4A3410" stroke-width="1.1" opacity="0.55"/>
    <line x1="321.11" y1="334.51" x2="328.47" y2="342.68" stroke="#4A3410" stroke-width="1.1" opacity="0.55"/>
    <line x1="311.43" y1="342.63" x2="318.21" y2="351.30" stroke="#4A3410" stroke-width="1.1" opacity="0.55"/>
    <line x1="301.21" y1="350.06" x2="307.37" y2="359.18" stroke="#4A3410" stroke-width="1.1" opacity="0.55"/>
    <line x1="290.50" y1="356.75" x2="296.00" y2="366.28" stroke="#4A3410" stroke-width="1.1" opacity="0.55"/>
    <line x1="279.35" y1="362.68" x2="284.17" y2="372.57" stroke="#4A3410" stroke-width="1.1" opacity="0.55"/>
    <line x1="267.80" y1="367.82" x2="271.92" y2="378.02" stroke="#4A3410" stroke-width="1.1" opacity="0.55"/>
    <line x1="255.93" y1="372.14" x2="259.33" y2="382.60" stroke="#4A3410" stroke-width="1.1" opacity="0.55"/>
    <line x1="243.79" y1="375.62" x2="246.45" y2="386.30" stroke="#4A3410" stroke-width="1.1" opacity="0.55"/>
    <line x1="231.43" y1="378.25" x2="233.34" y2="389.08" stroke="#4A3410" stroke-width="1.1" opacity="0.55"/>
    <line x1="218.92" y1="380.01" x2="220.07" y2="390.95" stroke="#4A3410" stroke-width="1.1" opacity="0.55"/>
    <line x1="206.32" y1="380.89" x2="206.70" y2="391.88" stroke="#4A3410" stroke-width="1.1" opacity="0.55"/>
    <line x1="193.68" y1="380.89" x2="193.30" y2="391.88" stroke="#4A3410" stroke-width="1.1" opacity="0.55"/>
    <line x1="181.08" y1="380.01" x2="179.93" y2="390.95" stroke="#4A3410" stroke-width="1.1" opacity="0.55"/>
    <line x1="168.57" y1="378.25" x2="166.66" y2="389.08" stroke="#4A3410" stroke-width="1.1" opacity="0.55"/>
    <line x1="156.21" y1="375.62" x2="153.55" y2="386.30" stroke="#4A3410" stroke-width="1.1" opacity="0.55"/>
    <line x1="144.07" y1="372.14" x2="140.67" y2="382.60" stroke="#4A3410" stroke-width="1.1" opacity="0.55"/>
    <line x1="132.20" y1="367.82" x2="128.08" y2="378.02" stroke="#4A3410" stroke-width="1.1" opacity="0.55"/>
    <line x1="120.65" y1="362.68" x2="115.83" y2="372.57" stroke="#4A3410" stroke-width="1.1" opacity="0.55"/>
    <line x1="109.50" y1="356.75" x2="104.00" y2="366.28" stroke="#4A3410" stroke-width="1.1" opacity="0.55"/>
    <line x1="98.79" y1="350.06" x2="92.63" y2="359.18" stroke="#4A3410" stroke-width="1.1" opacity="0.55"/>
    <line x1="88.57" y1="342.63" x2="81.79" y2="351.30" stroke="#4A3410" stroke-width="1.1" opacity="0.55"/>
    <line x1="78.89" y1="334.51" x2="71.53" y2="342.68" stroke="#4A3410" stroke-width="1.1" opacity="0.55"/>
    <line x1="69.80" y1="325.73" x2="61.89" y2="333.37" stroke="#4A3410" stroke-width="1.1" opacity="0.55"/>
    <line x1="61.35" y1="316.34" x2="52.92" y2="323.42" stroke="#4A3410" stroke-width="1.1" opacity="0.55"/>
    <line x1="53.57" y1="306.39" x2="44.67" y2="312.85" stroke="#4A3410" stroke-width="1.1" opacity="0.55"/>
    <line x1="46.50" y1="295.92" x2="37.17" y2="301.74" stroke="#4A3410" stroke-width="1.1" opacity="0.55"/>
    <line x1="40.19" y1="284.97" x2="30.47" y2="290.14" stroke="#4A3410" stroke-width="1.1" opacity="0.55"/>
    <line x1="34.65" y1="273.62" x2="24.60" y2="278.09" stroke="#4A3410" stroke-width="1.1" opacity="0.55"/>
    <line x1="29.92" y1="261.91" x2="19.58" y2="265.67" stroke="#4A3410" stroke-width="1.1" opacity="0.55"/>
    <line x1="26.01" y1="249.89" x2="15.44" y2="252.92" stroke="#4A3410" stroke-width="1.1" opacity="0.55"/>
    <line x1="22.96" y1="237.63" x2="12.20" y2="239.92" stroke="#4A3410" stroke-width="1.1" opacity="0.55"/>
    <line x1="20.76" y1="225.19" x2="9.87" y2="226.72" stroke="#4A3410" stroke-width="1.1" opacity="0.55"/>
    <line x1="19.44" y1="212.63" x2="8.47" y2="213.39" stroke="#4A3410" stroke-width="1.1" opacity="0.55"/>
    <line x1="19.00" y1="200.00" x2="8.00" y2="200.00" stroke="#4A3410" stroke-width="1.1" opacity="0.55"/>
    <line x1="19.44" y1="187.37" x2="8.47" y2="186.61" stroke="#4A3410" stroke-width="1.1" opacity="0.55"/>
    <line x1="20.76" y1="174.81" x2="9.87" y2="173.28" stroke="#4A3410" stroke-width="1.1" opacity="0.55"/>
    <line x1="22.96" y1="162.37" x2="12.20" y2="160.08" stroke="#4A3410" stroke-width="1.1" opacity="0.55"/>
    <line x1="26.01" y1="150.11" x2="15.44" y2="147.08" stroke="#4A3410" stroke-width="1.1" opacity="0.55"/>
    <line x1="29.92" y1="138.09" x2="19.58" y2="134.33" stroke="#4A3410" stroke-width="1.1" opacity="0.55"/>
    <line x1="34.65" y1="126.38" x2="24.60" y2="121.91" stroke="#4A3410" stroke-width="1.1" opacity="0.55"/>
    <line x1="40.19" y1="115.03" x2="30.47" y2="109.86" stroke="#4A3410" stroke-width="1.1" opacity="0.55"/>
    <line x1="46.50" y1="104.08" x2="37.17" y2="98.26" stroke="#4A3410" stroke-width="1.1" opacity="0.55"/>
    <line x1="53.57" y1="93.61" x2="44.67" y2="87.15" stroke="#4A3410" stroke-width="1.1" opacity="0.55"/>
    <line x1="61.35" y1="83.66" x2="52.92" y2="76.58" stroke="#4A3410" stroke-width="1.1" opacity="0.55"/>
    <line x1="69.80" y1="74.27" x2="61.89" y2="66.63" stroke="#4A3410" stroke-width="1.1" opacity="0.55"/>
    <line x1="78.89" y1="65.49" x2="71.53" y2="57.32" stroke="#4A3410" stroke-width="1.1" opacity="0.55"/>
    <line x1="88.57" y1="57.37" x2="81.79" y2="48.70" stroke="#4A3410" stroke-width="1.1" opacity="0.55"/>
    <line x1="98.79" y1="49.94" x2="92.63" y2="40.82" stroke="#4A3410" stroke-width="1.1" opacity="0.55"/>
    <line x1="109.50" y1="43.25" x2="104.00" y2="33.72" stroke="#4A3410" stroke-width="1.1" opacity="0.55"/>
    <line x1="120.65" y1="37.32" x2="115.83" y2="27.43" stroke="#4A3410" stroke-width="1.1" opacity="0.55"/>
    <line x1="132.20" y1="32.18" x2="128.08" y2="21.98" stroke="#4A3410" stroke-width="1.1" opacity="0.55"/>
    <line x1="144.07" y1="27.86" x2="140.67" y2="17.40" stroke="#4A3410" stroke-width="1.1" opacity="0.55"/>
    <line x1="156.21" y1="24.38" x2="153.55" y2="13.70" stroke="#4A3410" stroke-width="1.1" opacity="0.55"/>
    <line x1="168.57" y1="21.75" x2="166.66" y2="10.92" stroke="#4A3410" stroke-width="1.1" opacity="0.55"/>
    <line x1="181.08" y1="19.99" x2="179.93" y2="9.05" stroke="#4A3410" stroke-width="1.1" opacity="0.55"/>
    <line x1="193.68" y1="19.11" x2="193.30" y2="8.12" stroke="#4A3410" stroke-width="1.1" opacity="0.55"/>
    <line x1="206.32" y1="19.11" x2="206.70" y2="8.12" stroke="#4A3410" stroke-width="1.1" opacity="0.55"/>
    <line x1="218.92" y1="19.99" x2="220.07" y2="9.05" stroke="#4A3410" stroke-width="1.1" opacity="0.55"/>
    <line x1="231.43" y1="21.75" x2="233.34" y2="10.92" stroke="#4A3410" stroke-width="1.1" opacity="0.55"/>
    <line x1="243.79" y1="24.38" x2="246.45" y2="13.70" stroke="#4A3410" stroke-width="1.1" opacity="0.55"/>
    <line x1="255.93" y1="27.86" x2="259.33" y2="17.40" stroke="#4A3410" stroke-width="1.1" opacity="0.55"/>
    <line x1="267.80" y1="32.18" x2="271.92" y2="21.98" stroke="#4A3410" stroke-width="1.1" opacity="0.55"/>
    <line x1="279.35" y1="37.32" x2="284.17" y2="27.43" stroke="#4A3410" stroke-width="1.1" opacity="0.55"/>
    <line x1="290.50" y1="43.25" x2="296.00" y2="33.72" stroke="#4A3410" stroke-width="1.1" opacity="0.55"/>
    <line x1="301.21" y1="49.94" x2="307.37" y2="40.82" stroke="#4A3410" stroke-width="1.1" opacity="0.55"/>
    <line x1="311.43" y1="57.37" x2="318.21" y2="48.70" stroke="#4A3410" stroke-width="1.1" opacity="0.55"/>
    <line x1="321.11" y1="65.49" x2="328.47" y2="57.32" stroke="#4A3410" stroke-width="1.1" opacity="0.55"/>
    <line x1="330.20" y1="74.27" x2="338.11" y2="66.63" stroke="#4A3410" stroke-width="1.1" opacity="0.55"/>
    <line x1="338.65" y1="83.66" x2="347.08" y2="76.58" stroke="#4A3410" stroke-width="1.1" opacity="0.55"/>
    <line x1="346.43" y1="93.61" x2="355.33" y2="87.15" stroke="#4A3410" stroke-width="1.1" opacity="0.55"/>
    <line x1="353.50" y1="104.08" x2="362.83" y2="98.26" stroke="#4A3410" stroke-width="1.1" opacity="0.55"/>
    <line x1="359.81" y1="115.03" x2="369.53" y2="109.86" stroke="#4A3410" stroke-width="1.1" opacity="0.55"/>
    <line x1="365.35" y1="126.38" x2="375.40" y2="121.91" stroke="#4A3410" stroke-width="1.1" opacity="0.55"/>
    <line x1="370.08" y1="138.09" x2="380.42" y2="134.33" stroke="#4A3410" stroke-width="1.1" opacity="0.55"/>
    <line x1="373.99" y1="150.11" x2="384.56" y2="147.08" stroke="#4A3410" stroke-width="1.1" opacity="0.55"/>
    <line x1="377.04" y1="162.37" x2="387.80" y2="160.08" stroke="#4A3410" stroke-width="1.1" opacity="0.55"/>
    <line x1="379.24" y1="174.81" x2="390.13" y2="173.28" stroke="#4A3410" stroke-width="1.1" opacity="0.55"/>
    <line x1="380.56" y1="187.37" x2="391.53" y2="186.61" stroke="#4A3410" stroke-width="1.1" opacity="0.55"/>
  </g>
  <!-- beaded ring -->
  <g>
    <circle cx="387.00" cy="200.00" r="2.1" fill="url(#goldTexttb)"/>
    <circle cx="386.29" cy="216.30" r="2.1" fill="url(#goldTexttb)"/>
    <circle cx="384.16" cy="232.47" r="2.1" fill="url(#goldTexttb)"/>
    <circle cx="380.63" cy="248.40" r="2.1" fill="url(#goldTexttb)"/>
    <circle cx="375.72" cy="263.96" r="2.1" fill="url(#goldTexttb)"/>
    <circle cx="369.48" cy="279.03" r="2.1" fill="url(#goldTexttb)"/>
    <circle cx="361.95" cy="293.50" r="2.1" fill="url(#goldTexttb)"/>
    <circle cx="353.18" cy="307.26" r="2.1" fill="url(#goldTexttb)"/>
    <circle cx="343.25" cy="320.20" r="2.1" fill="url(#goldTexttb)"/>
    <circle cx="332.23" cy="332.23" r="2.1" fill="url(#goldTexttb)"/>
    <circle cx="320.20" cy="343.25" r="2.1" fill="url(#goldTexttb)"/>
    <circle cx="307.26" cy="353.18" r="2.1" fill="url(#goldTexttb)"/>
    <circle cx="293.50" cy="361.95" r="2.1" fill="url(#goldTexttb)"/>
    <circle cx="279.03" cy="369.48" r="2.1" fill="url(#goldTexttb)"/>
    <circle cx="263.96" cy="375.72" r="2.1" fill="url(#goldTexttb)"/>
    <circle cx="248.40" cy="380.63" r="2.1" fill="url(#goldTexttb)"/>
    <circle cx="232.47" cy="384.16" r="2.1" fill="url(#goldTexttb)"/>
    <circle cx="216.30" cy="386.29" r="2.1" fill="url(#goldTexttb)"/>
    <circle cx="200.00" cy="387.00" r="2.1" fill="url(#goldTexttb)"/>
    <circle cx="183.70" cy="386.29" r="2.1" fill="url(#goldTexttb)"/>
    <circle cx="167.53" cy="384.16" r="2.1" fill="url(#goldTexttb)"/>
    <circle cx="151.60" cy="380.63" r="2.1" fill="url(#goldTexttb)"/>
    <circle cx="136.04" cy="375.72" r="2.1" fill="url(#goldTexttb)"/>
    <circle cx="120.97" cy="369.48" r="2.1" fill="url(#goldTexttb)"/>
    <circle cx="106.50" cy="361.95" r="2.1" fill="url(#goldTexttb)"/>
    <circle cx="92.74" cy="353.18" r="2.1" fill="url(#goldTexttb)"/>
    <circle cx="79.80" cy="343.25" r="2.1" fill="url(#goldTexttb)"/>
    <circle cx="67.77" cy="332.23" r="2.1" fill="url(#goldTexttb)"/>
    <circle cx="56.75" cy="320.20" r="2.1" fill="url(#goldTexttb)"/>
    <circle cx="46.82" cy="307.26" r="2.1" fill="url(#goldTexttb)"/>
    <circle cx="38.05" cy="293.50" r="2.1" fill="url(#goldTexttb)"/>
    <circle cx="30.52" cy="279.03" r="2.1" fill="url(#goldTexttb)"/>
    <circle cx="24.28" cy="263.96" r="2.1" fill="url(#goldTexttb)"/>
    <circle cx="19.37" cy="248.40" r="2.1" fill="url(#goldTexttb)"/>
    <circle cx="15.84" cy="232.47" r="2.1" fill="url(#goldTexttb)"/>
    <circle cx="13.71" cy="216.30" r="2.1" fill="url(#goldTexttb)"/>
    <circle cx="13.00" cy="200.00" r="2.1" fill="url(#goldTexttb)"/>
    <circle cx="13.71" cy="183.70" r="2.1" fill="url(#goldTexttb)"/>
    <circle cx="15.84" cy="167.53" r="2.1" fill="url(#goldTexttb)"/>
    <circle cx="19.37" cy="151.60" r="2.1" fill="url(#goldTexttb)"/>
    <circle cx="24.28" cy="136.04" r="2.1" fill="url(#goldTexttb)"/>
    <circle cx="30.52" cy="120.97" r="2.1" fill="url(#goldTexttb)"/>
    <circle cx="38.05" cy="106.50" r="2.1" fill="url(#goldTexttb)"/>
    <circle cx="46.82" cy="92.74" r="2.1" fill="url(#goldTexttb)"/>
    <circle cx="56.75" cy="79.80" r="2.1" fill="url(#goldTexttb)"/>
    <circle cx="67.77" cy="67.77" r="2.1" fill="url(#goldTexttb)"/>
    <circle cx="79.80" cy="56.75" r="2.1" fill="url(#goldTexttb)"/>
    <circle cx="92.74" cy="46.82" r="2.1" fill="url(#goldTexttb)"/>
    <circle cx="106.50" cy="38.05" r="2.1" fill="url(#goldTexttb)"/>
    <circle cx="120.97" cy="30.52" r="2.1" fill="url(#goldTexttb)"/>
    <circle cx="136.04" cy="24.28" r="2.1" fill="url(#goldTexttb)"/>
    <circle cx="151.60" cy="19.37" r="2.1" fill="url(#goldTexttb)"/>
    <circle cx="167.53" cy="15.84" r="2.1" fill="url(#goldTexttb)"/>
    <circle cx="183.70" cy="13.71" r="2.1" fill="url(#goldTexttb)"/>
    <circle cx="200.00" cy="13.00" r="2.1" fill="url(#goldTexttb)"/>
    <circle cx="216.30" cy="13.71" r="2.1" fill="url(#goldTexttb)"/>
    <circle cx="232.47" cy="15.84" r="2.1" fill="url(#goldTexttb)"/>
    <circle cx="248.40" cy="19.37" r="2.1" fill="url(#goldTexttb)"/>
    <circle cx="263.96" cy="24.28" r="2.1" fill="url(#goldTexttb)"/>
    <circle cx="279.03" cy="30.52" r="2.1" fill="url(#goldTexttb)"/>
    <circle cx="293.50" cy="38.05" r="2.1" fill="url(#goldTexttb)"/>
    <circle cx="307.26" cy="46.82" r="2.1" fill="url(#goldTexttb)"/>
    <circle cx="320.20" cy="56.75" r="2.1" fill="url(#goldTexttb)"/>
    <circle cx="332.23" cy="67.77" r="2.1" fill="url(#goldTexttb)"/>
    <circle cx="343.25" cy="79.80" r="2.1" fill="url(#goldTexttb)"/>
    <circle cx="353.18" cy="92.74" r="2.1" fill="url(#goldTexttb)"/>
    <circle cx="361.95" cy="106.50" r="2.1" fill="url(#goldTexttb)"/>
    <circle cx="369.48" cy="120.97" r="2.1" fill="url(#goldTexttb)"/>
    <circle cx="375.72" cy="136.04" r="2.1" fill="url(#goldTexttb)"/>
    <circle cx="380.63" cy="151.60" r="2.1" fill="url(#goldTexttb)"/>
    <circle cx="384.16" cy="167.53" r="2.1" fill="url(#goldTexttb)"/>
    <circle cx="386.29" cy="183.70" r="2.1" fill="url(#goldTexttb)"/>
  </g>
  <circle cx="200" cy="200" r="183" fill="none" stroke="#FCEBB6" stroke-width="1" stroke-opacity="0.55"/>
  <circle cx="200" cy="200" r="179" fill="none" stroke="#071322" stroke-width="3"/>

  <!-- navy field -->
  <circle cx="200" cy="200" r="176" fill="url(#navyFieldtb)"/>
  <!-- inner thin gold ring -->
  <circle cx="200" cy="200" r="140" fill="none" stroke="url(#goldTexttb)" stroke-width="2"/>

  <!-- flanking dots -->
  <circle cx="51.5" cy="146.0" r="2.8" fill="#E0B454"/>
  <circle cx="348.5" cy="146.0" r="2.8" fill="#E0B454"/>

  <!-- arched top text: company name (faux emboss: shadow + gold) -->
  <text font-family="Liberation Serif" font-weight="bold" font-size="28" letter-spacing="3.6" fill="#04101c">
    <textPath href="#arcTop3tb" startOffset="50%" text-anchor="middle" dy="1.6">LA SOLUCIÓN DE LEO</textPath>
  </text>
  <text font-family="Liberation Serif" font-weight="bold" font-size="28" letter-spacing="3.6" fill="url(#goldTexttb)">
    <textPath href="#arcTop3tb" startOffset="50%" text-anchor="middle">LA SOLUCIÓN DE LEO</textPath>
  </text>

  <!-- arched bottom text: LICENSED AND BONDED -->
  <text font-family="Liberation Serif" font-weight="bold" font-size="14" letter-spacing="2.2" fill="#04101c">
    <textPath href="#arcBottom3tb" startOffset="50%" text-anchor="middle" dy="1.4">LICENSED AND BONDED</textPath>
  </text>
  <text font-family="Liberation Serif" font-weight="bold" font-size="14" letter-spacing="2.2" fill="url(#goldTexttb)">
    <textPath href="#arcBottom3tb" startOffset="50%" text-anchor="middle">LICENSED AND BONDED</textPath>
  </text>

  <!-- monogram group -->
  <g transform="translate(200,192)">
    <!-- feather quill: detailed plume with barbs, angled up-right off second L -->
    <g transform="translate(44,-44) rotate(28) scale(0.72)">
      <path d="M0,2 C 6,-28 4,-58 -10,-84 C -2,-58 -6,-38 -18,-20
               C -12,-24 -4,-20 0,-10 C 4,-2 2,4 0,2 Z"
            fill="url(#goldTexttb)" stroke="#5C4310" stroke-width="0.8"/>
      <!-- barb lines -->
      <path d="M -6,-6 C -10,-16 -16,-24 -22,-30" stroke="#5C4310" stroke-width="0.6" fill="none" opacity="0.7"/>
      <path d="M -4,-16 C -8,-26 -13,-34 -19,-42" stroke="#5C4310" stroke-width="0.6" fill="none" opacity="0.7"/>
      <path d="M -3,-28 C -6,-38 -10,-46 -15,-54" stroke="#5C4310" stroke-width="0.6" fill="none" opacity="0.7"/>
      <path d="M -2,-40 C -4,-50 -7,-58 -11,-66" stroke="#5C4310" stroke-width="0.6" fill="none" opacity="0.7"/>
      <path d="M -1,-52 C -3,-61 -5,-68 -8,-76" stroke="#5C4310" stroke-width="0.6" fill="none" opacity="0.7"/>
      <path d="M -10,-84 L 8,6" stroke="#5C4310" stroke-width="1.1" fill="none"/>
      <!-- pen shaft -->
      <line x1="4" y1="-2" x2="30" y2="24" stroke="url(#goldTexttb)" stroke-width="3.6" stroke-linecap="round"/>
      <!-- ink swirl at nib -->
      <path d="M 30,24 C 38,26 42,32 38,38 C 34,43 26,41 26,35" fill="none" stroke="url(#goldTexttb)" stroke-width="2.4" stroke-linecap="round"/>
    </g>

    <!-- monogram L S L with faux-emboss shadow -->
    <g transform="translate(1.6,2.4)" fill="#04101c" opacity="0.55">
      <text x="-58" y="34" font-family="Liberation Serif" font-weight="bold" font-size="112" text-anchor="middle">L</text>
      <text x="0" y="20" font-family="Liberation Serif" font-weight="bold" font-size="68" text-anchor="middle">S</text>
      <text x="55" y="34" font-family="Liberation Serif" font-weight="bold" font-size="112" text-anchor="middle">L</text>
    </g>
    <text x="-58" y="34" font-family="Liberation Serif" font-weight="bold" font-size="112" fill="url(#goldTexttb)" text-anchor="middle">L</text>
    <text x="0" y="20" font-family="Liberation Serif" font-weight="bold" font-size="68" fill="url(#goldTexttb)" text-anchor="middle">S</text>
    <text x="55" y="34" font-family="Liberation Serif" font-weight="bold" font-size="112" fill="url(#goldTexttb)" text-anchor="middle">L</text>

    <!-- pillar icon -->
    <g transform="translate(0,64)">
      <g transform="translate(1.4,2)" fill="#04101c" opacity="0.5">
        <rect x="-30" y="0" width="60" height="7" rx="1.5"/>
        <rect x="-24" y="7" width="48" height="4"/>
        <rect x="-19" y="11" width="6" height="26"/>
        <rect x="-6.5" y="11" width="6" height="26"/>
        <rect x="6" y="11" width="6" height="26"/>
        <rect x="18.5" y="11" width="6" height="26"/>
        <rect x="-24" y="37" width="48" height="4"/>
        <rect x="-30" y="41" width="60" height="7" rx="1.5"/>
      </g>
      <g fill="url(#goldTexttb)">
        <rect x="-30" y="0" width="60" height="7" rx="1.5"/>
        <rect x="-24" y="7" width="48" height="4"/>
        <rect x="-19" y="11" width="6" height="26"/>
        <rect x="-6.5" y="11" width="6" height="26"/>
        <rect x="6" y="11" width="6" height="26"/>
        <rect x="18.5" y="11" width="6" height="26"/>
        <rect x="-24" y="37" width="48" height="4"/>
        <rect x="-30" y="41" width="60" height="7" rx="1.5"/>
      </g>
    </g>
  </g>
</svg>

      <span class="brand-name">La Solución de Leo<span>NOTARY PUBLIC · DOCUMENTOS · IMPUESTOS</span></span>
    </a>
    <a class="call-btn" href="tel:+14086134713">📞 (408) 613-4713</a>
  </div>
</div>

<!-- ================= HERO ================= -->
<header class="hero" id="top">
  <div class="wrap hero-grid">
    <div>
      <span class="eyebrow">Notary Public · Servicio Móvil</span>
      <h1>Documentos, impuestos<br> y traducciones — <em>nosotros vamos a usted.</em></h1>
      <p class="sub-en">Mobile document, tax &amp; translation service — we come to you, anywhere in Greater Sacramento.</p>
      <p class="lead">Licenciado y afianzado. Trabajo garantizado. Un servicio honesto y personal para nuestra comunidad — se habla español.</p>
      <div class="hero-ctas">
        <a class="btn btn-primary" href="tel:+14086134713">📞 Llamar / Call: (408) 613-4713</a>
        <a class="btn btn-ghost" href="#servicios">Ver servicios · See services</a>
      </div>
      <div class="hero-badges">
        <span class="pill">LICENCIADO Y AFIANZADO · LICENSED &amp; BONDED</span>
        <span class="pill">TRABAJO GARANTIZADO · WORK GUARANTEED</span>
        <span class="pill">SE HABLA ESPAÑOL · ENGLISH SPOKEN</span>
        <span class="pill">SERVICIO MÓVIL · MOBILE SERVICE</span>
      </div>
    </div>
    <div class="seal-wrap">
      <svg viewBox="0 0 400 400" xmlns="http://www.w3.org/2000/svg">
  <defs>
    <linearGradient id="goldRing" x1="15%" y1="10%" x2="85%" y2="95%">
      <stop offset="0%" stop-color="#FCEBB6"/>
      <stop offset="14%" stop-color="#F3D276"/>
      <stop offset="30%" stop-color="#C9972E"/>
      <stop offset="42%" stop-color="#8F6A1D"/>
      <stop offset="50%" stop-color="#FCEBB6"/>
      <stop offset="64%" stop-color="#E8BE5E"/>
      <stop offset="80%" stop-color="#B5872A"/>
      <stop offset="100%" stop-color="#6B4E15"/>
    </linearGradient>
    <linearGradient id="goldText" x1="0%" y1="0%" x2="0%" y2="100%">
      <stop offset="0%" stop-color="#FCEBB6"/>
      <stop offset="45%" stop-color="#E0B454"/>
      <stop offset="100%" stop-color="#9C7420"/>
    </linearGradient>
    <radialGradient id="navyField" cx="42%" cy="32%" r="78%">
      <stop offset="0%" stop-color="#16324E"/>
      <stop offset="60%" stop-color="#0B2036"/>
      <stop offset="100%" stop-color="#071322"/>
    </radialGradient>
    <path id="arcTop3" d="M 59.0,148.7 A 150,150 0 0 1 341.0,148.7" />
    <path id="arcBottom3" d="M 70.6,290.6 A 158,158 0 0 0 329.4,290.6" />
  </defs>

  <!-- outer gold ring (embossed, coin-edge style) -->
  <circle cx="200" cy="200" r="194" fill="url(#goldRing)"/>
  <circle cx="200" cy="200" r="194" fill="none" stroke="#4A3410" stroke-width="1"/>
  <!-- fluted / reeded texture -->
  <g>
    <line x1="381.00" y1="200.00" x2="392.00" y2="200.00" stroke="#4A3410" stroke-width="1.1" opacity="0.55"/>
    <line x1="380.56" y1="212.63" x2="391.53" y2="213.39" stroke="#4A3410" stroke-width="1.1" opacity="0.55"/>
    <line x1="379.24" y1="225.19" x2="390.13" y2="226.72" stroke="#4A3410" stroke-width="1.1" opacity="0.55"/>
    <line x1="377.04" y1="237.63" x2="387.80" y2="239.92" stroke="#4A3410" stroke-width="1.1" opacity="0.55"/>
    <line x1="373.99" y1="249.89" x2="384.56" y2="252.92" stroke="#4A3410" stroke-width="1.1" opacity="0.55"/>
    <line x1="370.08" y1="261.91" x2="380.42" y2="265.67" stroke="#4A3410" stroke-width="1.1" opacity="0.55"/>
    <line x1="365.35" y1="273.62" x2="375.40" y2="278.09" stroke="#4A3410" stroke-width="1.1" opacity="0.55"/>
    <line x1="359.81" y1="284.97" x2="369.53" y2="290.14" stroke="#4A3410" stroke-width="1.1" opacity="0.55"/>
    <line x1="353.50" y1="295.92" x2="362.83" y2="301.74" stroke="#4A3410" stroke-width="1.1" opacity="0.55"/>
    <line x1="346.43" y1="306.39" x2="355.33" y2="312.85" stroke="#4A3410" stroke-width="1.1" opacity="0.55"/>
    <line x1="338.65" y1="316.34" x2="347.08" y2="323.42" stroke="#4A3410" stroke-width="1.1" opacity="0.55"/>
    <line x1="330.20" y1="325.73" x2="338.11" y2="333.37" stroke="#4A3410" stroke-width="1.1" opacity="0.55"/>
    <line x1="321.11" y1="334.51" x2="328.47" y2="342.68" stroke="#4A3410" stroke-width="1.1" opacity="0.55"/>
    <line x1="311.43" y1="342.63" x2="318.21" y2="351.30" stroke="#4A3410" stroke-width="1.1" opacity="0.55"/>
    <line x1="301.21" y1="350.06" x2="307.37" y2="359.18" stroke="#4A3410" stroke-width="1.1" opacity="0.55"/>
    <line x1="290.50" y1="356.75" x2="296.00" y2="366.28" stroke="#4A3410" stroke-width="1.1" opacity="0.55"/>
    <line x1="279.35" y1="362.68" x2="284.17" y2="372.57" stroke="#4A3410" stroke-width="1.1" opacity="0.55"/>
    <line x1="267.80" y1="367.82" x2="271.92" y2="378.02" stroke="#4A3410" stroke-width="1.1" opacity="0.55"/>
    <line x1="255.93" y1="372.14" x2="259.33" y2="382.60" stroke="#4A3410" stroke-width="1.1" opacity="0.55"/>
    <line x1="243.79" y1="375.62" x2="246.45" y2="386.30" stroke="#4A3410" stroke-width="1.1" opacity="0.55"/>
    <line x1="231.43" y1="378.25" x2="233.34" y2="389.08" stroke="#4A3410" stroke-width="1.1" opacity="0.55"/>
    <line x1="218.92" y1="380.01" x2="220.07" y2="390.95" stroke="#4A3410" stroke-width="1.1" opacity="0.55"/>
    <line x1="206.32" y1="380.89" x2="206.70" y2="391.88" stroke="#4A3410" stroke-width="1.1" opacity="0.55"/>
    <line x1="193.68" y1="380.89" x2="193.30" y2="391.88" stroke="#4A3410" stroke-width="1.1" opacity="0.55"/>
    <line x1="181.08" y1="380.01" x2="179.93" y2="390.95" stroke="#4A3410" stroke-width="1.1" opacity="0.55"/>
    <line x1="168.57" y1="378.25" x2="166.66" y2="389.08" stroke="#4A3410" stroke-width="1.1" opacity="0.55"/>
    <line x1="156.21" y1="375.62" x2="153.55" y2="386.30" stroke="#4A3410" stroke-width="1.1" opacity="0.55"/>
    <line x1="144.07" y1="372.14" x2="140.67" y2="382.60" stroke="#4A3410" stroke-width="1.1" opacity="0.55"/>
    <line x1="132.20" y1="367.82" x2="128.08" y2="378.02" stroke="#4A3410" stroke-width="1.1" opacity="0.55"/>
    <line x1="120.65" y1="362.68" x2="115.83" y2="372.57" stroke="#4A3410" stroke-width="1.1" opacity="0.55"/>
    <line x1="109.50" y1="356.75" x2="104.00" y2="366.28" stroke="#4A3410" stroke-width="1.1" opacity="0.55"/>
    <line x1="98.79" y1="350.06" x2="92.63" y2="359.18" stroke="#4A3410" stroke-width="1.1" opacity="0.55"/>
    <line x1="88.57" y1="342.63" x2="81.79" y2="351.30" stroke="#4A3410" stroke-width="1.1" opacity="0.55"/>
    <line x1="78.89" y1="334.51" x2="71.53" y2="342.68" stroke="#4A3410" stroke-width="1.1" opacity="0.55"/>
    <line x1="69.80" y1="325.73" x2="61.89" y2="333.37" stroke="#4A3410" stroke-width="1.1" opacity="0.55"/>
    <line x1="61.35" y1="316.34" x2="52.92" y2="323.42" stroke="#4A3410" stroke-width="1.1" opacity="0.55"/>
    <line x1="53.57" y1="306.39" x2="44.67" y2="312.85" stroke="#4A3410" stroke-width="1.1" opacity="0.55"/>
    <line x1="46.50" y1="295.92" x2="37.17" y2="301.74" stroke="#4A3410" stroke-width="1.1" opacity="0.55"/>
    <line x1="40.19" y1="284.97" x2="30.47" y2="290.14" stroke="#4A3410" stroke-width="1.1" opacity="0.55"/>
    <line x1="34.65" y1="273.62" x2="24.60" y2="278.09" stroke="#4A3410" stroke-width="1.1" opacity="0.55"/>
    <line x1="29.92" y1="261.91" x2="19.58" y2="265.67" stroke="#4A3410" stroke-width="1.1" opacity="0.55"/>
    <line x1="26.01" y1="249.89" x2="15.44" y2="252.92" stroke="#4A3410" stroke-width="1.1" opacity="0.55"/>
    <line x1="22.96" y1="237.63" x2="12.20" y2="239.92" stroke="#4A3410" stroke-width="1.1" opacity="0.55"/>
    <line x1="20.76" y1="225.19" x2="9.87" y2="226.72" stroke="#4A3410" stroke-width="1.1" opacity="0.55"/>
    <line x1="19.44" y1="212.63" x2="8.47" y2="213.39" stroke="#4A3410" stroke-width="1.1" opacity="0.55"/>
    <line x1="19.00" y1="200.00" x2="8.00" y2="200.00" stroke="#4A3410" stroke-width="1.1" opacity="0.55"/>
    <line x1="19.44" y1="187.37" x2="8.47" y2="186.61" stroke="#4A3410" stroke-width="1.1" opacity="0.55"/>
    <line x1="20.76" y1="174.81" x2="9.87" y2="173.28" stroke="#4A3410" stroke-width="1.1" opacity="0.55"/>
    <line x1="22.96" y1="162.37" x2="12.20" y2="160.08" stroke="#4A3410" stroke-width="1.1" opacity="0.55"/>
    <line x1="26.01" y1="150.11" x2="15.44" y2="147.08" stroke="#4A3410" stroke-width="1.1" opacity="0.55"/>
    <line x1="29.92" y1="138.09" x2="19.58" y2="134.33" stroke="#4A3410" stroke-width="1.1" opacity="0.55"/>
    <line x1="34.65" y1="126.38" x2="24.60" y2="121.91" stroke="#4A3410" stroke-width="1.1" opacity="0.55"/>
    <line x1="40.19" y1="115.03" x2="30.47" y2="109.86" stroke="#4A3410" stroke-width="1.1" opacity="0.55"/>
    <line x1="46.50" y1="104.08" x2="37.17" y2="98.26" stroke="#4A3410" stroke-width="1.1" opacity="0.55"/>
    <line x1="53.57" y1="93.61" x2="44.67" y2="87.15" stroke="#4A3410" stroke-width="1.1" opacity="0.55"/>
    <line x1="61.35" y1="83.66" x2="52.92" y2="76.58" stroke="#4A3410" stroke-width="1.1" opacity="0.55"/>
    <line x1="69.80" y1="74.27" x2="61.89" y2="66.63" stroke="#4A3410" stroke-width="1.1" opacity="0.55"/>
    <line x1="78.89" y1="65.49" x2="71.53" y2="57.32" stroke="#4A3410" stroke-width="1.1" opacity="0.55"/>
    <line x1="88.57" y1="57.37" x2="81.79" y2="48.70" stroke="#4A3410" stroke-width="1.1" opacity="0.55"/>
    <line x1="98.79" y1="49.94" x2="92.63" y2="40.82" stroke="#4A3410" stroke-width="1.1" opacity="0.55"/>
    <line x1="109.50" y1="43.25" x2="104.00" y2="33.72" stroke="#4A3410" stroke-width="1.1" opacity="0.55"/>
    <line x1="120.65" y1="37.32" x2="115.83" y2="27.43" stroke="#4A3410" stroke-width="1.1" opacity="0.55"/>
    <line x1="132.20" y1="32.18" x2="128.08" y2="21.98" stroke="#4A3410" stroke-width="1.1" opacity="0.55"/>
    <line x1="144.07" y1="27.86" x2="140.67" y2="17.40" stroke="#4A3410" stroke-width="1.1" opacity="0.55"/>
    <line x1="156.21" y1="24.38" x2="153.55" y2="13.70" stroke="#4A3410" stroke-width="1.1" opacity="0.55"/>
    <line x1="168.57" y1="21.75" x2="166.66" y2="10.92" stroke="#4A3410" stroke-width="1.1" opacity="0.55"/>
    <line x1="181.08" y1="19.99" x2="179.93" y2="9.05" stroke="#4A3410" stroke-width="1.1" opacity="0.55"/>
    <line x1="193.68" y1="19.11" x2="193.30" y2="8.12" stroke="#4A3410" stroke-width="1.1" opacity="0.55"/>
    <line x1="206.32" y1="19.11" x2="206.70" y2="8.12" stroke="#4A3410" stroke-width="1.1" opacity="0.55"/>
    <line x1="218.92" y1="19.99" x2="220.07" y2="9.05" stroke="#4A3410" stroke-width="1.1" opacity="0.55"/>
    <line x1="231.43" y1="21.75" x2="233.34" y2="10.92" stroke="#4A3410" stroke-width="1.1" opacity="0.55"/>
    <line x1="243.79" y1="24.38" x2="246.45" y2="13.70" stroke="#4A3410" stroke-width="1.1" opacity="0.55"/>
    <line x1="255.93" y1="27.86" x2="259.33" y2="17.40" stroke="#4A3410" stroke-width="1.1" opacity="0.55"/>
    <line x1="267.80" y1="32.18" x2="271.92" y2="21.98" stroke="#4A3410" stroke-width="1.1" opacity="0.55"/>
    <line x1="279.35" y1="37.32" x2="284.17" y2="27.43" stroke="#4A3410" stroke-width="1.1" opacity="0.55"/>
    <line x1="290.50" y1="43.25" x2="296.00" y2="33.72" stroke="#4A3410" stroke-width="1.1" opacity="0.55"/>
    <line x1="301.21" y1="49.94" x2="307.37" y2="40.82" stroke="#4A3410" stroke-width="1.1" opacity="0.55"/>
    <line x1="311.43" y1="57.37" x2="318.21" y2="48.70" stroke="#4A3410" stroke-width="1.1" opacity="0.55"/>
    <line x1="321.11" y1="65.49" x2="328.47" y2="57.32" stroke="#4A3410" stroke-width="1.1" opacity="0.55"/>
    <line x1="330.20" y1="74.27" x2="338.11" y2="66.63" stroke="#4A3410" stroke-width="1.1" opacity="0.55"/>
    <line x1="338.65" y1="83.66" x2="347.08" y2="76.58" stroke="#4A3410" stroke-width="1.1" opacity="0.55"/>
    <line x1="346.43" y1="93.61" x2="355.33" y2="87.15" stroke="#4A3410" stroke-width="1.1" opacity="0.55"/>
    <line x1="353.50" y1="104.08" x2="362.83" y2="98.26" stroke="#4A3410" stroke-width="1.1" opacity="0.55"/>
    <line x1="359.81" y1="115.03" x2="369.53" y2="109.86" stroke="#4A3410" stroke-width="1.1" opacity="0.55"/>
    <line x1="365.35" y1="126.38" x2="375.40" y2="121.91" stroke="#4A3410" stroke-width="1.1" opacity="0.55"/>
    <line x1="370.08" y1="138.09" x2="380.42" y2="134.33" stroke="#4A3410" stroke-width="1.1" opacity="0.55"/>
    <line x1="373.99" y1="150.11" x2="384.56" y2="147.08" stroke="#4A3410" stroke-width="1.1" opacity="0.55"/>
    <line x1="377.04" y1="162.37" x2="387.80" y2="160.08" stroke="#4A3410" stroke-width="1.1" opacity="0.55"/>
    <line x1="379.24" y1="174.81" x2="390.13" y2="173.28" stroke="#4A3410" stroke-width="1.1" opacity="0.55"/>
    <line x1="380.56" y1="187.37" x2="391.53" y2="186.61" stroke="#4A3410" stroke-width="1.1" opacity="0.55"/>
  </g>
  <!-- beaded ring -->
  <g>
    <circle cx="387.00" cy="200.00" r="2.1" fill="url(#goldText)"/>
    <circle cx="386.29" cy="216.30" r="2.1" fill="url(#goldText)"/>
    <circle cx="384.16" cy="232.47" r="2.1" fill="url(#goldText)"/>
    <circle cx="380.63" cy="248.40" r="2.1" fill="url(#goldText)"/>
    <circle cx="375.72" cy="263.96" r="2.1" fill="url(#goldText)"/>
    <circle cx="369.48" cy="279.03" r="2.1" fill="url(#goldText)"/>
    <circle cx="361.95" cy="293.50" r="2.1" fill="url(#goldText)"/>
    <circle cx="353.18" cy="307.26" r="2.1" fill="url(#goldText)"/>
    <circle cx="343.25" cy="320.20" r="2.1" fill="url(#goldText)"/>
    <circle cx="332.23" cy="332.23" r="2.1" fill="url(#goldText)"/>
    <circle cx="320.20" cy="343.25" r="2.1" fill="url(#goldText)"/>
    <circle cx="307.26" cy="353.18" r="2.1" fill="url(#goldText)"/>
    <circle cx="293.50" cy="361.95" r="2.1" fill="url(#goldText)"/>
    <circle cx="279.03" cy="369.48" r="2.1" fill="url(#goldText)"/>
    <circle cx="263.96" cy="375.72" r="2.1" fill="url(#goldText)"/>
    <circle cx="248.40" cy="380.63" r="2.1" fill="url(#goldText)"/>
    <circle cx="232.47" cy="384.16" r="2.1" fill="url(#goldText)"/>
    <circle cx="216.30" cy="386.29" r="2.1" fill="url(#goldText)"/>
    <circle cx="200.00" cy="387.00" r="2.1" fill="url(#goldText)"/>
    <circle cx="183.70" cy="386.29" r="2.1" fill="url(#goldText)"/>
    <circle cx="167.53" cy="384.16" r="2.1" fill="url(#goldText)"/>
    <circle cx="151.60" cy="380.63" r="2.1" fill="url(#goldText)"/>
    <circle cx="136.04" cy="375.72" r="2.1" fill="url(#goldText)"/>
    <circle cx="120.97" cy="369.48" r="2.1" fill="url(#goldText)"/>
    <circle cx="106.50" cy="361.95" r="2.1" fill="url(#goldText)"/>
    <circle cx="92.74" cy="353.18" r="2.1" fill="url(#goldText)"/>
    <circle cx="79.80" cy="343.25" r="2.1" fill="url(#goldText)"/>
    <circle cx="67.77" cy="332.23" r="2.1" fill="url(#goldText)"/>
    <circle cx="56.75" cy="320.20" r="2.1" fill="url(#goldText)"/>
    <circle cx="46.82" cy="307.26" r="2.1" fill="url(#goldText)"/>
    <circle cx="38.05" cy="293.50" r="2.1" fill="url(#goldText)"/>
    <circle cx="30.52" cy="279.03" r="2.1" fill="url(#goldText)"/>
    <circle cx="24.28" cy="263.96" r="2.1" fill="url(#goldText)"/>
    <circle cx="19.37" cy="248.40" r="2.1" fill="url(#goldText)"/>
    <circle cx="15.84" cy="232.47" r="2.1" fill="url(#goldText)"/>
    <circle cx="13.71" cy="216.30" r="2.1" fill="url(#goldText)"/>
    <circle cx="13.00" cy="200.00" r="2.1" fill="url(#goldText)"/>
    <circle cx="13.71" cy="183.70" r="2.1" fill="url(#goldText)"/>
    <circle cx="15.84" cy="167.53" r="2.1" fill="url(#goldText)"/>
    <circle cx="19.37" cy="151.60" r="2.1" fill="url(#goldText)"/>
    <circle cx="24.28" cy="136.04" r="2.1" fill="url(#goldText)"/>
    <circle cx="30.52" cy="120.97" r="2.1" fill="url(#goldText)"/>
    <circle cx="38.05" cy="106.50" r="2.1" fill="url(#goldText)"/>
    <circle cx="46.82" cy="92.74" r="2.1" fill="url(#goldText)"/>
    <circle cx="56.75" cy="79.80" r="2.1" fill="url(#goldText)"/>
    <circle cx="67.77" cy="67.77" r="2.1" fill="url(#goldText)"/>
    <circle cx="79.80" cy="56.75" r="2.1" fill="url(#goldText)"/>
    <circle cx="92.74" cy="46.82" r="2.1" fill="url(#goldText)"/>
    <circle cx="106.50" cy="38.05" r="2.1" fill="url(#goldText)"/>
    <circle cx="120.97" cy="30.52" r="2.1" fill="url(#goldText)"/>
    <circle cx="136.04" cy="24.28" r="2.1" fill="url(#goldText)"/>
    <circle cx="151.60" cy="19.37" r="2.1" fill="url(#goldText)"/>
    <circle cx="167.53" cy="15.84" r="2.1" fill="url(#goldText)"/>
    <circle cx="183.70" cy="13.71" r="2.1" fill="url(#goldText)"/>
    <circle cx="200.00" cy="13.00" r="2.1" fill="url(#goldText)"/>
    <circle cx="216.30" cy="13.71" r="2.1" fill="url(#goldText)"/>
    <circle cx="232.47" cy="15.84" r="2.1" fill="url(#goldText)"/>
    <circle cx="248.40" cy="19.37" r="2.1" fill="url(#goldText)"/>
    <circle cx="263.96" cy="24.28" r="2.1" fill="url(#goldText)"/>
    <circle cx="279.03" cy="30.52" r="2.1" fill="url(#goldText)"/>
    <circle cx="293.50" cy="38.05" r="2.1" fill="url(#goldText)"/>
    <circle cx="307.26" cy="46.82" r="2.1" fill="url(#goldText)"/>
    <circle cx="320.20" cy="56.75" r="2.1" fill="url(#goldText)"/>
    <circle cx="332.23" cy="67.77" r="2.1" fill="url(#goldText)"/>
    <circle cx="343.25" cy="79.80" r="2.1" fill="url(#goldText)"/>
    <circle cx="353.18" cy="92.74" r="2.1" fill="url(#goldText)"/>
    <circle cx="361.95" cy="106.50" r="2.1" fill="url(#goldText)"/>
    <circle cx="369.48" cy="120.97" r="2.1" fill="url(#goldText)"/>
    <circle cx="375.72" cy="136.04" r="2.1" fill="url(#goldText)"/>
    <circle cx="380.63" cy="151.60" r="2.1" fill="url(#goldText)"/>
    <circle cx="384.16" cy="167.53" r="2.1" fill="url(#goldText)"/>
    <circle cx="386.29" cy="183.70" r="2.1" fill="url(#goldText)"/>
  </g>
  <circle cx="200" cy="200" r="183" fill="none" stroke="#FCEBB6" stroke-width="1" stroke-opacity="0.55"/>
  <circle cx="200" cy="200" r="179" fill="none" stroke="#071322" stroke-width="3"/>

  <!-- navy field -->
  <circle cx="200" cy="200" r="176" fill="url(#navyField)"/>
  <!-- inner thin gold ring -->
  <circle cx="200" cy="200" r="140" fill="none" stroke="url(#goldText)" stroke-width="2"/>

  <!-- flanking dots -->
  <circle cx="51.5" cy="146.0" r="2.8" fill="#E0B454"/>
  <circle cx="348.5" cy="146.0" r="2.8" fill="#E0B454"/>

  <!-- arched top text: company name (faux emboss: shadow + gold) -->
  <text font-family="Liberation Serif" font-weight="bold" font-size="28" letter-spacing="3.6" fill="#04101c">
    <textPath href="#arcTop3" startOffset="50%" text-anchor="middle" dy="1.6">LA SOLUCIÓN DE LEO</textPath>
  </text>
  <text font-family="Liberation Serif" font-weight="bold" font-size="28" letter-spacing="3.6" fill="url(#goldText)">
    <textPath href="#arcTop3" startOffset="50%" text-anchor="middle">LA SOLUCIÓN DE LEO</textPath>
  </text>

  <!-- arched bottom text: LICENSED AND BONDED -->
  <text font-family="Liberation Serif" font-weight="bold" font-size="14" letter-spacing="2.2" fill="#04101c">
    <textPath href="#arcBottom3" startOffset="50%" text-anchor="middle" dy="1.4">LICENSED AND BONDED</textPath>
  </text>
  <text font-family="Liberation Serif" font-weight="bold" font-size="14" letter-spacing="2.2" fill="url(#goldText)">
    <textPath href="#arcBottom3" startOffset="50%" text-anchor="middle">LICENSED AND BONDED</textPath>
  </text>

  <!-- monogram group -->
  <g transform="translate(200,192)">
    <!-- feather quill: detailed plume with barbs, angled up-right off second L -->
    <g transform="translate(44,-44) rotate(28) scale(0.72)">
      <path d="M0,2 C 6,-28 4,-58 -10,-84 C -2,-58 -6,-38 -18,-20
               C -12,-24 -4,-20 0,-10 C 4,-2 2,4 0,2 Z"
            fill="url(#goldText)" stroke="#5C4310" stroke-width="0.8"/>
      <!-- barb lines -->
      <path d="M -6,-6 C -10,-16 -16,-24 -22,-30" stroke="#5C4310" stroke-width="0.6" fill="none" opacity="0.7"/>
      <path d="M -4,-16 C -8,-26 -13,-34 -19,-42" stroke="#5C4310" stroke-width="0.6" fill="none" opacity="0.7"/>
      <path d="M -3,-28 C -6,-38 -10,-46 -15,-54" stroke="#5C4310" stroke-width="0.6" fill="none" opacity="0.7"/>
      <path d="M -2,-40 C -4,-50 -7,-58 -11,-66" stroke="#5C4310" stroke-width="0.6" fill="none" opacity="0.7"/>
      <path d="M -1,-52 C -3,-61 -5,-68 -8,-76" stroke="#5C4310" stroke-width="0.6" fill="none" opacity="0.7"/>
      <path d="M -10,-84 L 8,6" stroke="#5C4310" stroke-width="1.1" fill="none"/>
      <!-- pen shaft -->
      <line x1="4" y1="-2" x2="30" y2="24" stroke="url(#goldText)" stroke-width="3.6" stroke-linecap="round"/>
      <!-- ink swirl at nib -->
      <path d="M 30,24 C 38,26 42,32 38,38 C 34,43 26,41 26,35" fill="none" stroke="url(#goldText)" stroke-width="2.4" stroke-linecap="round"/>
    </g>

    <!-- monogram L S L with faux-emboss shadow -->
    <g transform="translate(1.6,2.4)" fill="#04101c" opacity="0.55">
      <text x="-58" y="34" font-family="Liberation Serif" font-weight="bold" font-size="112" text-anchor="middle">L</text>
      <text x="0" y="20" font-family="Liberation Serif" font-weight="bold" font-size="68" text-anchor="middle">S</text>
      <text x="55" y="34" font-family="Liberation Serif" font-weight="bold" font-size="112" text-anchor="middle">L</text>
    </g>
    <text x="-58" y="34" font-family="Liberation Serif" font-weight="bold" font-size="112" fill="url(#goldText)" text-anchor="middle">L</text>
    <text x="0" y="20" font-family="Liberation Serif" font-weight="bold" font-size="68" fill="url(#goldText)" text-anchor="middle">S</text>
    <text x="55" y="34" font-family="Liberation Serif" font-weight="bold" font-size="112" fill="url(#goldText)" text-anchor="middle">L</text>

    <!-- pillar icon -->
    <g transform="translate(0,64)">
      <g transform="translate(1.4,2)" fill="#04101c" opacity="0.5">
        <rect x="-30" y="0" width="60" height="7" rx="1.5"/>
        <rect x="-24" y="7" width="48" height="4"/>
        <rect x="-19" y="11" width="6" height="26"/>
        <rect x="-6.5" y="11" width="6" height="26"/>
        <rect x="6" y="11" width="6" height="26"/>
        <rect x="18.5" y="11" width="6" height="26"/>
        <rect x="-24" y="37" width="48" height="4"/>
        <rect x="-30" y="41" width="60" height="7" rx="1.5"/>
      </g>
      <g fill="url(#goldText)">
        <rect x="-30" y="0" width="60" height="7" rx="1.5"/>
        <rect x="-24" y="7" width="48" height="4"/>
        <rect x="-19" y="11" width="6" height="26"/>
        <rect x="-6.5" y="11" width="6" height="26"/>
        <rect x="6" y="11" width="6" height="26"/>
        <rect x="18.5" y="11" width="6" height="26"/>
        <rect x="-24" y="37" width="48" height="4"/>
        <rect x="-30" y="41" width="60" height="7" rx="1.5"/>
      </g>
    </g>
  </g>
</svg>


    </div>
  </div>
</header>

<!-- ================= TRUST STRIP ================= -->
<div class="trust-strip">
  <div class="wrap">
    <span class="item">✅ Licenciado y Afianzado · Licensed &amp; Bonded</span>
    <span class="item">🚗 Servicio Móvil · Mobile Service</span>
    <span class="item">🗣️ Se Habla Español · English Spoken</span>
    <span class="item">📄 Trabajo Garantizado · Work Guaranteed</span>
  </div>
</div>

<!-- ================= SERVICES ================= -->
<section id="servicios">
  <div class="wrap">
    <div class="section-head">
      <span class="eyebrow">Nuestros servicios</span>
      <h2>Todo lo que necesita, en un solo lugar</h2>
      <p>Everything you need, in one place. Servicio personal y en español para trámites de notaría, gobierno, impuestos y más.</p>
    </div>

    <div class="services-grid">
      <div class="svc-card">
        <span class="num">01</span>
        <h3>Notaría y Documentos Legales</h3>
        <p class="en">Notary &amp; legal documents</p>
        <ul>
          <li>Servicios Notariales <span class="li-en">(Notary Services)</span></li>
          <li>Cartas de Permiso de Viaje <span class="li-en">(Travel Letters)</span></li>
          <li>Poder Notarial <span class="li-en">(Power of Attorney)</span></li>
          <li>Apostillas <span class="li-en">(Apostilles)</span></li>
        </ul>
      </div>

      <div class="svc-card">
        <span class="num">02</span>
        <h3>Beneficios y Gobierno</h3>
        <p class="en">Government &amp; benefits assistance</p>
        <ul>
          <li>Desempleo <span class="li-en">(Unemployment / EDD)</span></li>
          <li>Incapacidad / Permiso Familiar <span class="li-en">(Disability / FPL)</span></li>
          <li>Seguro Social — Retiro <span class="li-en">(Social Security)</span></li>
        </ul>
      </div>

      <div class="svc-card">
        <span class="num">03</span>
        <h3>Impuestos y Traducción</h3>
        <p class="en">Taxes &amp; document translation</p>
        <ul>
          <li>Declaración de Impuestos <span class="li-en">(Tax Returns, W-2)</span></li>
          <li>Impuestos de Pequeños Negocios <span class="li-en">(Small Business Taxes)</span></li>
          <li>Traducción de Documentos <span class="li-en">(Document Translation)</span></li>
        </ul>
      </div>

      <div class="svc-card">
        <span class="num">04</span>
        <h3>Viajes, Vehículos y Más</h3>
        <p class="en">Travel, vehicles &amp; more</p>
        <ul>
          <li>Renovación de Pasaporte <span class="li-en">(Passport Renewal)</span></li>
          <li>Retiro de Vehículo <span class="li-en">(Vehicle Retirement)</span></li>
          <li>Seguro de Renta <span class="li-en">(Renters Insurance)</span></li>
          <li>Llenado de Cualquier Formulario <span class="li-en">(Any Form/Document)</span></li>
        </ul>
      </div>
    </div>

    <div class="soon-banner">
      <div>
        <strong>Próximamente: Inmigración y DMV</strong>
        <span>Coming soon — immigration and DMV services. Call to be the first to know.</span>
      </div>
      <a class="btn btn-primary" href="tel:+14086134713">Llamar ahora</a>
    </div>
  </div>
</section>

<!-- ================= WHY US ================= -->
<section class="why">
  <div class="wrap">
    <div class="section-head">
      <span class="eyebrow">¿Por qué elegirnos?</span>
      <h2>Un servicio honesto, cerca de casa</h2>
      <p>An honest, personal service — close to home.</p>
    </div>
    <div class="why-grid">
      <div class="why-item">
        <div class="ic">🏠</div>
        <h3>Venimos a Usted</h3>
        <p>Sin necesidad de faltar al trabajo — le visitamos en su hogar u oficina.</p>
        <p class="why-en">We come to you — no need to miss work.</p>
      </div>
      <div class="why-item">
        <div class="ic">🛡️</div>
        <h3>Licenciado y Afianzado</h3>
        <p>Notary Public con comisión vigente del estado de California, verificable ante la Secretaría de Estado.</p>
        <p class="why-en">Licensed &amp; bonded, verifiable with the CA Secretary of State.</p>
      </div>
      <div class="why-item">
        <div class="ic">🗣️</div>
        <h3>Se Habla Español</h3>
        <p>Comunicación clara, en su idioma, sin malentendidos.</p>
        <p class="why-en">Clear communication, in your language — no misunderstandings.</p>
      </div>
      <div class="why-item">
        <div class="ic">✔️</div>
        <h3>Trabajo Garantizado</h3>
        <p>Hacemos las cosas bien la primera vez — o lo corregimos sin costo extra.</p>
        <p class="why-en">We do it right the first time — or we fix it at no extra cost.</p>
      </div>
    </div>
  </div>
</section>

<!-- ================= SERVICE AREA ================= -->
<section id="area">
  <div class="wrap area">
    <div>
      <span class="eyebrow">Área de servicio</span>
      <h2 style="font-size:clamp(24px,3vw,32px);color:var(--navy);margin:8px 0 10px;font-weight:800;">Sirviendo el Gran Sacramento</h2>
      <p style="color:var(--muted);font-size:15px;margin:0 0 4px;">Serving Greater Sacramento — mobile service within a 30-mile radius, with a focus on South Sacramento.</p>
      <div class="area-list">
        <span class="main">Sur de Sacramento · South Sac.</span>
        <span>Elk Grove</span>
        <span>Natomas</span>
        <span>Carmichael</span>
        <span>Roseville</span>
        <span>Folsom</span>
        <span>East Sacramento</span>
        <span>West Sacramento</span>
        <span>Del Paso Heights</span>
        <span>Citrus Heights</span>
      </div>
    </div>
    <div class="radius-card">
      <div class="miles">30<sup>mi</sup></div>
      <p>Radio de servicio móvil desde el centro de Sacramento<br>Mobile service radius from downtown Sacramento</p>
    </div>
  </div>
</section>

<!-- ================= CTA ================= -->
<section class="cta">
  <div class="wrap">
    <span class="eyebrow">Contáctenos hoy</span>
    <h2>¿Listo para empezar?</h2>
    <p class="sub-en">Ready to get started? Call or text — most requests answered the same day.</p>
    <a class="phone-big" href="tel:+14086134713">(408) 613-4713</a>
    <a class="email-big" href="mailto:lasoluciondeleo@gmail.com">✉️ lasoluciondeleo@gmail.com</a>
    <div class="cta-row">
      <a class="btn btn-primary" href="tel:+14086134713">📞 Llamar / Call</a>
      <a class="btn btn-ghost" href="sms:+14086134713">💬 Enviar Texto / Text Us</a>
    </div>
  </div>
</section>

<!-- ================= FOOTER ================= -->
<footer>
  <div class="wrap footer-grid">
    <div>
      <a class="brand" href="#top" style="display:flex;align-items:center;gap:10px;text-decoration:none;">
        <svg viewBox="0 0 400 400" xmlns="http://www.w3.org/2000/svg">
  <defs>
    <linearGradient id="goldRingft" x1="15%" y1="10%" x2="85%" y2="95%">
      <stop offset="0%" stop-color="#FCEBB6"/>
      <stop offset="14%" stop-color="#F3D276"/>
      <stop offset="30%" stop-color="#C9972E"/>
      <stop offset="42%" stop-color="#8F6A1D"/>
      <stop offset="50%" stop-color="#FCEBB6"/>
      <stop offset="64%" stop-color="#E8BE5E"/>
      <stop offset="80%" stop-color="#B5872A"/>
      <stop offset="100%" stop-color="#6B4E15"/>
    </linearGradient>
    <linearGradient id="goldTextft" x1="0%" y1="0%" x2="0%" y2="100%">
      <stop offset="0%" stop-color="#FCEBB6"/>
      <stop offset="45%" stop-color="#E0B454"/>
      <stop offset="100%" stop-color="#9C7420"/>
    </linearGradient>
    <radialGradient id="navyFieldft" cx="42%" cy="32%" r="78%">
      <stop offset="0%" stop-color="#16324E"/>
      <stop offset="60%" stop-color="#0B2036"/>
      <stop offset="100%" stop-color="#071322"/>
    </radialGradient>
    <path id="arcTop3ft" d="M 59.0,148.7 A 150,150 0 0 1 341.0,148.7" />
    <path id="arcBottom3ft" d="M 70.6,290.6 A 158,158 0 0 0 329.4,290.6" />
  </defs>

  <!-- outer gold ring (embossed, coin-edge style) -->
  <circle cx="200" cy="200" r="194" fill="url(#goldRingft)"/>
  <circle cx="200" cy="200" r="194" fill="none" stroke="#4A3410" stroke-width="1"/>
  <!-- fluted / reeded texture -->
  <g>
    <line x1="381.00" y1="200.00" x2="392.00" y2="200.00" stroke="#4A3410" stroke-width="1.1" opacity="0.55"/>
    <line x1="380.56" y1="212.63" x2="391.53" y2="213.39" stroke="#4A3410" stroke-width="1.1" opacity="0.55"/>
    <line x1="379.24" y1="225.19" x2="390.13" y2="226.72" stroke="#4A3410" stroke-width="1.1" opacity="0.55"/>
    <line x1="377.04" y1="237.63" x2="387.80" y2="239.92" stroke="#4A3410" stroke-width="1.1" opacity="0.55"/>
    <line x1="373.99" y1="249.89" x2="384.56" y2="252.92" stroke="#4A3410" stroke-width="1.1" opacity="0.55"/>
    <line x1="370.08" y1="261.91" x2="380.42" y2="265.67" stroke="#4A3410" stroke-width="1.1" opacity="0.55"/>
    <line x1="365.35" y1="273.62" x2="375.40" y2="278.09" stroke="#4A3410" stroke-width="1.1" opacity="0.55"/>
    <line x1="359.81" y1="284.97" x2="369.53" y2="290.14" stroke="#4A3410" stroke-width="1.1" opacity="0.55"/>
    <line x1="353.50" y1="295.92" x2="362.83" y2="301.74" stroke="#4A3410" stroke-width="1.1" opacity="0.55"/>
    <line x1="346.43" y1="306.39" x2="355.33" y2="312.85" stroke="#4A3410" stroke-width="1.1" opacity="0.55"/>
    <line x1="338.65" y1="316.34" x2="347.08" y2="323.42" stroke="#4A3410" stroke-width="1.1" opacity="0.55"/>
    <line x1="330.20" y1="325.73" x2="338.11" y2="333.37" stroke="#4A3410" stroke-width="1.1" opacity="0.55"/>
    <line x1="321.11" y1="334.51" x2="328.47" y2="342.68" stroke="#4A3410" stroke-width="1.1" opacity="0.55"/>
    <line x1="311.43" y1="342.63" x2="318.21" y2="351.30" stroke="#4A3410" stroke-width="1.1" opacity="0.55"/>
    <line x1="301.21" y1="350.06" x2="307.37" y2="359.18" stroke="#4A3410" stroke-width="1.1" opacity="0.55"/>
    <line x1="290.50" y1="356.75" x2="296.00" y2="366.28" stroke="#4A3410" stroke-width="1.1" opacity="0.55"/>
    <line x1="279.35" y1="362.68" x2="284.17" y2="372.57" stroke="#4A3410" stroke-width="1.1" opacity="0.55"/>
    <line x1="267.80" y1="367.82" x2="271.92" y2="378.02" stroke="#4A3410" stroke-width="1.1" opacity="0.55"/>
    <line x1="255.93" y1="372.14" x2="259.33" y2="382.60" stroke="#4A3410" stroke-width="1.1" opacity="0.55"/>
    <line x1="243.79" y1="375.62" x2="246.45" y2="386.30" stroke="#4A3410" stroke-width="1.1" opacity="0.55"/>
    <line x1="231.43" y1="378.25" x2="233.34" y2="389.08" stroke="#4A3410" stroke-width="1.1" opacity="0.55"/>
    <line x1="218.92" y1="380.01" x2="220.07" y2="390.95" stroke="#4A3410" stroke-width="1.1" opacity="0.55"/>
    <line x1="206.32" y1="380.89" x2="206.70" y2="391.88" stroke="#4A3410" stroke-width="1.1" opacity="0.55"/>
    <line x1="193.68" y1="380.89" x2="193.30" y2="391.88" stroke="#4A3410" stroke-width="1.1" opacity="0.55"/>
    <line x1="181.08" y1="380.01" x2="179.93" y2="390.95" stroke="#4A3410" stroke-width="1.1" opacity="0.55"/>
    <line x1="168.57" y1="378.25" x2="166.66" y2="389.08" stroke="#4A3410" stroke-width="1.1" opacity="0.55"/>
    <line x1="156.21" y1="375.62" x2="153.55" y2="386.30" stroke="#4A3410" stroke-width="1.1" opacity="0.55"/>
    <line x1="144.07" y1="372.14" x2="140.67" y2="382.60" stroke="#4A3410" stroke-width="1.1" opacity="0.55"/>
    <line x1="132.20" y1="367.82" x2="128.08" y2="378.02" stroke="#4A3410" stroke-width="1.1" opacity="0.55"/>
    <line x1="120.65" y1="362.68" x2="115.83" y2="372.57" stroke="#4A3410" stroke-width="1.1" opacity="0.55"/>
    <line x1="109.50" y1="356.75" x2="104.00" y2="366.28" stroke="#4A3410" stroke-width="1.1" opacity="0.55"/>
    <line x1="98.79" y1="350.06" x2="92.63" y2="359.18" stroke="#4A3410" stroke-width="1.1" opacity="0.55"/>
    <line x1="88.57" y1="342.63" x2="81.79" y2="351.30" stroke="#4A3410" stroke-width="1.1" opacity="0.55"/>
    <line x1="78.89" y1="334.51" x2="71.53" y2="342.68" stroke="#4A3410" stroke-width="1.1" opacity="0.55"/>
    <line x1="69.80" y1="325.73" x2="61.89" y2="333.37" stroke="#4A3410" stroke-width="1.1" opacity="0.55"/>
    <line x1="61.35" y1="316.34" x2="52.92" y2="323.42" stroke="#4A3410" stroke-width="1.1" opacity="0.55"/>
    <line x1="53.57" y1="306.39" x2="44.67" y2="312.85" stroke="#4A3410" stroke-width="1.1" opacity="0.55"/>
    <line x1="46.50" y1="295.92" x2="37.17" y2="301.74" stroke="#4A3410" stroke-width="1.1" opacity="0.55"/>
    <line x1="40.19" y1="284.97" x2="30.47" y2="290.14" stroke="#4A3410" stroke-width="1.1" opacity="0.55"/>
    <line x1="34.65" y1="273.62" x2="24.60" y2="278.09" stroke="#4A3410" stroke-width="1.1" opacity="0.55"/>
    <line x1="29.92" y1="261.91" x2="19.58" y2="265.67" stroke="#4A3410" stroke-width="1.1" opacity="0.55"/>
    <line x1="26.01" y1="249.89" x2="15.44" y2="252.92" stroke="#4A3410" stroke-width="1.1" opacity="0.55"/>
    <line x1="22.96" y1="237.63" x2="12.20" y2="239.92" stroke="#4A3410" stroke-width="1.1" opacity="0.55"/>
    <line x1="20.76" y1="225.19" x2="9.87" y2="226.72" stroke="#4A3410" stroke-width="1.1" opacity="0.55"/>
    <line x1="19.44" y1="212.63" x2="8.47" y2="213.39" stroke="#4A3410" stroke-width="1.1" opacity="0.55"/>
    <line x1="19.00" y1="200.00" x2="8.00" y2="200.00" stroke="#4A3410" stroke-width="1.1" opacity="0.55"/>
    <line x1="19.44" y1="187.37" x2="8.47" y2="186.61" stroke="#4A3410" stroke-width="1.1" opacity="0.55"/>
    <line x1="20.76" y1="174.81" x2="9.87" y2="173.28" stroke="#4A3410" stroke-width="1.1" opacity="0.55"/>
    <line x1="22.96" y1="162.37" x2="12.20" y2="160.08" stroke="#4A3410" stroke-width="1.1" opacity="0.55"/>
    <line x1="26.01" y1="150.11" x2="15.44" y2="147.08" stroke="#4A3410" stroke-width="1.1" opacity="0.55"/>
    <line x1="29.92" y1="138.09" x2="19.58" y2="134.33" stroke="#4A3410" stroke-width="1.1" opacity="0.55"/>
    <line x1="34.65" y1="126.38" x2="24.60" y2="121.91" stroke="#4A3410" stroke-width="1.1" opacity="0.55"/>
    <line x1="40.19" y1="115.03" x2="30.47" y2="109.86" stroke="#4A3410" stroke-width="1.1" opacity="0.55"/>
    <line x1="46.50" y1="104.08" x2="37.17" y2="98.26" stroke="#4A3410" stroke-width="1.1" opacity="0.55"/>
    <line x1="53.57" y1="93.61" x2="44.67" y2="87.15" stroke="#4A3410" stroke-width="1.1" opacity="0.55"/>
    <line x1="61.35" y1="83.66" x2="52.92" y2="76.58" stroke="#4A3410" stroke-width="1.1" opacity="0.55"/>
    <line x1="69.80" y1="74.27" x2="61.89" y2="66.63" stroke="#4A3410" stroke-width="1.1" opacity="0.55"/>
    <line x1="78.89" y1="65.49" x2="71.53" y2="57.32" stroke="#4A3410" stroke-width="1.1" opacity="0.55"/>
    <line x1="88.57" y1="57.37" x2="81.79" y2="48.70" stroke="#4A3410" stroke-width="1.1" opacity="0.55"/>
    <line x1="98.79" y1="49.94" x2="92.63" y2="40.82" stroke="#4A3410" stroke-width="1.1" opacity="0.55"/>
    <line x1="109.50" y1="43.25" x2="104.00" y2="33.72" stroke="#4A3410" stroke-width="1.1" opacity="0.55"/>
    <line x1="120.65" y1="37.32" x2="115.83" y2="27.43" stroke="#4A3410" stroke-width="1.1" opacity="0.55"/>
    <line x1="132.20" y1="32.18" x2="128.08" y2="21.98" stroke="#4A3410" stroke-width="1.1" opacity="0.55"/>
    <line x1="144.07" y1="27.86" x2="140.67" y2="17.40" stroke="#4A3410" stroke-width="1.1" opacity="0.55"/>
    <line x1="156.21" y1="24.38" x2="153.55" y2="13.70" stroke="#4A3410" stroke-width="1.1" opacity="0.55"/>
    <line x1="168.57" y1="21.75" x2="166.66" y2="10.92" stroke="#4A3410" stroke-width="1.1" opacity="0.55"/>
    <line x1="181.08" y1="19.99" x2="179.93" y2="9.05" stroke="#4A3410" stroke-width="1.1" opacity="0.55"/>
    <line x1="193.68" y1="19.11" x2="193.30" y2="8.12" stroke="#4A3410" stroke-width="1.1" opacity="0.55"/>
    <line x1="206.32" y1="19.11" x2="206.70" y2="8.12" stroke="#4A3410" stroke-width="1.1" opacity="0.55"/>
    <line x1="218.92" y1="19.99" x2="220.07" y2="9.05" stroke="#4A3410" stroke-width="1.1" opacity="0.55"/>
    <line x1="231.43" y1="21.75" x2="233.34" y2="10.92" stroke="#4A3410" stroke-width="1.1" opacity="0.55"/>
    <line x1="243.79" y1="24.38" x2="246.45" y2="13.70" stroke="#4A3410" stroke-width="1.1" opacity="0.55"/>
    <line x1="255.93" y1="27.86" x2="259.33" y2="17.40" stroke="#4A3410" stroke-width="1.1" opacity="0.55"/>
    <line x1="267.80" y1="32.18" x2="271.92" y2="21.98" stroke="#4A3410" stroke-width="1.1" opacity="0.55"/>
    <line x1="279.35" y1="37.32" x2="284.17" y2="27.43" stroke="#4A3410" stroke-width="1.1" opacity="0.55"/>
    <line x1="290.50" y1="43.25" x2="296.00" y2="33.72" stroke="#4A3410" stroke-width="1.1" opacity="0.55"/>
    <line x1="301.21" y1="49.94" x2="307.37" y2="40.82" stroke="#4A3410" stroke-width="1.1" opacity="0.55"/>
    <line x1="311.43" y1="57.37" x2="318.21" y2="48.70" stroke="#4A3410" stroke-width="1.1" opacity="0.55"/>
    <line x1="321.11" y1="65.49" x2="328.47" y2="57.32" stroke="#4A3410" stroke-width="1.1" opacity="0.55"/>
    <line x1="330.20" y1="74.27" x2="338.11" y2="66.63" stroke="#4A3410" stroke-width="1.1" opacity="0.55"/>
    <line x1="338.65" y1="83.66" x2="347.08" y2="76.58" stroke="#4A3410" stroke-width="1.1" opacity="0.55"/>
    <line x1="346.43" y1="93.61" x2="355.33" y2="87.15" stroke="#4A3410" stroke-width="1.1" opacity="0.55"/>
    <line x1="353.50" y1="104.08" x2="362.83" y2="98.26" stroke="#4A3410" stroke-width="1.1" opacity="0.55"/>
    <line x1="359.81" y1="115.03" x2="369.53" y2="109.86" stroke="#4A3410" stroke-width="1.1" opacity="0.55"/>
    <line x1="365.35" y1="126.38" x2="375.40" y2="121.91" stroke="#4A3410" stroke-width="1.1" opacity="0.55"/>
    <line x1="370.08" y1="138.09" x2="380.42" y2="134.33" stroke="#4A3410" stroke-width="1.1" opacity="0.55"/>
    <line x1="373.99" y1="150.11" x2="384.56" y2="147.08" stroke="#4A3410" stroke-width="1.1" opacity="0.55"/>
    <line x1="377.04" y1="162.37" x2="387.80" y2="160.08" stroke="#4A3410" stroke-width="1.1" opacity="0.55"/>
    <line x1="379.24" y1="174.81" x2="390.13" y2="173.28" stroke="#4A3410" stroke-width="1.1" opacity="0.55"/>
    <line x1="380.56" y1="187.37" x2="391.53" y2="186.61" stroke="#4A3410" stroke-width="1.1" opacity="0.55"/>
  </g>
  <!-- beaded ring -->
  <g>
    <circle cx="387.00" cy="200.00" r="2.1" fill="url(#goldTextft)"/>
    <circle cx="386.29" cy="216.30" r="2.1" fill="url(#goldTextft)"/>
    <circle cx="384.16" cy="232.47" r="2.1" fill="url(#goldTextft)"/>
    <circle cx="380.63" cy="248.40" r="2.1" fill="url(#goldTextft)"/>
    <circle cx="375.72" cy="263.96" r="2.1" fill="url(#goldTextft)"/>
    <circle cx="369.48" cy="279.03" r="2.1" fill="url(#goldTextft)"/>
    <circle cx="361.95" cy="293.50" r="2.1" fill="url(#goldTextft)"/>
    <circle cx="353.18" cy="307.26" r="2.1" fill="url(#goldTextft)"/>
    <circle cx="343.25" cy="320.20" r="2.1" fill="url(#goldTextft)"/>
    <circle cx="332.23" cy="332.23" r="2.1" fill="url(#goldTextft)"/>
    <circle cx="320.20" cy="343.25" r="2.1" fill="url(#goldTextft)"/>
    <circle cx="307.26" cy="353.18" r="2.1" fill="url(#goldTextft)"/>
    <circle cx="293.50" cy="361.95" r="2.1" fill="url(#goldTextft)"/>
    <circle cx="279.03" cy="369.48" r="2.1" fill="url(#goldTextft)"/>
    <circle cx="263.96" cy="375.72" r="2.1" fill="url(#goldTextft)"/>
    <circle cx="248.40" cy="380.63" r="2.1" fill="url(#goldTextft)"/>
    <circle cx="232.47" cy="384.16" r="2.1" fill="url(#goldTextft)"/>
    <circle cx="216.30" cy="386.29" r="2.1" fill="url(#goldTextft)"/>
    <circle cx="200.00" cy="387.00" r="2.1" fill="url(#goldTextft)"/>
    <circle cx="183.70" cy="386.29" r="2.1" fill="url(#goldTextft)"/>
    <circle cx="167.53" cy="384.16" r="2.1" fill="url(#goldTextft)"/>
    <circle cx="151.60" cy="380.63" r="2.1" fill="url(#goldTextft)"/>
    <circle cx="136.04" cy="375.72" r="2.1" fill="url(#goldTextft)"/>
    <circle cx="120.97" cy="369.48" r="2.1" fill="url(#goldTextft)"/>
    <circle cx="106.50" cy="361.95" r="2.1" fill="url(#goldTextft)"/>
    <circle cx="92.74" cy="353.18" r="2.1" fill="url(#goldTextft)"/>
    <circle cx="79.80" cy="343.25" r="2.1" fill="url(#goldTextft)"/>
    <circle cx="67.77" cy="332.23" r="2.1" fill="url(#goldTextft)"/>
    <circle cx="56.75" cy="320.20" r="2.1" fill="url(#goldTextft)"/>
    <circle cx="46.82" cy="307.26" r="2.1" fill="url(#goldTextft)"/>
    <circle cx="38.05" cy="293.50" r="2.1" fill="url(#goldTextft)"/>
    <circle cx="30.52" cy="279.03" r="2.1" fill="url(#goldTextft)"/>
    <circle cx="24.28" cy="263.96" r="2.1" fill="url(#goldTextft)"/>
    <circle cx="19.37" cy="248.40" r="2.1" fill="url(#goldTextft)"/>
    <circle cx="15.84" cy="232.47" r="2.1" fill="url(#goldTextft)"/>
    <circle cx="13.71" cy="216.30" r="2.1" fill="url(#goldTextft)"/>
    <circle cx="13.00" cy="200.00" r="2.1" fill="url(#goldTextft)"/>
    <circle cx="13.71" cy="183.70" r="2.1" fill="url(#goldTextft)"/>
    <circle cx="15.84" cy="167.53" r="2.1" fill="url(#goldTextft)"/>
    <circle cx="19.37" cy="151.60" r="2.1" fill="url(#goldTextft)"/>
    <circle cx="24.28" cy="136.04" r="2.1" fill="url(#goldTextft)"/>
    <circle cx="30.52" cy="120.97" r="2.1" fill="url(#goldTextft)"/>
    <circle cx="38.05" cy="106.50" r="2.1" fill="url(#goldTextft)"/>
    <circle cx="46.82" cy="92.74" r="2.1" fill="url(#goldTextft)"/>
    <circle cx="56.75" cy="79.80" r="2.1" fill="url(#goldTextft)"/>
    <circle cx="67.77" cy="67.77" r="2.1" fill="url(#goldTextft)"/>
    <circle cx="79.80" cy="56.75" r="2.1" fill="url(#goldTextft)"/>
    <circle cx="92.74" cy="46.82" r="2.1" fill="url(#goldTextft)"/>
    <circle cx="106.50" cy="38.05" r="2.1" fill="url(#goldTextft)"/>
    <circle cx="120.97" cy="30.52" r="2.1" fill="url(#goldTextft)"/>
    <circle cx="136.04" cy="24.28" r="2.1" fill="url(#goldTextft)"/>
    <circle cx="151.60" cy="19.37" r="2.1" fill="url(#goldTextft)"/>
    <circle cx="167.53" cy="15.84" r="2.1" fill="url(#goldTextft)"/>
    <circle cx="183.70" cy="13.71" r="2.1" fill="url(#goldTextft)"/>
    <circle cx="200.00" cy="13.00" r="2.1" fill="url(#goldTextft)"/>
    <circle cx="216.30" cy="13.71" r="2.1" fill="url(#goldTextft)"/>
    <circle cx="232.47" cy="15.84" r="2.1" fill="url(#goldTextft)"/>
    <circle cx="248.40" cy="19.37" r="2.1" fill="url(#goldTextft)"/>
    <circle cx="263.96" cy="24.28" r="2.1" fill="url(#goldTextft)"/>
    <circle cx="279.03" cy="30.52" r="2.1" fill="url(#goldTextft)"/>
    <circle cx="293.50" cy="38.05" r="2.1" fill="url(#goldTextft)"/>
    <circle cx="307.26" cy="46.82" r="2.1" fill="url(#goldTextft)"/>
    <circle cx="320.20" cy="56.75" r="2.1" fill="url(#goldTextft)"/>
    <circle cx="332.23" cy="67.77" r="2.1" fill="url(#goldTextft)"/>
    <circle cx="343.25" cy="79.80" r="2.1" fill="url(#goldTextft)"/>
    <circle cx="353.18" cy="92.74" r="2.1" fill="url(#goldTextft)"/>
    <circle cx="361.95" cy="106.50" r="2.1" fill="url(#goldTextft)"/>
    <circle cx="369.48" cy="120.97" r="2.1" fill="url(#goldTextft)"/>
    <circle cx="375.72" cy="136.04" r="2.1" fill="url(#goldTextft)"/>
    <circle cx="380.63" cy="151.60" r="2.1" fill="url(#goldTextft)"/>
    <circle cx="384.16" cy="167.53" r="2.1" fill="url(#goldTextft)"/>
    <circle cx="386.29" cy="183.70" r="2.1" fill="url(#goldTextft)"/>
  </g>
  <circle cx="200" cy="200" r="183" fill="none" stroke="#FCEBB6" stroke-width="1" stroke-opacity="0.55"/>
  <circle cx="200" cy="200" r="179" fill="none" stroke="#071322" stroke-width="3"/>

  <!-- navy field -->
  <circle cx="200" cy="200" r="176" fill="url(#navyFieldft)"/>
  <!-- inner thin gold ring -->
  <circle cx="200" cy="200" r="140" fill="none" stroke="url(#goldTextft)" stroke-width="2"/>

  <!-- flanking dots -->
  <circle cx="51.5" cy="146.0" r="2.8" fill="#E0B454"/>
  <circle cx="348.5" cy="146.0" r="2.8" fill="#E0B454"/>

  <!-- arched top text: company name (faux emboss: shadow + gold) -->
  <text font-family="Liberation Serif" font-weight="bold" font-size="28" letter-spacing="3.6" fill="#04101c">
    <textPath href="#arcTop3ft" startOffset="50%" text-anchor="middle" dy="1.6">LA SOLUCIÓN DE LEO</textPath>
  </text>
  <text font-family="Liberation Serif" font-weight="bold" font-size="28" letter-spacing="3.6" fill="url(#goldTextft)">
    <textPath href="#arcTop3ft" startOffset="50%" text-anchor="middle">LA SOLUCIÓN DE LEO</textPath>
  </text>

  <!-- arched bottom text: LICENSED AND BONDED -->
  <text font-family="Liberation Serif" font-weight="bold" font-size="14" letter-spacing="2.2" fill="#04101c">
    <textPath href="#arcBottom3ft" startOffset="50%" text-anchor="middle" dy="1.4">LICENSED AND BONDED</textPath>
  </text>
  <text font-family="Liberation Serif" font-weight="bold" font-size="14" letter-spacing="2.2" fill="url(#goldTextft)">
    <textPath href="#arcBottom3ft" startOffset="50%" text-anchor="middle">LICENSED AND BONDED</textPath>
  </text>

  <!-- monogram group -->
  <g transform="translate(200,192)">
    <!-- feather quill: detailed plume with barbs, angled up-right off second L -->
    <g transform="translate(44,-44) rotate(28) scale(0.72)">
      <path d="M0,2 C 6,-28 4,-58 -10,-84 C -2,-58 -6,-38 -18,-20
               C -12,-24 -4,-20 0,-10 C 4,-2 2,4 0,2 Z"
            fill="url(#goldTextft)" stroke="#5C4310" stroke-width="0.8"/>
      <!-- barb lines -->
      <path d="M -6,-6 C -10,-16 -16,-24 -22,-30" stroke="#5C4310" stroke-width="0.6" fill="none" opacity="0.7"/>
      <path d="M -4,-16 C -8,-26 -13,-34 -19,-42" stroke="#5C4310" stroke-width="0.6" fill="none" opacity="0.7"/>
      <path d="M -3,-28 C -6,-38 -10,-46 -15,-54" stroke="#5C4310" stroke-width="0.6" fill="none" opacity="0.7"/>
      <path d="M -2,-40 C -4,-50 -7,-58 -11,-66" stroke="#5C4310" stroke-width="0.6" fill="none" opacity="0.7"/>
      <path d="M -1,-52 C -3,-61 -5,-68 -8,-76" stroke="#5C4310" stroke-width="0.6" fill="none" opacity="0.7"/>
      <path d="M -10,-84 L 8,6" stroke="#5C4310" stroke-width="1.1" fill="none"/>
      <!-- pen shaft -->
      <line x1="4" y1="-2" x2="30" y2="24" stroke="url(#goldTextft)" stroke-width="3.6" stroke-linecap="round"/>
      <!-- ink swirl at nib -->
      <path d="M 30,24 C 38,26 42,32 38,38 C 34,43 26,41 26,35" fill="none" stroke="url(#goldTextft)" stroke-width="2.4" stroke-linecap="round"/>
    </g>

    <!-- monogram L S L with faux-emboss shadow -->
    <g transform="translate(1.6,2.4)" fill="#04101c" opacity="0.55">
      <text x="-58" y="34" font-family="Liberation Serif" font-weight="bold" font-size="112" text-anchor="middle">L</text>
      <text x="0" y="20" font-family="Liberation Serif" font-weight="bold" font-size="68" text-anchor="middle">S</text>
      <text x="55" y="34" font-family="Liberation Serif" font-weight="bold" font-size="112" text-anchor="middle">L</text>
    </g>
    <text x="-58" y="34" font-family="Liberation Serif" font-weight="bold" font-size="112" fill="url(#goldTextft)" text-anchor="middle">L</text>
    <text x="0" y="20" font-family="Liberation Serif" font-weight="bold" font-size="68" fill="url(#goldTextft)" text-anchor="middle">S</text>
    <text x="55" y="34" font-family="Liberation Serif" font-weight="bold" font-size="112" fill="url(#goldTextft)" text-anchor="middle">L</text>

    <!-- pillar icon -->
    <g transform="translate(0,64)">
      <g transform="translate(1.4,2)" fill="#04101c" opacity="0.5">
        <rect x="-30" y="0" width="60" height="7" rx="1.5"/>
        <rect x="-24" y="7" width="48" height="4"/>
        <rect x="-19" y="11" width="6" height="26"/>
        <rect x="-6.5" y="11" width="6" height="26"/>
        <rect x="6" y="11" width="6" height="26"/>
        <rect x="18.5" y="11" width="6" height="26"/>
        <rect x="-24" y="37" width="48" height="4"/>
        <rect x="-30" y="41" width="60" height="7" rx="1.5"/>
      </g>
      <g fill="url(#goldTextft)">
        <rect x="-30" y="0" width="60" height="7" rx="1.5"/>
        <rect x="-24" y="7" width="48" height="4"/>
        <rect x="-19" y="11" width="6" height="26"/>
        <rect x="-6.5" y="11" width="6" height="26"/>
        <rect x="6" y="11" width="6" height="26"/>
        <rect x="18.5" y="11" width="6" height="26"/>
        <rect x="-24" y="37" width="48" height="4"/>
        <rect x="-30" y="41" width="60" height="7" rx="1.5"/>
      </g>
    </g>
  </g>
</svg>

        <span style="font-weight:700;">La Solución de Leo</span>
      </a>
      <div class="lic">Sirviendo el área del Gran Sacramento, CA</div>
      <div class="disclaimer">I am not an attorney and cannot give legal advice about immigration or any other legal matter.<br>No soy abogado y no puedo dar asesoría legal sobre inmigración ni sobre ningún otro asunto legal.</div>
    </div>
    <div class="footer-links">
      <a href="#servicios">Servicios · Services</a>
      <a href="#area">Área de Servicio · Service Area</a>
      <a href="tel:+14086134713">(408) 613-4713</a>
      <a href="mailto:lasoluciondeleo@gmail.com" style="font-weight:700;">lasoluciondeleo@gmail.com</a>
    </div>
  </div>
</footer>

</body>
</html>
