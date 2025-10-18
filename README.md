<html lang="ru">
<head>
  <meta charset="utf-8">
  <meta name="viewport" content="width=device-width,initial-scale=1">
  <title>Мой сайт — стартовая страница</title>

  <style>
    :root{
      --bg:#0f1724; --card:#0b1220; --accent:#7c3aed; --muted:#9aa4b2; --glass: rgba(255,255,255,0.04);
      --radius:14px; --fw-strong:700; --fw-normal:400; --maxw:1100px;
    }
    *{box-sizing:border-box}
    html,body{height:100%;margin:0;font-family:Inter, ui-sans-serif, system-ui, -apple-system, "Segoe UI", Roboto, "Helvetica Neue", Arial;color:#e6eef6;background:linear-gradient(180deg,#071025 0%, #07192b 100%);}
    .wrap{max-width:var(--maxw);margin:36px auto;padding:24px}

    /* NAV */
    header{display:flex;align-items:center;justify-content:space-between;gap:16px}
    .brand{display:flex;align-items:center;gap:12px}
    .logo{width:44px;height:44px;border-radius:10px;background:linear-gradient(135deg,var(--accent),#0ea5a3);display:flex;align-items:center;justify-content:center;color:white;font-weight:800}
    nav ul{display:flex;gap:18px;list-style:none;padding:0;margin:0}
    nav a{color:var(--muted);text-decoration:none;font-weight:600}
    .cta{background:var(--accent);color:#fff;padding:10px 14px;border-radius:10px;text-decoration:none;font-weight:700}

    /* HERO */
    .hero{display:grid;grid-template-columns:1fr 380px;gap:28px;align-items:center;margin-top:28px}
    .hero-card{background:linear-gradient(180deg, rgba(255,255,255,0.02), rgba(255,255,255,0.01));border-radius:18px;padding:28px;box-shadow:0 6px 30px rgba(2,6,23,0.6);}
    h1{margin:0;font-size:34px;line-height:1.02}
    p.lead{color:var(--muted);margin-top:12px}
    .actions{display:flex;gap:12px;margin-top:18px}

    /* FEATURES */
    .features{display:grid;grid-template-columns:repeat(3,1fr);gap:16px;margin-top:36px}
    .feature{background:var(--card);padding:18px;border-radius:12px}

    /* PORTFOLIO */
    .portfolio{display:grid;grid-template-columns:repeat(3,1fr);gap:12px;margin-top:24px}
    .tile{height:120px;border-radius:10px;background:linear-gradient(180deg, rgba(255,255,255,0.02), rgba(255,255,255,0.01));display:flex;align-items:flex-end;padding:12px;color:#fff;font-weight:700}

    /* CONTACT */
    form{display:grid;gap:12px}
    input,textarea{width:100%;padding:12px;border-radius:10px;border:1px solid rgba(255,255,255,0.04);background:transparent;color:inherit}
    button{padding:10px 14px;border-radius:10px;border:0;background:var(--accent);color:white;font-weight:700}

    footer{margin-top:36px;color:var(--muted);font-size:14px}

    /* Responsive */
    @media (max-width:900px){
      .hero{grid-template-columns:1fr;}
      .features{grid-template-columns:repeat(2,1fr)}
      .portfolio{grid-template-columns:repeat(2,1fr)}
    }
    @media (max-width:560px){
      nav ul{display:none}
      .hero{gap:18px}
      .features{grid-template-columns:1fr}
      .portfolio{grid-template-columns:1fr}
    }

  </style>
</head>
<body>
  <div class="wrap">
    <header>
      <div class="brand">
        <div class="logo">MS</div>
        <div>
          <div style="font-weight:800">Мой Сайт</div>
          <div style="font-size:12px;color:var(--muted)">Красивый стартовый шаблон</div>
        </div>
      </div>

      <nav>
        <ul>
          <li><a href="#about">О нас</a></li>
          <li><a href="#work">Работы</a></li>
          <li><a href="#contact">Контакты</a></li>
        </ul>
      </nav>

      <a class="cta" href="#contact">Связаться</a>
    </header>

    <section class="hero">
      <div class="hero-card">
        <h1>Простой, быстрый и адаптивный сайт</h1>
        <p class="lead">Шаблон для презентации ваших услуг, портфолио или лендинга. Лёгко кастомизируется — замените текст, цвета и картинки.</p>
        <div class="actions">
          <a class="cta" href="#work">Посмотреть работы</a>
          <a href="#about" style="padding:10px 14px;border-radius:10px;background:transparent;border:1px solid rgba(255,255,255,0.04);color:var(--muted);text-decoration:none;font-weight:700">Узнать больше</a>
        </div>

        <div style="margin-top:22px;display:flex;gap:12px;flex-wrap:wrap;color:var(--muted)">
          <div style="background:var(--glass);padding:10px;border-radius:10px">Высокая скорость</div>
          <div style="background:var(--glass);padding:10px;border-radius:10px">Адаптивность</div>
          <div style="background:var(--glass);padding:10px;border-radius:10px">Лёгкая настройка</div>
        </div>
      </div>

      <aside class="hero-card">
        <h3 style="margin-top:0">Контактная карточка</h3>
        <p class="lead">Нужна помощь с сайтом? Напиши — и я помогу с дизайном, кодом и деплоем.</p>
        <div style="margin-top:12px;font-weight:700">email: info@example.com</div>
        <div style="margin-top:8px;color:var(--muted)">Тел: +420 123 456 789</div>
      </aside>
    </section>

    <section id="about" style="margin-top:28px">
      <h2>Наши услуги</h2>
      <div class="features">
        <div class="feature">Веб-дизайн — от прототипа до финала</div>
        <div class="feature">Front-end разработка — HTML/CSS/JS</div>
        <div class="feature">Деплой — GitHub Pages, Netlify, Vercel</div>
      </div>
    </section>

    <section id="work">
      <h2 style="margin-top:28px">Портфолио</h2>
      <div class="portfolio">
        <div class="tile">Проект A</div>
        <div class="tile">Проект B</div>
        <div class="tile">Проект C</div>
        <div class="tile">Проект D</div>
        <div class="tile">Проект E</div>
        <div class="tile">Проект F</div>
      </div>
    </section>

    <section id="contact" style="margin-top:28px">
      <h2>Связаться</h2>
      <div style="display:grid;grid-template-columns:1fr 360px;gap:18px;margin-top:12px">
        <div class="hero-card">
          <form id="contactForm" onsubmit="return false">
            <input type="text" id="name" placeholder="Ваше имя" required>
            <input type="email" id="email" placeholder="Email" required>
            <textarea id="message" rows="5" placeholder="Сообщение"></textarea>
            <div style="display:flex;gap:8px;align-items:center">
              <button id="sendBtn">Отправить</button>
              <div id="notice" style="color:var(--muted);font-size:13px">Форма не отправляет сообщения — это шаблон.</div>
            </div>
          </form>
        </div>

        <div class="hero-card">
          <h4 style="margin:0">Адрес</h4>
          <p class="lead">Улица Примерная 12, Братислава</p>

          <h4 style="margin-top:18px">Контакт</h4>
          <p class="lead">info@example.com<br>+420 123 456 789</p>
        </div>
      </div>
    </section>

    <footer>
      © 2025 — Мой Сайт. Все права защищены.
    </footer>
  </div>

  <script>
    // Простая валидация формы
    document.getElementById('sendBtn').addEventListener('click', function(){
      const name = document.getElementById('name').value.trim();
      const email = document.getElementById('email').value.trim();
      if(!name || !email){
        alert('Пожалуйста, заполните имя и email.');
        return;
      }
      // демонстрация: сохраняем данные в localStorage
      const data = {name, email, message: document.getElementById('message').value};
      const list = JSON.parse(localStorage.getItem('messages')||'[]');
      list.push({...data, at: new Date().toISOString()});
      localStorage.setItem('messages', JSON.stringify(list));
      alert('Спасибо! Сообщение сохранено локально (шаблон).');
      document.getElementById('contactForm').reset();
    });

    // Простая плавная прокрутка
    document.querySelectorAll('a[href^="#"]').forEach(a=>{
      a.addEventListener('click', function(e){
        e.preventDefault();
        const id = this.getAttribute('href').slice(1);
        const el = document.getElementById(id);
        if(el) el.scrollIntoView({behavior:'smooth',block:'start'});
      });
    });
  </script>
</body>
</html>
