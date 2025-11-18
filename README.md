<!doctype html>
<html lang="pt-BR">
<head>
  <meta charset="utf-8" />
  <meta name="viewport" content="width=device-width,initial-scale=1" />
  <title>Bolo Fit de Banana — Receita</title>
  <style>
    :root{--bg:#fff;--card:#fafafa;--accent:#6b8e23;--muted:#666}
    body{font-family:system-ui,-apple-system,Segoe UI,Roboto,Helvetica,Arial;line-height:1.5;background:linear-gradient(180deg,#fbfbfb,#f5f7f9);margin:0;padding:16px;color:#222}

    .container{max-width:900px;margin:0 auto;background:var(--card);border-radius:12px;padding:20px;box-shadow:0 8px 30px rgba(20,30,50,0.06)}

    header{display:flex;gap:16px;align-items:center;flex-wrap:wrap}
    .thumb{flex:1 1 260px;min-width:220px;border-radius:10px;overflow:hidden;box-shadow:0 6px 18px rgba(20,30,50,0.06)}
    .thumb img{display:block;width:100%;height:100%;object-fit:cover}

    h1{margin:0;font-size:1.8rem}
    p.lead{margin:6px 0 0;color:var(--muted)}

    .grid{display:grid;grid-template-columns:1fr 320px;gap:20px;margin-top:20px}

    .card{background:white;padding:18px;border-radius:10px;box-shadow:0 4px 14px rgba(15,20,30,0.03)}
    ul.ingredients{list-style:none;padding:0;margin:0}
    ul.ingredients li{padding:6px 0;border-bottom:1px dashed #eee}

    .steps{counter-reset:step;margin:0;padding:0}
    .steps li{display:block;padding:12px 0;border-bottom:1px solid #faf0e6;position:relative;margin-left:40px}
    .steps li::before{counter-increment:step;content:counter(step);position:absolute;left:-40px;top:12px;background:var(--accent);color:white;width:28px;height:28px;line-height:28px;border-radius:50%;text-align:center;font-weight:600}

    .meta{font-size:0.95rem;color:var(--muted);margin-top:8px}
    .actions{display:flex;gap:10px;flex-wrap:wrap;margin-top:12px}
    button{background:var(--accent);border:0;color:white;padding:10px 14px;border-radius:8px;cursor:pointer}
    button.secondary{background:#eee;color:#333}

    footer{margin-top:22px;font-size:0.9rem;color:var(--muted)}

    /* RESPONSIVIDADE */
    @media (max-width:900px){
      .grid{grid-template-columns:1fr}
      body{padding:10px}
    }

    @media (max-width:600px){
      h1{font-size:1.5rem}
      .container{padding:16px}
      .steps li{margin-left:36px}
      .steps li::before{left:-34px;width:26px;height:26px;line-height:26px}
    }

    @media (max-width:420px){
      .thumb{min-width:100%;height:200px}
      .actions button{flex:1}
      .grid{gap:14px}
    }
  </style>
</head>
<body>
  <div class="container">
    <header>
      <div class="thumb">
        <!-- Imagem representativa: banana bread / fit -->
        <img src="https://receitadaboa.com.br/wp-content/uploads/2024/09/Imagem-ilustrativa-de-bolinho-de-banana.webp" alt="Bolo fit de banana fatiado com granola e chocolate" />
      </div>
      <div>
        <h1>BOLO FIT DE BANANA</h1>
        <p class="lead">Rendimento: 4 porções • Tempo aproximado: 25–30 min (airfryer)</p>
        <div class="meta">Ingredientes simples, opção com chocolate 80% e granola para crocância.</div>
        <div class="actions">
          <button onclick="window.print()">Imprimir receita</button>
          <button class="secondary" onclick="downloadHTML()">Baixar página (HTML)</button>
        </div>
      </div>
    </header>

    <div class="grid">
      <main class="card">
        <h2>Ingredientes (4 porções)</h2>
        <ul class="ingredients">
          <li>1 banana madura grande</li>
          <li>1 ovo inteiro</li>
          <li>1/2 xícara de farinha de aveia integral</li>
          <li>Canela a gosto</li>
          <li>1 colher (chá) cheia de fermento</li>
          <li>50 g de chocolate 80% (pedaços ou gotas)</li>
          <li>50 g de granola</li>
        </ul>

        <h2 style="margin-top:18px">Modo de preparo</h2>
        <ol class="steps">
          <li>Amasse a banana até ficar um purê homogêneo.</li>
          <li>Adicione o ovo e misture bem até incorporar.</li>
          <li>Adicione a farinha de aveia, a canela em pó e a granola; misture até obter uma massa uniforme.</li>
          <li>O fermento vai por último; incorpore delicadamente em velocidade baixa (ou mexa suavemente).</li>
          <li>Coloque a massa nas forminhas de silicone e acrescente o chocolate a gosto (por cima ou misturado).</li>
          <li>Leve para assar na airfryer — o tempo varia conforme o modelo; quando desligar e puxar a bandeja, faça o teste do palito: se sair limpo, está pronto.</li>
        </ol>

        <p class="meta">Dicas: use banana bem madura para mais doce natural; se preferir menos doce, reduza o chocolate ou use apenas 30 g.</p>
      </main>

      <aside class="card">
        <h3>Nutrição & Porções</h3>
        <p class="meta">Estimativa por porção (aprox.): 220–260 kcal — depende do tamanho da banana e do chocolate usado.</p>

        <h3 style="margin-top:12px">Variações</h3>
        <ul>
          <li>Substitua a granola por nozes picadas para mais proteína.</li>
          <li>Use cacau em pó (1 colher de sopa) na massa para versão chocolateada.</li>
          <li>Versão vegana: substitua o ovo por 2 colheres de sopa de purê extra de banana ou 1 colher de sopa de farinha de linhaça + 3 colheres de sopa de água (deixe hidratar).</li>
        </ul>

        <h3 style="margin-top:12px">Informações rápidas</h3>
        <p class="meta">Equipamento: airfryer (ou forno convencional). Forminhas: silicone ou papel.</p>
      </aside>
    </div>
  </div>

  <script>
    function downloadHTML(){
      const blob = new Blob([document.documentElement.outerHTML], {type: 'text/html'});
      const url = URL.createObjectURL(blob);
      const a = document.createElement('a');
      a.href = url;
      a.download = 'bolo-fit-banana.html';
      document.body.appendChild(a);
      a.click();
      a.remove();
      URL.revokeObjectURL(url);
    }
  </script>
</body>
</html>
