# resume.html.
<!doctype html>
<html lang="zh-Hant">
<head>
  <meta charset="utf-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1" />
  <title>個人履歷 — 姓名</title>
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

    /* 左側個人卡 */
    .card{background:var(--card);border-radius:16px;padding:20px;box-shadow:0 6px 20px rgba(15,23,42,0.06);}
    .profile-photo{width:100%;aspect-ratio:1/1;border-radius:12px;object-fit:cover;background:#e6eefc;display:block;margin-bottom:14px}
    .name{font-size:20px;font-weight:700;margin:6px 0}
    .title{font-size:13px;color:var(--muted);margin-bottom:12px}
    .contact{font-size:14px;color:#111827}
    .contact a{color:var(--accent);text-decoration:none}
    .skills{display:flex;flex-wrap:wrap;gap:8px;margin-top:12px}
    .skill{background:var(--glass);padding:6px 10px;border-radius:999px;font-size:13px;color:#0f172a;border:1px solid rgba(15,23,42,0.04)}

    /* 右側內容 */
    .content{padding:20px;background:linear-gradient(180deg,rgba(255,255,255,0.9),#ffffff);border-radius:16px;box-shadow:0 6px 20px rgba(15,23,42,0.04)}
    section{margin-bottom:18px}
    h2{font-size:16px;margin:0 0 10px 0}
    .muted{color:var(--muted);font-size:14px}

    .job{padding:12px;border-left:3px solid rgba(37,99,235,0.08);margin-bottom:10px}
    .job h3{margin:0;font-size:15px}
    .job .meta{font-size:13px;color:var(--muted);margin-top:4px}
    ul{margin:8px 0 0 20px}

    /* Footer / contact bar */
    .contact-bar{display:flex;gap:12px;flex-wrap:wrap;margin-top:10px}
    .btn{background:transparent;border:1px solid rgba(15,23,42,0.06);padding:8px 12px;border-radius:8px;font-weight:600}

    /* Responsive */
    @media (max-width:880px){
      .container{grid-template-columns:1fr;}
      .card{order:2}
      .content{order:1}
    }

    /* Print-friendly */
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
    <!-- 左側個人資訊卡：請將圖片檔放到同個資料夾下的 images/profile.jpg 或修改下面 img 的 src -->
    <aside class="card">
      <img class="profile-photo" src="images/profile.jpg" alt="個人照片（請替換成你的照片）">
      <div class="name">你的姓名</div>
      <div class="title">職稱 / 專長（例如：前端工程師｜產品設計）</div>

      <div class="contact">
        <div class="muted">聯絡方式</div>
        <div class="contact-bar">
          <div>✉️ <a href="mailto:you@example.com">you@example.com</a></div>
          <div>📱 0912-345-678</div>
          <div>🔗 <a href="#">linkedin.com/in/yourname</a></div>
        </div>
      </div>

      <div style="margin-top:14px">
        <div class="muted">技能</div>
        <div class="skills">
          <div class="skill">HTML</div>
          <div class="skill">CSS</div>
          <div class="skill">JavaScript</div>
          <div class="skill">React</div>
          <div class="skill">UI 設計</div>
        </div>
      </div>

      <div style="margin-top:14px">
        <div class="muted">語言</div>
        <div class="skills">
          <div class="skill">中文（母語）</div>
          <div class="skill">英文（中上）</div>
        </div>
      </div>
    </aside>

    <!-- 右側履歷內容 -->
    <main class="content">
      <section>
        <h2>個人簡介</h2>
        <p class="muted">一句到兩句，簡潔描述你的專業定位與職涯目標。例如：具有 3 年前端開發經驗，擅長打造響應式網站與元件化 UI，期望加入以使用者為中心的產品團隊。</p>
      </section>

      <section>
        <h2>工作經歷</h2>
        <article class="job">
          <h3>公司名稱 — 職稱</h3>
          <div class="meta">2022/07 — 現在 · 台北</div>
          <ul>
            <li>主導 XXX 專案，負責前端架構與元件設計，提升網站效能 30%。</li>
            <li>與設計、後端協作，將設計系統化並導入自動化測試流程。</li>
          </ul>
        </article>

        <article class="job">
          <h3>公司名稱 — 職稱</h3>
          <div class="meta">2020/09 — 2022/06 · 新北</div>
          <ul>
            <li>參與產品上線與維護，負責多頁面網站切版與互動。</li>
          </ul>
        </article>
      </section>

      <section>
        <h2>學歷</h2>
        <div class="muted">2016 — 2020 • 國立某某大學 • 資訊工程學系</div>
      </section>

      <section>
        <h2>專案</h2>
        <div class="job">
          <h3>專案名稱（連結）</h3>
          <div class="meta">簡短描述 • 使用技術：HTML, CSS, JavaScript</div>
          <ul>
            <li>功能或挑戰：例如：實作自適應卡片排列、加入無障礙（a11y）考量。</li>
          </ul>
        </div>
      </section>

      <section>
        <h2>其他資訊</h2>
        <p class="muted">興趣、證照、志工經驗或可提供的作品連結（Portfolio / GitHub）。</p>
        <div style="margin-top:8px">
          <button class="btn">下載 PDF 履歷（示意）</button>
          <button class="btn">查看作品集</button>
        </div>
      </section>
    </main>
  </div>

  <!-- 使用說明（可刪除）：
       1. 將本檔案儲存為 index.html。
       2. 新增資料夾 images/ 並放入你的個人照片，檔名為 profile.jpg，或直接修改 <img> 的 src。
       3. 在瀏覽器中開啟 index.html 以預覽。
  -->
</body>
</html>
      </section>
    </main>
  </div>

</body>
</html>
