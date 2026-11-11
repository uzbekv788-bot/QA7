[greendent_dental.html](https://github.com/user-attachments/files/34688497/greendent_dental.html)
<!DOCTYPE html>
<html lang="ru">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0, viewport-fit=cover">
<meta name="theme-color" content="#f7fff9">
<title>GreenDent — современная стоматология</title>
<style>
:root{
  --bg:#f7fff9; --surface:#ffffff; --surface-2:#effaf1; --text:#102018;
  --muted:#5d7064; --line:#cfe3d3; --green:#147a43; --green-2:#1e9a58;
  --yellow:#f4c542; --yellow-2:#fff2bd; --blue:#2868d7; --danger:#b52c35;
  --nav:#ffffff; --focus:#135ee8; --radius:24px;
}
[data-theme="dark"]{
  --bg:#071015; --surface:#0d171d; --surface-2:#10242b; --text:#f1fbf5;
  --muted:#a9bbb4; --line:#254149; --green:#37c77a; --green-2:#2aa968;
  --yellow:#f2c94c; --yellow-2:#3b3218; --blue:#55a1ff; --danger:#ff6b73;
  --nav:#0d171d; --focus:#79b7ff;
}
*{box-sizing:border-box}
html{scroll-behavior:smooth}
body{margin:0;background:var(--bg);color:var(--text);font-family:Inter,ui-sans-serif,system-ui,-apple-system,BlinkMacSystemFont,"Segoe UI",sans-serif;line-height:1.5;padding-bottom:96px}
button,input,select{font:inherit}
button,a{ -webkit-tap-highlight-color:transparent}
a{color:inherit;text-decoration:none}
:focus-visible{outline:3px solid var(--focus);outline-offset:3px}
.container{width:min(1180px,calc(100% - 36px));margin:auto}
.topline{background:var(--green);color:#fff;font-size:13px;font-weight:700;padding:9px 0}
.topline .container{display:flex;justify-content:space-between;gap:15px}
.header{position:sticky;top:0;z-index:20;background:var(--bg);border-bottom:1px solid var(--line)}
.header-inner{min-height:72px;display:flex;align-items:center;justify-content:space-between;gap:20px}
.brand{display:flex;align-items:center;gap:11px;font-weight:900;letter-spacing:-.03em;font-size:21px}
.logo{width:40px;height:40px;border-radius:12px;background:var(--green);display:grid;place-items:center;color:#fff;font-size:21px}
.desktop-nav{display:flex;gap:8px;align-items:center}
.desktop-nav a{padding:10px 14px;border-radius:12px;color:var(--muted);font-weight:700}
.desktop-nav a:hover{background:var(--surface-2);color:var(--text)}
.actions{display:flex;gap:8px;align-items:center}
.icon-btn,.theme-btn{border:1px solid var(--line);background:var(--surface);color:var(--text);height:42px;min-width:42px;border-radius:12px;cursor:pointer}
.icon-btn:hover,.theme-btn:hover{background:var(--surface-2)}
.primary{border:1px solid var(--green);background:var(--green);color:#fff;border-radius:13px;padding:12px 18px;font-weight:800;cursor:pointer}
.primary:hover{background:var(--green-2)}
.secondary{border:1px solid var(--green);background:transparent;color:var(--green);border-radius:13px;padding:11px 17px;font-weight:800;cursor:pointer}
.secondary:hover{background:var(--surface-2)}
.hero{padding:46px 0 30px}
.hero-grid{display:grid;grid-template-columns:1.15fr .85fr;gap:24px;align-items:stretch}
.hero-copy{background:var(--green);color:#fff;border-radius:28px;padding:42px;position:relative;overflow:hidden}
.hero-copy:after{content:"+";position:absolute;right:25px;top:8px;font-size:160px;line-height:1;font-weight:900;color:#fff;opacity:.10}
.eyebrow{font-size:12px;text-transform:uppercase;letter-spacing:.14em;font-weight:900}
h1{font-size:clamp(36px,6vw,68px);line-height:.98;letter-spacing:-.055em;margin:14px 0 18px;max-width:720px}
.hero-copy p{font-size:18px;max-width:610px;color:#effff4}
.hero-actions{display:flex;gap:10px;flex-wrap:wrap;margin-top:25px}
.hero .secondary{border-color:#fff;color:#fff;background:transparent}
.hero .secondary:hover{background:rgba(255,255,255,.12)}
.hero-art{border-radius:28px;background:var(--yellow);min-height:390px;display:grid;place-items:center;overflow:hidden}
.hero-art svg{width:86%;height:86%;max-width:470px}
.stats{display:grid;grid-template-columns:repeat(4,1fr);gap:10px;margin-top:18px}
.stat{background:var(--surface);border:1px solid var(--line);padding:17px;border-radius:18px}
.stat strong{display:block;font-size:24px}
.stat span{color:var(--muted);font-size:13px}
section{padding:54px 0}
.section-head{display:flex;justify-content:space-between;align-items:end;gap:20px;margin-bottom:22px}
.section-head h2{font-size:34px;letter-spacing:-.04em;margin:0}
.section-head p{margin:7px 0 0;color:var(--muted);max-width:620px}
.chips{display:flex;gap:8px;flex-wrap:wrap}
.chip{border:1px solid var(--line);background:var(--surface);padding:8px 12px;border-radius:999px;font-size:13px;font-weight:800;color:var(--muted)}
.chip.active{background:var(--yellow);border-color:var(--yellow);color:#302708}
.services{display:grid;grid-template-columns:repeat(3,1fr);gap:15px}
.card{background:var(--surface);border:1px solid var(--line);border-radius:22px;overflow:hidden}
.card:hover{border-color:var(--green)}
.card-art{height:190px;background:var(--surface-2);display:grid;place-items:center;border-bottom:1px solid var(--line)}
.card-art svg{width:80%;height:80%}
.card-body{padding:18px}
.card-body h3{margin:0 0 6px;font-size:20px}
.card-body p{color:var(--muted);margin:0 0 15px;font-size:14px}
.meta{display:flex;justify-content:space-between;gap:12px;align-items:center}
.price{font-size:19px;font-weight:900;color:var(--green)}
.small{font-size:12px;color:var(--muted)}
.products{display:grid;grid-template-columns:repeat(4,1fr);gap:13px}
.product{padding:17px;background:var(--surface);border:1px solid var(--line);border-radius:20px}
.product-icon{width:54px;height:54px;border-radius:15px;background:var(--yellow-2);display:grid;place-items:center;color:#6d5712;font-size:25px;margin-bottom:13px}
.product h3{margin:0;font-size:17px}.product p{color:var(--muted);font-size:13px;margin:5px 0 12px}
.help{display:grid;grid-template-columns:1fr 1fr;gap:15px}
.help-card{background:var(--surface);border:1px solid var(--line);border-radius:22px;padding:24px}
.help-card h3{margin-top:0}
.faq{border-top:1px solid var(--line)}
.faq button{width:100%;border:0;border-bottom:1px solid var(--line);background:transparent;color:var(--text);text-align:left;padding:16px 0;cursor:pointer;font-weight:800;display:flex;justify-content:space-between}
.answer{display:none;color:var(--muted);padding:0 0 15px}
.faq.open .answer{display:block}
.booking{background:var(--blue);color:#fff;border-radius:28px;padding:30px;display:grid;grid-template-columns:1fr 1fr;gap:25px}
.booking p{color:#e8f2ff}
.form{background:var(--surface);color:var(--text);padding:22px;border-radius:22px;border:1px solid var(--line)}
.field{margin-bottom:14px}.field label{display:block;font-size:13px;font-weight:800;margin-bottom:6px}
.field input,.field select{width:100%;padding:12px 13px;border:1px solid var(--line);border-radius:12px;background:var(--surface);color:var(--text)}
.time-row{display:grid;grid-template-columns:1fr 1fr 1fr;gap:7px}
.form-note{font-size:12px;color:var(--muted);margin-top:10px}
footer{padding:36px 0 24px;border-top:1px solid var(--line);color:var(--muted)}
.footer-grid{display:grid;grid-template-columns:2fr 1fr 1fr;gap:25px}
.mobile-nav{display:none}
.toast{position:fixed;left:50%;bottom:105px;transform:translateX(-50%) translateY(20px);background:var(--text);color:var(--bg);padding:12px 17px;border-radius:14px;font-weight:800;opacity:0;pointer-events:none;transition:.2s;z-index:50}
.toast.show{opacity:1;transform:translateX(-50%) translateY(0)}
.modal{display:none;position:fixed;inset:0;background:rgba(0,0,0,.45);z-index:60;padding:20px;place-items:center}
.modal.show{display:grid}
.modal-box{width:min(560px,100%);background:var(--surface);color:var(--text);border:1px solid var(--line);border-radius:25px;padding:25px}
.modal-head{display:flex;justify-content:space-between;gap:10px;align-items:start}
.modal-head h2{margin:0}
.close{border:1px solid var(--line);background:var(--surface);color:var(--text);width:40px;height:40px;border-radius:12px;cursor:pointer}
@media(max-width:900px){
 .desktop-nav{display:none}.hero-grid{grid-template-columns:1fr}.hero-art{min-height:300px}
 .services{grid-template-columns:1fr 1fr}.products{grid-template-columns:1fr 1fr}.booking{grid-template-columns:1fr}.help{grid-template-columns:1fr}
 .stats{grid-template-columns:1fr 1fr}
}
@media(max-width:650px){
 body{padding-bottom:92px}
 .container{width:min(100% - 24px,1180px)}
 .topline .container{justify-content:center}.topline span:last-child{display:none}
 .header-inner{min-height:62px}.actions .primary{display:none}
 .hero{padding-top:20px}.hero-copy{padding:27px;border-radius:22px}
 h1{font-size:42px}.hero-art{border-radius:22px;min-height:260px}
 .stats{grid-template-columns:1fr 1fr}.stat{padding:14px}
 section{padding:38px 0}.section-head{display:block}.section-head h2{font-size:29px}
 .services{grid-template-columns:1fr}.products{grid-template-columns:1fr 1fr}
 .booking{padding:20px;border-radius:22px}
 .footer-grid{grid-template-columns:1fr}
 .mobile-nav{position:fixed;display:grid;grid-template-columns:repeat(4,1fr);left:0;right:0;bottom:0;z-index:40;background:var(--nav);border-top:1px solid var(--line);padding:8px 8px calc(8px + env(safe-area-inset-bottom));}
 .mobile-nav a{display:flex;flex-direction:column;align-items:center;justify-content:center;gap:3px;min-height:58px;color:var(--muted);font-size:11px;font-weight:800;position:relative}
 .mobile-nav a.active{color:var(--green)}
 .nav-icon{font-size:20px;line-height:1}
 .badge{position:absolute;top:1px;margin-left:24px;background:var(--danger);color:#fff;border-radius:999px;min-width:17px;height:17px;padding:0 5px;display:grid;place-items:center;font-size:10px}
}
@media(prefers-reduced-motion:reduce){html{scroll-behavior:auto}.toast{transition:none}}
</style>
</head>
<body>
<div class="topline"><div class="container"><span>● Приём сегодня до 21:00</span><span>Ташкент · Безболезненная стоматология</span></div></div>

<header class="header">
  <div class="container header-inner">
    <a class="brand" href="#home" aria-label="GreenDent">
      <span class="logo">✦</span><span>GreenDent</span>
    </a>
    <nav class="desktop-nav" aria-label="Основная навигация">
      <a href="#services">Услуги</a><a href="#products">Продукция</a><a href="#help">Помощь</a><a href="#booking">Запись</a>
    </nav>
    <div class="actions">
      <button class="theme-btn" id="themeBtn" aria-label="Переключить тему">☾</button>
      <button class="primary" data-booking>Записаться</button>
    </div>
  </div>
</header>

<main id="home">
<section class="hero">
<div class="container">
<div class="hero-grid">
  <div class="hero-copy">
    <div class="eyebrow">Стоматология нового поколения</div>
    <h1>Здоровая улыбка без лишнего стресса.</h1>
    <p>GreenDent объединяет профилактику, лечение и эстетику в одном спокойном пространстве. Понятные цены, внимательные врачи и современный подход.</p>
    <div class="hero-actions">
      <button class="primary" data-booking>Записаться на приём</button>
      <a class="secondary" href="#services">Посмотреть услуги</a>
    </div>
  </div>
  <div class="hero-art" aria-label="Иллюстрация улыбки">
    <svg viewBox="0 0 520 420" role="img">
      <rect x="36" y="42" width="448" height="336" rx="38" fill="#fff"/>
      <circle cx="410" cy="92" r="35" fill="#147a43"/>
      <path d="M130 160c35-48 72-71 130-71s95 23 130 71c-19 97-69 151-130 151S149 257 130 160Z" fill="#f4c542"/>
      <path d="M163 173c25-31 55-45 97-45s72 14 97 45c-13 63-48 100-97 100s-84-37-97-100Z" fill="#fff"/>
      <path d="M190 198c18 27 42 40 70 40s52-13 70-40" fill="none" stroke="#147a43" stroke-width="12" stroke-linecap="round"/>
      <circle cx="222" cy="170" r="8" fill="#102018"/><circle cx="298" cy="170" r="8" fill="#102018"/>
      <rect x="68" y="315" width="140" height="24" rx="12" fill="#147a43"/>
      <rect x="222" y="315" width="92" height="24" rx="12" fill="#f4c542"/>
    </svg>
  </div>
</div>
<div class="stats">
  <div class="stat"><strong>4.9/5</strong><span>средняя оценка</span></div>
  <div class="stat"><strong>12 000+</strong><span>довольных пациентов</span></div>
  <div class="stat"><strong>15 лет</strong><span>опыта команды</span></div>
  <div class="stat"><strong>21:00</strong><span>приём до позднего вечера</span></div>
</div>
</div>
</section>

<section id="services">
<div class="container">
<div class="section-head">
<div><div class="eyebrow" style="color:var(--green)">Услуги</div><h2>Всё для улыбки</h2><p>Выбирайте направление — от профилактики до эстетической реставрации.</p></div>
<div class="chips"><span class="chip active">Все</span><span class="chip">Лечение</span><span class="chip">Эстетика</span></div>
</div>
<div class="services">
<article class="card">
<div class="card-art"><svg viewBox="0 0 320 180"><rect width="320" height="180" fill="#effaf1"/><circle cx="160" cy="90" r="67" fill="#fff"/><path d="M118 72c13-18 26-27 42-27s29 9 42 27c-6 48-20 76-42 76s-36-28-42-76Z" fill="#f4c542"/><path d="M137 83h46v37h-46z" fill="#fff"/><path d="M145 101h30" stroke="#147a43" stroke-width="8" stroke-linecap="round"/></svg></div>
<div class="card-body"><h3>Профессиональная чистка</h3><p>Удаление налёта и бережная полировка для ощущения свежести.</p><div class="meta"><span class="price">от 250 000 сум</span><span class="small">45–60 мин</span></div></div>
</article>

<article class="card">
<div class="card-art"><svg viewBox="0 0 320 180"><rect width="320" height="180" fill="#effaf1"/><rect x="78" y="55" width="164" height="72" rx="36" fill="#fff"/><circle cx="130" cy="91" r="18" fill="#f4c542"/><circle cx="190" cy="91" r="18" fill="#f4c542"/><path d="M110 124c30 20 70 20 100 0" fill="none" stroke="#147a43" stroke-width="10" stroke-linecap="round"/></svg></div>
<div class="card-body"><h3>Лечение кариеса</h3><p>Диагностика, аккуратное лечение и восстановление формы зуба.</p><div class="meta"><span class="price">от 420 000 сум</span><span class="small">60–90 мин</span></div></div>
</article>

<article class="card">
<div class="card-art"><svg viewBox="0 0 320 180"><rect width="320" height="180" fill="#effaf1"/><path d="M90 119c0-53 30-80 70-80s70 27 70 80" fill="#fff" stroke="#147a43" stroke-width="12"/><path d="M112 92h96M126 67h68" stroke="#f4c542" stroke-width="12" stroke-linecap="round"/></svg></div>
<div class="card-body"><h3>Отбеливание</h3><p>Эстетическая процедура с подбором оттенка и консультацией врача.</p><div class="meta"><span class="price">от 1 100 000 сум</span><span class="small">60 мин</span></div></div>
</article>

<article class="card">
<div class="card-art"><svg viewBox="0 0 320 180"><rect width="320" height="180" fill="#effaf1"/><circle cx="160" cy="90" r="70" fill="#fff"/><path d="M122 61h76v58h-76z" fill="#f4c542"/><path d="M134 75h52v30h-52z" fill="#fff"/><path d="M160 42v16M160 122v16M112 90H96M224 90h-16" stroke="#147a43" stroke-width="9" stroke-linecap="round"/></svg></div>
<div class="card-body"><h3>Имплантация</h3><p>Планирование восстановления зуба с использованием цифровой диагностики.</p><div class="meta"><span class="price">от 4 800 000 сум</span><span class="small">по плану врача</span></div></div>
</article>

<article class="card">
<div class="card-art"><svg viewBox="0 0 320 180"><rect width="320" height="180" fill="#effaf1"/><path d="M91 64h138v52H91z" fill="#fff" stroke="#147a43" stroke-width="10"/><path d="M105 78h24v24h-24zm43 0h24v24h-24zm43 0h24v24h-24z" fill="#f4c542"/></svg></div>
<div class="card-body"><h3>Виниры</h3><p>Точная эстетическая коррекция формы и оттенка после консультации.</p><div class="meta"><span class="price">от 2 900 000 сум</span><span class="small">за единицу</span></div></div>
</article>

<article class="card">
<div class="card-art"><svg viewBox="0 0 320 180"><rect width="320" height="180" fill="#effaf1"/><path d="M104 56h112v68H104z" fill="#fff"/><path d="M122 74h76v32h-76z" fill="#f4c542"/><path d="M134 137h52" stroke="#147a43" stroke-width="10" stroke-linecap="round"/></svg></div>
<div class="card-body"><h3>Детская стоматология</h3><p>Спокойный первый контакт, профилактика и лечение в дружелюбной атмосфере.</p><div class="meta"><span class="price">от 180 000 сум</span><span class="small">30–60 мин</span></div></div>
</article>
</div>
</div>
</section>

<section id="products">
<div class="container">
<div class="section-head"><div><div class="eyebrow" style="color:var(--green)">Продукция</div><h2>Домашняя забота</h2><p>Подобранные средства, которые помогают поддерживать результат между визитами.</p></div></div>
<div class="products">
<div class="product"><div class="product-icon">✦</div><h3>Щётки Soft</h3><p>Мягкие щетинки для ежедневного ухода.</p><strong>от 45 000 сум</strong></div>
<div class="product"><div class="product-icon">◒</div><h3>Флосс</h3><p>Нежная нить для межзубных промежутков.</p><strong>от 35 000 сум</strong></div>
<div class="product"><div class="product-icon">＋</div><h3>Паста Care+</h3><p>Фторсодержащая паста для регулярной защиты.</p><strong>от 65 000 сум</strong></div>
<div class="product"><div class="product-icon">◉</div><h3>Ирригатор</h3><p>Удобный домашний уход для труднодоступных зон.</p><strong>от 690 000 сум</strong></div>
</div>
</div>
</section>

<section id="help">
<div class="container">
<div class="section-head"><div><div class="eyebrow" style="color:var(--green)">Помощь</div><h2>Частые вопросы</h2><p>Короткие ответы перед визитом.</p></div></div>
<div class="help">
<div class="help-card">
<h3>Перед приёмом</h3>
<div class="faq open"><button>Нужно ли приходить натощак? <span>+</span></button><div class="answer">Обычно нет. Для стандартного стоматологического приёма можно есть как обычно, если врач не дал иных инструкций.</div></div>
<div class="faq"><button>Сколько длится консультация? <span>+</span></button><div class="answer">В среднем 30–45 минут, включая осмотр и обсуждение плана лечения.</div></div>
<div class="faq"><button>Можно ли выбрать время онлайн? <span>+</span></button><div class="answer">Да. Выберите дату и время в форме записи — после отправки заявки администратор подтвердит визит.</div></div>
</div>
<div class="help-card">
<h3>Связаться с клиникой</h3>
<p style="color:var(--muted)">Если вопрос срочный, позвоните в клинику. Для обычных вопросов оставьте заявку.</p>
<p><strong>+998 71 200 20 20</strong><br><span style="color:var(--muted)">Пн–Сб · 08:00–21:00</span></p>
<button class="secondary" data-booking>Оставить заявку</button>
</div>
</div>
</div>
</section>

<section id="booking">
<div class="container">
<div class="booking">
<div>
<div class="eyebrow">Запись</div>
<h2 style="font-size:35px;letter-spacing:-.04em;margin:8px 0">Выберите удобное время</h2>
<p>Время хранится в формате 24 часа (HH:mm), а в интерфейсе показывается в привычном 12-часовом формате.</p>
<ul style="padding-left:19px;line-height:2;color:#e8f2ff">
<li>Подтверждение администратором</li><li>Без скрытых доплат</li><li>Напоминание о визите</li>
</ul>
</div>
<form class="form" id="bookingForm">
<div class="field"><label for="name">Имя</label><input id="name" required placeholder="Ваше имя"></div>
<div class="field"><label for="service">Услуга</label><select id="service"><option>Консультация</option><option>Профессиональная чистка</option><option>Лечение кариеса</option><option>Отбеливание</option><option>Имплантация</option></select></div>
<div class="field"><label for="date">Дата</label><input id="date" type="date" required></div>
<div class="field"><label>Время</label>
<div class="time-row">
<select id="hour" aria-label="Часы"></select>
<select id="minute" aria-label="Минуты"></select>
<select id="ampm" aria-label="AM или PM"><option>AM</option><option>PM</option></select>
</div></div>
<button class="primary" style="width:100%;margin-top:5px" type="submit">Подтвердить запись</button>
<div class="form-note">После отправки заявки время будет сохранено как HH:mm.</div>
</form>
</div>
</div>
</section>
</main>

<footer><div class="container footer-grid"><div><div class="brand"><span class="logo">✦</span><span>GreenDent</span></div><p>Современная стоматология с человеческим отношением.</p></div><div><strong>Клиника</strong><p>Услуги<br>Продукция<br>Помощь</p></div><div><strong>Контакты</strong><p>Ташкент<br>+998 71 200 20 20<br>08:00–21:00</p></div></div></footer>

<nav class="mobile-nav" aria-label="Нижняя навигация">
<a href="#home" class="active" aria-current="page"><span class="nav-icon">⌂</span><span>Главная</span></a>
<a href="#services"><span class="nav-icon">✚</span><span>Услуги</span></a>
<a href="#products"><span class="nav-icon">◈</span><span>Продукция</span></a>
<a href="#help"><span class="nav-icon">▢</span><span>Inbox</span><span class="badge">3</span></a>
</nav>

<div class="toast" id="toast"></div>

<div class="modal" id="modal" aria-hidden="true">
<div class="modal-box" role="dialog" aria-modal="true" aria-labelledby="modalTitle">
<div class="modal-head"><div><div class="eyebrow" style="color:var(--green)">Быстрая запись</div><h2 id="modalTitle">Выберите время</h2></div><button class="close" id="closeModal" aria-label="Закрыть">×</button></div>
<p style="color:var(--muted)">Заполните форму ниже — заявка отправится администратору.</p>
<form id="quickForm">
<div class="field"><label>Имя</label><input required placeholder="Ваше имя"></div>
<div class="field"><label>Дата</label><input type="date" required></div>
<div class="field"><label>Время</label><div class="time-row"><select class="m-hour"></select><select class="m-minute"></select><select class="m-ampm"><option>AM</option><option>PM</option></select></div></div>
<button class="primary" style="width:100%">Записаться</button>
</form>
</div></div>

<script>
const root=document.documentElement;
const themeBtn=document.getElementById('themeBtn');
const saved=localStorage.getItem('greendent-theme');
if(saved) root.dataset.theme=saved;
function syncTheme(){themeBtn.textContent=root.dataset.theme==='dark'?'☀':'☾';}
syncTheme();
themeBtn.addEventListener('click',()=>{
  root.dataset.theme=root.dataset.theme==='dark'?'light':'dark';
  localStorage.setItem('greendent-theme',root.dataset.theme);
  syncTheme();
});

function fillTime(selectH,selectM,selectAP){
  for(let h=1;h<=12;h++) selectH.add(new Option(String(h).padStart(2,'0'),h));
  for(let m=0;m<60;m+=5) selectM.add(new Option(String(m).padStart(2,'0'),m));
  selectH.value=10; selectM.value=30; selectAP.value='AM';
}
fillTime(document.getElementById('hour'),document.getElementById('minute'),document.getElementById('ampm'));
fillTime(document.querySelector('.m-hour'),document.querySelector('.m-minute'),document.querySelector('.m-ampm'));

function to24(h,m,ap){let hh=Number(h)%12;if(ap==='PM')hh+=12;return String(hh).padStart(2,'0')+':'+String(m).padStart(2,'0')}
const toast=document.getElementById('toast');
function showToast(msg){toast.textContent=msg;toast.classList.add('show');setTimeout(()=>toast.classList.remove('show'),3200)}

document.querySelectorAll('.faq button').forEach(btn=>btn.addEventListener('click',()=>btn.parentElement.classList.toggle('open')));

const modal=document.getElementById('modal');
document.querySelectorAll('[data-booking]').forEach(b=>b.addEventListener('click',()=>{modal.classList.add('show');modal.setAttribute('aria-hidden','false')}));
document.getElementById('closeModal').addEventListener('click',()=>{modal.classList.remove('show');modal.setAttribute('aria-hidden','true')});
modal.addEventListener('click',e=>{if(e.target===modal)modal.classList.remove('show')});

document.getElementById('bookingForm').addEventListener('submit',e=>{
 e.preventDefault();
 const time=to24(hour.value,minute.value,ampm.value);
 showToast('Заявка принята. Вы выбрали '+time+' — администратор свяжется с вами.');
});
document.getElementById('quickForm').addEventListener('submit',e=>{
 e.preventDefault();
 const h=e.currentTarget.querySelector('.m-hour').value,m=e.currentTarget.querySelector('.m-minute').value,ap=e.currentTarget.querySelector('.m-ampm').value;
 showToast('Заявка принята. Время: '+to24(h,m,ap));
 modal.classList.remove('show');
});

const sections=[...document.querySelectorAll('main section')];
const navLinks=[...document.querySelectorAll('.mobile-nav a')];
const observer=new IntersectionObserver(entries=>{
 entries.forEach(entry=>{
   if(entry.isIntersecting){
     const id=entry.target.id;
     navLinks.forEach(a=>{
       const active=a.getAttribute('href')==='#'+id;
       a.classList.toggle('active',active);
       if(active)a.setAttribute('aria-current','page');else a.removeAttribute('aria-current');
     });
   }
 });
},{rootMargin:'-35% 0px -50% 0px',threshold:0});
sections.forEach(s=>observer.observe(s));

document.getElementById('date').min=new Date().toISOString().split('T')[0];
document.querySelector('.m-hour').addEventListener('keydown',e=>{if(e.key==='ArrowUp'||e.key==='ArrowDown')e.stopPropagation()});
</script>
</body>
</html>
