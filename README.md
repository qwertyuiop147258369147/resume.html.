# resume.html.
<!doctype html>
<html lang="zh-Hant">
<head>
  <meta charset="utf-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1" />
  <title>個人履歷 — 吳秉澤</title>
  <link rel="preconnect" href="https://fonts.googleapis.com">
  <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
  <link href="https://fonts.googleapis.com/css2?family=Inter:wght@300;400;600;700&display=swap" rel="stylesheet">
  <style>
    :root{
      --bg:#f6f8fb; --card:#ffffff; --muted:#6b7280; --accent:#2563eb;
      --glass: rgba(255,255,255,0.6);
    }
    *{box-sizing:border-box}
    html,body{height:100%;margin:0;font-family:Inter,system-ui,-apple-system,"Segoe UI",Roboto,'Noto Sans TC',"Helvetica Neue",Arial}
    body{background:linear-gradient(180deg,var(--bg),#ffffff);color:#0f172a;padding:32px}

    .container{max-width:1000px;margin:0 auto;display:grid;grid-template-columns:320px 1fr;gap:24px}

    .card{background:var(--card);border-radius:16px;padding:20px;box-shadow:0 6px 20px rgba(15,23,42,0.06);}
    .profile-photo{width:100%;aspect-ratio:1/1;border-radius:12px;object-fit:cover;background:#e6eefc;display:block;margin-bottom:14px}
    .name{font-size:20px;font-weight:700;margin:6px 0}
    .contact{font-size:14px;color:#111827}
    .contact a{color:var(--accent);text-decoration:none}
    .skills{display:flex;flex-wrap:wrap;gap:8px;margin-top:12px}
    .skill{background:var(--glass);padding:6px 10px;border-radius:999px;font-size:13px;color:#0f172a;border:1px solid rgba(15,23,42,0.04)}

    .content{padding:20px;background:linear-gradient(180deg,rgba(255,255,255,0.9),#ffffff);border-radius:16px;box-shadow:0 6px 20px rgba(15,23,42,0.04)}
    section{margin-bottom:18px}
    h2{font-size:16px;margin:0 0 10px 0}
    .muted{color:var(--muted);font-size:14px}

    .job{padding:12px;border-left:3px solid rgba(37,99,235,0.08);margin-bottom:10px}
    .job h3{margin:0;font-size:15px}
    .job .meta{font-size:13px;color:var(--muted);margin-top:4px}
    ul{margin:8px 0 0 20px}

    .contact-bar{display:flex;gap:12px;flex-wrap:wrap;margin-top:10px}

    @media (max-width:880px){
      .container{grid-template-columns:1fr;}
      .card{order:2}
      .content{order:1}
    }

    @media print{
      body{padding:0}
      .container{max-width:100%;grid-template-columns:1fr}
      .card .profile-photo{display:none}
      .content, .card{box-shadow:none;border-radius:0}
    }
  </style>
</head>
<body>
  <div class="container">
    <aside class="card">
      <img class="profile-photo" src="images/profile.jpg" alt="個人照片（請替換成你的照片）">
      <div class="name">吳秉澤</div>

      <div class="contact">
        <div class="muted">聯絡方式</div>
        <div class="contact-bar">
          <div>✉️ <a href="mailto:hallow3096@gmail.com">hallow3096@gmail.com</a></div>
          <div>📱 0962077962</div>
        </div>
      </div>

      <div style="margin-top:14px">
        <div class="muted">技能</div>
        <div class="skills">
          <div class="skill">打掃</div>
          <div class="skill">煮飯</div>
        </div>
      </div>
    </aside>

    <main class="content">
      <section>
        <h2>個人簡介</h2>
        <p class="muted">我來自新北中和，有一點點社交恐懼，但是不用認識多久就會很活潑，面對考試的心態是臨時抱佛腳。</p>
      </section>

      <section>
        <h2>工作經歷</h2>
        <article class="job">
          <h3>補習班工讀生</h3>
        </article>
      </section>

      <section>
        <h2>興趣</h2>
        <div class="skills">
          <div class="skill">打遊戲</div>
          <div class="skill">看漫畫</div>
        </div>
      </section>
    </main>
  </div>

</body>
</html>
