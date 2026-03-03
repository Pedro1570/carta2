<!doctype html>
<html lang="pt-BR">
<head>
  <meta charset="utf-8" />
  <meta name="viewport" content="width=device-width,initial-scale=1" />
  <title>Cartão para você</title>
  <style>
    :root{
      --bg:#fff9f6;
      --card:#fff;
      --accent:#D96A6A;
      --spotify-green:#1DB954;
      --text:#333;
      --muted:#666;
    }
    *{box-sizing:border-box}
    body{
      margin:0;
      font-family: -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, "Helvetica Neue", Arial;
      background:linear-gradient(180deg,#fff9f6 0%, #27a852 100%);
      display:flex;
      align-items:center;
      justify-content:center;
      min-height:100vh;
      color:var(--text);
      padding:20px;
    }

    .card{
      background:var(--card);
      padding:22px;
      border-radius:12px;
      box-shadow:0 8px 30px rgba(0,0,0,0.08);
      max-width:900px;
      width:100%;
      display:flex;
      gap:18px;
      align-items:center;
    }

    /* Texto */
    .content{flex:1}
    h1{ margin:0 0 8px 0; font-size:20px; color:var(--accent) }
    p{ margin:10px 0; line-height:1.5 }
    .assinatura{ margin-top:14px; font-weight:600 }
    .footer{ margin-top:12px; color:var(--muted); font-size:13px }

    /* Moldura estilo "Spotify" */
    .photo-panel{
      width:260px;
      flex:0 0 260px;
      display:flex;
      align-items:center;
      justify-content:center;
    }

    .spotify-frame{
      width:100%;
      border-radius:18px;
      padding:10px;
      background:linear-gradient(180deg, rgba(29,185,84,0.12), rgba(29,185,84,0.06));
      box-shadow: inset 0 1px 0 rgba(255,255,255,0.5), 0 6px 18px rgba(16,32,20,0.06);
      border: 1px solid rgba(29,185,84,0.18);
    }

    .frame-inner{
      background:#fff;
      border-radius:12px;
      overflow:hidden;
      position:relative;
    }

    .frame-inner img{
      display:block;
      width:100%;
      height:260px;
      object-fit:cover;
    }

    /* Ícone de play discreto */
    .play{
      position:absolute;
      right:10px;
      bottom:10px;
      background: rgba(0,0,0,0.55);
      border: none;
      width:44px;
      height:44px;
      border-radius:50%;
      display:flex;
      align-items:center;
      justify-content:center;
      cursor:default;
      box-shadow: 0 4px 10px rgba(0,0,0,0.2);
    }
    .play svg{ fill:#fff; width:18px; height:18px }

    .badge{
      margin-top:8px;
      display:flex;
      align-items:center;
      gap:8px;
      color:var(--spotify-green);
      font-weight:600;
      font-size:13px;
    }

    .badge .dot{
      width:12px;
      height:12px;
      background:var(--spotify-green);
      border-radius:50%;
      box-shadow:0 1px 0 rgba(0,0,0,0.08) inset;
    }

    /* Responsivo */
    @media (max-width:720px){
      .card{ flex-direction:column; padding:18px }
      .photo-panel{ width:100%; flex:0 0 auto }
      .frame-inner img{ height:200px }
    }
  </style>
</head>
<body>
  <article class="card" role="article" aria-label="Cartão de amor">
    <div class="content">
      <h1>Para você, meu amor</h1>

      <p>Quero te agradecer por sempre estar do meu lado, quando tudo tem sido tão difícil vc sempre está comigo. Sua presença me dá força e paz nos dias em que eu mais preciso.</p>

      <p>Admiro você e o seu ministério — quando você canta, meu coração se acalma; ver você ministrar é uma das coisas que mais me encanta. <em>Amo ver você cantando.</em></p>

      <p>Obrigado por orar por mim e por não desistir de mim, mesmo quando eu me sinto fraco.</p>

      <p>Te amo muito. Prometo estar com você, orar junto e cuidar do que temos com todo carinho.</p>

      <p class="assinatura">Com todo o meu amor,<br>Seu Neném</p>

      <div class="footer">Observação: substitua <code>images/foto.jpg</code> pela sua foto (caminho local ou URL). Se quiser, eu subo a imagem no seu repositório — me envie owner/name e o caminho onde quer guardar.</div>
    </div>

    <div class="photo-panel" aria-hidden="false">
      <div class="spotify-frame" title="Sua foto com moldura">
        <div class="frame-inner">
          <!-- Troque o src abaixo pela URL ou caminho da sua foto -->
          <img src="c:\Users\ALL\Downloads\eueaana.jpeg" alt="Sua foto"/>
          <button class="play" aria-hidden="true" tabindex="-1">
            <!-- Ícone de play simples -->
            <svg viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg" aria-hidden="true">
              <path d="M8 5v14l11-7z"/>
            </svg>
          </button>
        </div>
        <div class="badge"><span class="dot" aria-hidden="true"></span>no Spotify</div>
      </div>
    </div>
  </article>
</body>
</html>
