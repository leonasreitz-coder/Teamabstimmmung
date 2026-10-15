```html
<!DOCTYPE html>
<html lang="de">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>AZURA | Premium Store</title>
<meta name="description" content="Azura Premium Store – FiveM Tweaks, Accounts und Community-Pakete.">
<link rel="preconnect" href="https://fonts.googleapis.com">
<link href="https://fonts.googleapis.com/css2?family=Cinzel:wght@500;600;700;800&family=Inter:wght@400;500;600;700;800&display=swap" rel="stylesheet">
<style>
:root {
  --bg:#080808;
  --panel:#111111;
  --panel2:#171411;
  --orange:#ff791f;
  --orange2:#ffad55;
  --text:#f7f3ef;
  --muted:#a39a92;
  --border:rgba(255,139,55,.19);
}
*{box-sizing:border-box;margin:0;padding:0}
html{scroll-behavior:smooth;scroll-padding-top:95px}
body{background:var(--bg);color:var(--text);font-family:Inter,Arial,sans-serif;overflow-x:hidden}
body:before{content:"";position:fixed;inset:0;pointer-events:none;z-index:-1;background:radial-gradient(ellipse at 10% 0%,#42200e66,transparent 38%),radial-gradient(ellipse at 90% 45%,#321b1050,transparent 35%),linear-gradient(180deg,#090807,#080808 70%)}
a{color:inherit;text-decoration:none}
button,input{font:inherit}
button{cursor:pointer}
#particles{position:fixed;inset:0;width:100%;height:100%;pointer-events:none;z-index:-1}
header{position:sticky;top:0;z-index:50;background:#090909e8;backdrop-filter:blur(18px);border-bottom:1px solid var(--border)}
.nav{max-width:1250px;margin:auto;padding:17px 24px;display:flex;align-items:center;justify-content:space-between;gap:20px}
.brand{font-family:Cinzel,serif;font-weight:800;font-size:27px;letter-spacing:5px;color:#fff}
.brand span{color:var(--orange)}
nav{display:flex;align-items:center;gap:22px}
nav a{font-size:12px;color:#c4bcb5;transition:.2s}
nav a:hover{color:var(--orange)}
.btn{border:1px solid var(--border);padding:12px 18px;border-radius:9px;color:#fff;background:#19130f;display:inline-flex;justify-content:center;align-items:center;gap:9px;transition:.25s;font-size:13px;font-weight:700}
.btn:hover{transform:translateY(-2px);border-color:var(--orange);box-shadow:0 8px 28px #ff791f20}
.btn.primary{background:linear-gradient(135deg,#ff8b35,#d94e12);border:0;color:#160b04}
.btn.small{padding:9px 12px;font-size:12px}
.hero{min-height:510px;display:grid;place-items:center;text-align:center;padding:90px 22px 75px;position:relative}
.eyebrow{display:inline-block;border:1px solid #ff8c3544;background:#ff791f0c;color:var(--orange2);padding:8px 14px;border-radius:50px;font-size:11px;letter-spacing:2px;text-transform:uppercase;margin-bottom:25px}
.hero h1{font-family:Cinzel,serif;font-size:clamp(48px,9vw,105px);line-height:1.05;letter-spacing:8px;text-shadow:0 0 50px #ff791f28}
.hero h1 span{color:var(--orange)}
.hero p{max-width:650px;margin:24px auto;color:#b4aaa2;line-height:1.9;font-size:15px}
.hero-actions{display:flex;justify-content:center;gap:12px;flex-wrap:wrap;margin-top:28px}
.stats{display:flex;justify-content:center;gap:50px;flex-wrap:wrap;margin-top:48px}
.stat strong{display:block;color:var(--orange2);font-size:22px}
.stat span{font-size:10px;letter-spacing:1.5px;color:var(--muted);text-transform:uppercase}
.section{max-width:1250px;margin:auto;padding:75px 24px}
.section-head{display:flex;justify-content:space-between;align-items:end;gap:20px;margin-bottom:30px;flex-wrap:wrap}
.kicker{font-size:10px;letter-spacing:3px;color:var(--orange);text-transform:uppercase;margin-bottom:10px}
h2{font-family:Cinzel,serif;font-size:clamp(27px,4vw,42px)}
.section-desc{color:var(--muted);font-size:13px;line-height:1.8;margin-top:10px;max-width:620px}
.search-row{display:flex;gap:12px;margin-bottom:20px;flex-wrap:wrap}
.search-row input{flex:1;min-width:180px;background:#101010;border:1px solid var(--border);color:white;padding:13px 15px;border-radius:9px;outline:none}
.search-row input:focus{border-color:var(--orange)}
.filters{display:flex;gap:8px;flex-wrap:wrap;margin-bottom:25px}
.filter{padding:9px 13px;background:#111;border:1px solid #29221c;border-radius:8px;color:#bdb3aa;font-size:11px}
.filter.active,.filter:hover{border-color:var(--orange);color:var(--orange2);background:#ff791f0d}
.grid{display:grid;grid-template-columns:repeat(3,minmax(0,1fr));gap:17px}
.product{background:linear-gradient(145deg,#151311,#0e0e0e 75%);border:1px solid #2b2119;border-radius:13px;padding:22px;position:relative;overflow:hidden;transition:.25s;display:flex;flex-direction:column;min-height:245px}
.product:before{content:"";position:absolute;top:0;left:18px;right:18px;height:1px;background:linear-gradient(90deg,transparent,#ff791f8a,transparent)}
.product:hover{transform:translateY(-5px);border-color:#ff791f77;box-shadow:0 16px 45px #0008}
.product-icon{width:43px;height:43px;display:grid;place-items:center;border:1px solid #ff791f42;background:#ff791f0c;border-radius:10px;font-size:21px;margin-bottom:18px}
.tag{display:inline-block;font-size:9px;letter-spacing:1px;text-transform:uppercase;color:var(--orange2);margin-bottom:9px}
.product h3{font-size:16px;margin-bottom:9px}
.product p{font-size:12px;color:#a69c94;line-height:1.7;flex:1}
.product-bottom{display:flex;justify-content:space-between;align-items:center;gap:12px;margin-top:20px}
.price{font-size:21px;font-weight:800;color:#fff}
.price small{font-size:10px;color:#aaa;font-weight:500}
.product[hidden]{display:none}
.banner{max-width:1200px;margin:20px auto 30px;padding:38px;border:1px solid var(--border);border-radius:16px;background:radial-gradient(ellipse at 100% 0%,#7a310f30,transparent 55%),#111;display:flex;justify-content:space-between;align-items:center;gap:24px;flex-wrap:wrap}
.banner p{color:var(--muted);font-size:13px;line-height:1.8;margin-top:10px;max-width:600px}
.member-grid{display:grid;grid-template-columns:repeat(4,minmax(0,1fr));gap:13px}
.member{background:#111;border:1px solid #2b2119;padding:20px;border-radius:11px;transition:.2s}
.member:hover{border-color:var(--orange)}
.member strong{font-size:21px;display:block;margin-bottom:6px}
.member span{font-size:11px;color:var(--muted)}
.member .member-price{display:block;color:var(--orange2);font-size:18px;font-weight:800;margin:16px 0}
.notice{border:1px solid #674021;background:#21160f;padding:16px;border-radius:9px;color:#e5c4a5;font-size:12px;line-height:1.8;margin-top:24px}
.steps{display:grid;grid-template-columns:repeat(3,1fr);gap:17px}
.step{padding:25px;border:1px solid var(--border);border-radius:12px;background:#101010}
.step b{color:var(--orange);font-size:12px;letter-spacing:2px}
.step h3{margin:15px 0 9px;font-size:16px}
.step p{color:var(--muted);font-size:12px;line-height:1.8}
.faq{border-top:1px solid #2a211b;padding:18px 0}
.faq h3{font-size:14px;margin-bottom:8px}
.faq p{font-size:12px;line-height:1.8;color:var(--muted)}
footer{border-top:1px solid var(--border);padding:35px 24px;text-align:center;color:#81776f;font-size:11px;line-height:2}
footer strong{font-family:Cinzel,serif;color:#eee;letter-spacing:3px}
.cart-float{position:fixed;bottom:22px;right:22px;z-index:60;box-shadow:0 8px 35px #000a}
.cart-count{display:inline-grid;place-items:center;min-width:20px;height:20px;border-radius:50%;background:#160b04;font-size:10px;padding:0 5px}
#toast{position:fixed;bottom:90px;right:22px;background:#17110d;border:1px solid var(--orange);border-radius:9px;padding:14px 18px;font-size:12px;z-index:100;opacity:0;transform:translateY(10px);transition:.25s;pointer-events:none}
#toast.show{opacity:1;transform:translateY(0)}
.cart-panel{position:fixed;right:0;top:0;height:100%;width:min(420px,100%);background:#0d0d0d;border-left:1px solid var(--border);z-index:90;padding:25px;transform:translateX(105%);transition:.3s;overflow-y:auto}
.cart-panel.open{transform:translateX(0)}
.cart-header{display:flex;justify-content:space-between;align-items:center;margin-bottom:25px}
.cart-items{display:grid;gap:12px}
.cart-item{padding:14px;border:1px solid #2b2119;border-radius:9px;display:flex;justify-content:space-between;gap:12px;font-size:12px}
.cart-item button{color:#ff8b35;background:none;border:0}
.cart-total{margin:24px 0;padding-top:20px;border-top:1px solid var(--border);display:flex;justify-content:space-between;font-weight:800}
.empty{font-size:12px;color:var(--muted);line-height:1.8}
.mobile-menu{display:none}
@keyframes rise{from{opacity:0;transform:translateY(20px)}to{opacity:1;transform:translateY(0)}}
.reveal{animation:rise .7s both}
@media(max-width:900px){.grid{grid-template-columns:repeat(2,minmax(0,1fr))}.member-grid{grid-template-columns:repeat(3,minmax(0,1fr))}nav{gap:12px}nav a{font-size:11px}}
@media(max-width:650px){.nav{padding:14px 17px}.brand{font-size:22px}nav a:not(.nav-discord){display:none}nav .btn{padding:10px;font-size:11px}.hero{min-height:470px;padding-top:70px}.hero h1{letter-spacing:4px}.stats{gap:25px}.section{padding:55px 17px}.grid{grid-template-columns:1fr}.member-grid{grid-template-columns:repeat(2,minmax(0,1fr))}.steps{grid-template-columns:1fr}.banner{margin:10px 17px;padding:25px}.product{min-height:220px}}
@media(prefers-reduced-motion:reduce){*,*:before,*:after{animation:none!important;scroll-behavior:auto!important;transition:none!important}}
</style>
</head>
<body>
<canvas id="particles"></canvas>
<header>
  <div class="nav">
    <a class="brand" href="#start">AZU<span>RA</span></a>
    <nav>
      <a href="#shop">Shop</a>
      <a href="#mitglieder">Mitglieder</a>
      <a href="#ablauf">Ablauf</a>
      <a href="#faq">FAQ</a>
      <a class="btn primary nav-discord" href="https://discord.gg/cYhUVtWQ2" target="_blank" rel="noopener">Discord ↗</a>
    </nav>
  </div>
</header>

<main>
<section class="hero" id="start">
  <div class="reveal">
    <span class="eyebrow">✦ AZURA PREMIUM STORE ✦</span>
    <h1>AZU<span>RA</span></h1>
    <p>Willkommen bei Azura. Entdecke unsere Tweaks, digitalen Produkte und Community-Pakete in einem dunklen Premium-Design. Fragen und Bestellungen laufen über unseren Discord.</p>
    <div class="hero-actions">
      <a class="btn primary" href="#shop">Shop entdecken ↓</a>
      <a class="btn" href="https://discord.gg/cYhUVtWQ2" target="_blank" rel="noopener">Discord beitreten ↗</a>
    </div>
    <div class="stats">
      <div class="stat"><strong>PREMIUM</strong><span>Unser Anspruch</span></div>
      <div class="stat"><strong>AZURA</strong><span>Unsere Community</span></div>
      <div class="stat"><strong>24/7</strong><span>Online-Shop ansehen</span></div>
    </div>
  </div>
</section>

<section class="section" id="shop">
  <div class="section-head">
    <div><div class="kicker">Der Azura Store</div><h2>Produkte entdecken</h2><p class="section-desc">Wähle ein Produkt und lege es in deinen Warenkorb. Die Bestellung wird anschließend über Discord besprochen.</p></div>
  </div>
  <div class="search-row">
    <input id="search" type="search" placeholder="Produkt suchen …" aria-label="Produkt suchen">
  </div>
  <div class="filters" id="filters">
    <button class="filter active" data-filter="alle">Alle Produkte</button>
    <button class="filter" data-filter="tweak">Tweaks</button>
    <button class="filter" data-filter="account">Accounts</button>
    <button class="filter" data-filter="premium">Premium</button>
    <button class="filter" data-filter="social">Social Media</button>
    <button class="filter" data-filter="community">Community</button>
  </div>
  <div class="grid" id="products">
    <article class="product" data-category="tweak" data-name="venix menu lifetime" data-price="0">
      <div class="product-icon">✦</div><span class="tag">Venix</span><h3>Venix Menu Lifetime</h3>
      <p>Lifetime-Angebot. Preis und Verfügbarkeit bitte direkt im Discord erfragen.</p>
      <div class="product-bottom"><span class="price">Auf Anfrage</span><a class="btn small" href="https://discord.gg/cYhUVtWQ2" target="_blank" rel="noopener">Anfragen ↗</a></div>
    </article>
    <article class="product" data-category="tweak" data-name="wasd tweak" data-price="5">
      <div class="product-icon">⌨</div><span class="tag">FiveM · Tweak</span><h3>WASD Tweak</h3>
      <p>WASD-bezogenes Tweak-Paket für dein Setup.</p>
      <div class="product-bottom"><span class="price">5,00 €</span><button class="btn small add" data-name="WASD Tweak" data-price="5">Hinzufügen +</button></div>
    </article>
    <article class="product" data-category="tweak" data-name="hitreg tweak" data-price="10">
      <div class="product-icon">◎</div><span class="tag">FiveM · Tweak</span><h3>Hitreg Tweak</h3>
      <p>Hitreg-bezogenes Tweak-Paket. Details vor dem Kauf im Discord klären.</p>
      <div class="product-bottom"><span class="price">10,00 €</span><button class="btn small add" data-name="Hitreg Tweak" data-price="10">Hinzufügen +</button></div>
    </article>
    <article class="product" data-category="tweak" data-name="full tweak" data-price="15">
      <div class="product-icon">⚙</div><span class="tag">FiveM · Komplettpaket</span><h3>Full Tweak</h3>
      <p>Das umfangreiche Tweak-Paket für dein Setup.</p>
      <div class="product-bottom"><span class="price">15,00 €</span><button class="btn small add" data-name="Full Tweak" data-price="15">Hinzufügen +</button></div>
    </article>
    <article class="product" data-category="tweak" data-name="windows tweak" data-price="10">
      <div class="product-icon">▦</div><span class="tag">Windows</span><h3>Windows Tweak</h3>
      <p>Windows-bezogenes Tweak-Paket. Leistungsversprechen hängen vom System ab.</p>
      <div class="product-bottom"><span class="price">10,00 €</span><button class="btn small add" data-name="Windows Tweak" data-price="10">Hinzufügen +</button></div>
    </article>
    <article class="product" data-category="account" data-name="steam accounts steam account" data-price="0.2">
      <div class="product-icon">◈</div><span class="tag">Steam</span><h3>Steam-Accounts</h3>
      <p>Digitale Accounts. Bestand, Inhalt und Nutzungsbedingungen vor der Bestellung prüfen.</p>
      <div class="product-bottom"><span class="price">0,20 € <small>/ Stück</small></span><button class="btn small add" data-name="Steam-Account (1 Stück)" data-price="0.2">Hinzufügen +</button></div>
    </article>
    <article class="product" data-category="account" data-name="fivem ready accounts fivem account" data-price="0.6">
      <div class="product-icon">♟</div><span class="tag">FiveM</span><h3>FiveM-ready-Accounts</h3>
      <p>Accounts für FiveM-bezogene Zwecke. Voraussetzungen und Verfügbarkeit vorab klären.</p>
      <div class="product-bottom"><span class="price">0,60 € <small>/ Stück</small></span><button class="btn small add" data-name="FiveM-ready-Account (1 Stück)" data-price="0.6">Hinzufügen +</button></div>
    </article>
    <article class="product" data-category="premium" data-name="premium pakete" data-price="0">
      <div class="product-icon">♛</div><span class="tag">Premium</span><h3>Premium-Pakete</h3>
      <p>Premium-Angebote. Die genauen Varianten und Preise müssen im Discord bestätigt werden.</p>
      <div class="product-bottom"><span class="price">Auf Anfrage</span><a class="btn small" href="https://discord.gg/cYhUVtWQ2" target="_blank" rel="noopener">Anfragen ↗</a></div>
    </article>
    <article class="product" data-category="social" data-name="tiktok follower" data-price="0">
      <div class="product-icon">♪</div><span class="tag">Social Media</span><h3>TikTok-Follower</h3>
      <p>Preise, Lieferumfang und Verfügbarkeit im Discord erfragen.</p>
      <div class="product-bottom"><span class="price">Auf Anfrage</span><a class="btn small" href="https://discord.gg/cYhUVtWQ2" target="_blank" rel="noopener">Anfragen ↗</a></div>
    </article>
    <article class="product" data-category="social" data-name="instagram follower" data-price="0">
      <div class="product-icon">◎</div><span class="tag">Social Media</span><h3>Instagram-Follower</h3>
      <p>Preise, Lieferumfang und Verfügbarkeit im Discord erfragen.</p>
      <div class="product-bottom"><span class="price">Auf Anfrage</span><a class="btn small" href="https://discord.gg/cYhUVtWQ2" target="_blank" rel="noopener">Anfragen ↗</a></div>
    </article>
    <article class="product" data-category="account" data-name="ältere accounts aged accounts" data-price="0">
      <div class="product-icon">◷</div><span class="tag">Accounts</span><h3>Ältere Accounts</h3>
      <p>Informationen zu Alter, Plattform und Verfügbarkeit bitte im Discord anfragen.</p>
      <div class="product-bottom"><span class="price">Auf Anfrage</span><a class="btn small" href="https://discord.gg/cYhUVtWQ2" target="_blank" rel="noopener">Anfragen ↗</a></div>
    </article>
  </div>
  <p id="no-results" class="empty" hidden>Keine Produkte gefunden. Ändere deine Suche oder wähle eine andere Kategorie.</p>
</section>

<section class="section" id="mitglieder">
  <div class="section-head">
    <div><div class="kicker">Community-Pakete</div><h2>Aktive Discord-Mitglieder</h2><p class="section-desc">Die angegebenen Paketpreise werden hier transparent angezeigt. Details zur Umsetzung und Verfügbarkeit bitte vorher im Discord klären.</p></div>
  </div>
  <div class="member-grid" id="member-grid"></div>
  <div class="notice">Hinweis: Die Pakete sind Angebotsangaben, keine Garantie für tatsächliche Aktivität oder dauerhaften Verbleib von Mitgliedern. Bitte kläre alle Bedingungen vor einer Bestellung.</div>
</section>

<section class="section" id="ablauf">
  <div class="section-head"><div><div class="kicker">Einfach und direkt</div><h2>So funktioniert es</h2></div></div>
  <div class="steps">
    <div class="step"><b>01 / AUSWÄHLEN</b><h3>Produkt aussuchen</h3><p>Sieh dir die Angebote an und lege Produkte mit festem Preis in den Warenkorb.</p></div>
    <div class="step"><b>02 / DISCORD</b><h3>Details klären</h3><p>Öffne unseren Discord und kläre Bestand, Lieferumfang, Bedingungen und Bezahlung.</p></div>
    <div class="step"><b>03 / ABSCHLIESSEN</b><h3>Bestellung abstimmen</h3><p>Bestätige die Bestellung erst, wenn dir alle Angaben und Bedingungen bekannt sind.</p></div>
  </div>
</section>

<section class="section" id="faq">
  <div class="section-head"><div><div class="kicker">Häufige Fragen</div><h2>FAQ</h2></div></div>
  <div class="faq"><h3>Wie bestelle ich?</h3><p>Nutze den Warenkorb als Merkliste und sende die Zusammenfassung über den Button an Discord. Die Website nimmt selbst keine Zahlung entgegen.</p></div>
  <div class="faq"><h3>Sind alle Preise fest?</h3><p>Nur die Angebote mit sichtbarem Euro-Preis haben einen eingetragenen Preis. Bei „Auf Anfrage“ ist der Preis noch nicht hinterlegt.</p></div>
  <div class="faq"><h3>Kann ich direkt bezahlen?</h3><p>Nein. Diese Version hat kein Zahlungssystem und keinen Server zur Bestellverarbeitung. Die Details müssen im Discord geklärt werden.</p></div>
  <div class="faq"><h3>Wo bekomme ich Support?</h3><p>Über den offiziellen Azura-Discord.</p></div>
</section>

<section class="banner">
  <div><div class="kicker">Tritt der Community bei</div><h2>Bereit für AZURA?</h2><p>Fragen zu Angeboten, Verfügbarkeit und Bestellungen? Besuche unseren Discord und sprich mit dem Team.</p></div>
  <a class="btn primary" href="https://discord.gg/cYhUVtWQ2" target="_blank" rel="noopener">Discord öffnen ↗</a>
</section>
</main>

<footer>
  <strong>AZURA</strong><br>
  Premium Store · Community · Support<br>
  Diese Website ist eine Shop-Vorlage. Produktverfügbarkeit, Rechte und Preise müssen vor Veröffentlichung geprüft werden.<br>
  © <span id="year"></span> AZURA
</footer>

<button class="btn primary cart-float" id="open-cart">🛒 Warenkorb <span class="cart-count" id="cart-count">0</span></button>
<aside class="cart-panel" id="cart-panel" aria-label="Warenkorb">
  <div class="cart-header"><h2>Warenkorb</h2><button class="btn small" id="close-cart" aria-label="Warenkorb schließen">✕</button></div>
  <div class="cart-items" id="cart-items"><p class="empty">Dein Warenkorb ist noch leer.</p></div>
  <div class="cart-total"><span>Gesamt</span><span id="cart-total">0,00 €</span></div>
  <p class="empty">Der Warenkorb ist eine Merkliste. Die Bestellung wird nicht automatisch bezahlt oder übermittelt.</p>
  <button class="btn primary" id="send-order" style="width:100%;margin-top:18px">Bestellung für Discord vorbereiten ↗</button>
  <button class="btn" id="clear-cart" style="width:100%;margin-top:10px">Warenkorb leeren</button>
</aside>
<div id="toast" role="status"></div>

<script>
const DISCORD = "https://discord.gg/cYhUVtWQ2";
const memberPackages = [
  [500,4.99],[1000,12.99],[2000,20],[3000,27.99],
  [4000,34.99],[5000,39.99],[6000,45.99],[7000,50.99],
  [8000,55.99],[9000,60.99],[10000,65.99],[11000,70.99]
];
const euro = n => n.toLocaleString("de-DE",{style:"currency",currency:"EUR"});
const memberGrid = document.getElementById("member-grid");
memberPackages.forEach(([count,price])=>{
  const card=document.createElement("article");
  card.className="member";
  card.innerHTML=`<strong>${count.toLocaleString("de-DE")}</strong><span>Mitglieder-Paket</span><span class="member-price">${euro(price)}</span><button class="btn small" style="width:100%">Paket anfragen ↗</button>`;
  card.querySelector("button").addEventListener("click",()=>{
    const msg=`Hallo Azura-Team, ich möchte das Paket mit ${count.toLocaleString("de-DE")} Mitgliedern für ${euro(price)} anfragen.`;
    window.open(DISCORD,"_blank","noopener");
    showToast("Discord geöffnet. Füge dort deine Paket-Anfrage ein.");
    try{navigator.clipboard.writeText(msg)}catch(e){}
  });
  memberGrid.appendChild(card);
});

let cart=[];
const cartPanel=document.getElementById("cart-panel");
const toast=document.getElementById("toast");
let toastTimer;
function showToast(msg){
  toast.textContent=msg;toast.classList.add("show");
  clearTimeout(toastTimer);toastTimer=setTimeout(()=>toast.classList.remove("show"),2600);
}
function renderCart(){
  document.getElementById("cart-count").textContent=cart.length;
  const root=document.getElementById("cart-items");
  root.innerHTML="";
  if(!cart.length){root.innerHTML='<p class="empty">Dein Warenkorb ist noch leer.</p>';}
  cart.forEach((item,index)=>{
    const row=document.createElement("div");row.className="cart-item";
    const label=document.createElement("span");label.textContent=item.name;
    const right=document.createElement("div");
    const price=document.createElement("strong");price.textContent=euro(item.price)+" ";
    const remove=document.createElement("button");remove.textContent="Entfernen";remove.addEventListener("click",()=>{cart.splice(index,1);renderCart()});
    right.append(price,remove);row.append(label,right);root.appendChild(row);
  });
  document.getElementById("cart-total").textContent=euro(cart.reduce((sum,item)=>sum+item.price,0));
}
document.querySelectorAll(".add").forEach(btn=>btn.addEventListener("click",()=>{
  cart.push({name:btn.dataset.name,price:Number(btn.dataset.price)});
  renderCart();showToast("Zum Warenkorb hinzugefügt ✓");
}));
document.getElementById("open-cart").addEventListener("click",()=>cartPanel.classList.add("open"));
document.getElementById("close-cart").addEventListener("click",()=>cartPanel.classList.remove("open"));
document.getElementById("clear-cart").addEventListener("click",()=>{cart=[];renderCart();showToast("Warenkorb geleert")});
document.getElementById("send-order").addEventListener("click",()=>{
  if(!cart.length){showToast("Dein Warenkorb ist noch leer.");return}
  const items=cart.map(i=>`- ${i.name}: ${euro(i.price)}`).join("\n");
  const total=euro(cart.reduce((s,i)=>s+i.price,0));
  const msg=`Hallo Azura-Team! Ich möchte folgende Produkte anfragen:\n${items}\nGesamt: ${total}\nBitte bestätigt mir Verfügbarkeit und Bestellbedingungen.`;
  try{navigator.clipboard.writeText(msg)}catch(e){}
  window.open(DISCORD,"_blank","noopener");
  showToast("Zusammenfassung vorbereitet. Bei Bedarf manuell kopieren.");
});
document.getElementById("filters").addEventListener("click",e=>{
  const btn=e.target.closest("[data-filter]");if(!btn)return;
  document.querySelectorAll(".filter").forEach(b=>b.classList.toggle("active",b===btn));
  filterProducts(btn.dataset.filter,document.getElementById("search").value);
});
document.getElementById("search").addEventListener("input",e=>{
  const active=document.querySelector(".filter.active");
  filterProducts(active?active.dataset.filter:"alle",e.target.value);
});
function filterProducts(category,query){
  let shown=0;
  document.querySelectorAll(".product").forEach(card=>{
    const matchesCategory=category==="alle"||card.dataset.category===category;
    const matchesText=(card.dataset.name+" "+card.textContent).toLowerCase().includes(query.toLowerCase());
    card.hidden=!(matchesCategory&&matchesText);if(!card.hidden)shown++;
  });
  document.getElementById("no-results").hidden=shown!==0;
}
document.getElementById("year").textContent=new Date().getFullYear();

// Animierter Halloween-Partikelhintergrund
const canvas=document.getElementById("particles"),ctx=canvas.getContext("2d");
let particles=[];
function resize(){
  const dpr=Math.min(window.devicePixelRatio||1,2);
  canvas.width=innerWidth*dpr;canvas.height=innerHeight*dpr;
  canvas.style.width=innerWidth+"px";canvas.style.height=innerHeight+"px";
  ctx.setTransform(dpr,0,0,dpr,0,0);
  particles=Array.from({length:Math.min(75,Math.floor(innerWidth/17))},()=>({
    x:Math.random()*innerWidth,y:Math.random()*innerHeight,
    r:Math.random()*2+0.5,v:Math.random()*.35+.08,
    a:Math.random()*.55+.12,drift:(Math.random()-.5)*.35
  }));
}
function animate(){
  ctx.clearRect(0,0,innerWidth,innerHeight);
  for(const p of particles){
    p.y-=p.v;p.x+=p.drift;
    if(p.y<-5){p.y=innerHeight+5;p.x=Math.random()*innerWidth}
    if(p.x<-5)p.x=innerWidth+5;if(p.x>innerWidth+5)p.x=-5;
    ctx.beginPath();ctx.arc(p.x,p.y,p.r,0,Math.PI*2);
    ctx.fillStyle=`rgba(255, ${105+Math.floor(p.r*20)}, 35, ${p.a})`;ctx.fill();
  }
  requestAnimationFrame(animate);
}
resize();animate();window.addEventListener("resize",resize);
</script>
</body>
</html>
```
