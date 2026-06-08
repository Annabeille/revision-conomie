<!DOCTYPE html>
<html lang="fr">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Marchés concurrentiels · Dossier de révision</title>
<style>
  :root {
    --bg: #1a1d29;
    --card: #252836;
    --text: #e4e6eb;
    --muted: #9ca3af;
    --accent: #7dd3fc;
    --accent2: #fbbf24;
    --accent3: #a78bfa;
    --accent4: #34d399;
    --danger: #f87171;
    --border: #3f4252;
  }

  * { box-sizing: border-box; margin: 0; padding: 0; }

  body {
    font-family: -apple-system, BlinkMacSystemFont, 'Segoe UI', Helvetica, Arial, sans-serif;
    background: var(--bg);
    color: var(--text);
    line-height: 1.6;
    padding: 24px 16px;
    max-width: 900px;
    margin: 0 auto;
    font-size: 15px;
  }

  h1.title {
    font-size: 30px;
    color: var(--accent);
    margin-bottom: 4px;
    font-weight: 700;
    line-height: 1.2;
  }

  .subtitle {
    font-size: 14px;
    color: var(--muted);
    font-style: italic;
    margin-bottom: 28px;
  }

  h2 {
    font-size: 20px;
    color: var(--accent);
    margin-top: 28px;
    margin-bottom: 12px;
    font-weight: 700;
  }

  h3 {
    font-size: 16px;
    color: var(--text);
    margin-top: 16px;
    margin-bottom: 8px;
    font-weight: 700;
  }

  p { margin-bottom: 10px; }

  strong { font-weight: 700; }

  .def, .key, .formula, .tip {
    background: var(--card);
    border-radius: 8px;
    padding: 12px 16px;
    margin: 12px 0;
  }

  .def-title { color: var(--accent3); font-weight: 700; display: block; margin-bottom: 4px; }
  .key-title { color: var(--accent2); font-weight: 700; display: block; margin-bottom: 4px; }

  .formula {
    text-align: center;
    color: var(--accent4);
    font-weight: 700;
    font-size: 18px;
    padding: 14px;
  }

  .tip {
    background: #2a2520;
    font-style: italic;
    font-size: 14px;
  }

  table {
    width: 100%;
    border-collapse: collapse;
    margin: 12px 0;
    font-size: 14px;
    border-radius: 8px;
    overflow: hidden;
  }

  thead { background: var(--accent); }
  thead th {
    color: var(--bg);
    padding: 10px 8px;
    text-align: center;
    font-weight: 700;
  }

  tbody td {
    background: var(--card);
    padding: 8px;
    text-align: center;
    border-bottom: 1px solid var(--bg);
  }

  tbody td:first-child {
    color: var(--accent2);
    font-weight: 700;
  }

  .small-table { font-size: 13px; }
  .small-table td { padding: 6px 4px; }

  .def-table td:first-child {
    color: var(--accent3);
    font-weight: 700;
    width: 28%;
    text-align: left;
    padding-left: 14px;
  }
  .def-table td:last-child {
    text-align: left;
    color: var(--text);
    padding-right: 14px;
  }

  .retenir-table td:first-child {
    color: var(--accent2);
    font-weight: 700;
    width: 26%;
    text-align: left;
    padding: 12px 14px;
  }
  .retenir-table td:last-child {
    text-align: left;
    padding: 12px 14px;
  }

  .formules-table td:first-child {
    color: var(--accent);
    font-weight: 700;
    text-align: left;
    padding-left: 14px;
  }
  .formules-table td:last-child {
    color: var(--accent4);
    font-weight: 700;
    font-size: 16px;
  }

  .prop-table td:first-child {
    color: var(--accent2);
    font-weight: 700;
    font-size: 22px;
    width: 50px;
  }
  .prop-table td:nth-child(2) {
    color: var(--accent);
    font-weight: 700;
    width: 28%;
    text-align: left;
  }
  .prop-table td:last-child {
    text-align: left;
    padding-right: 14px;
  }

  .highlight-max { color: var(--accent4); font-weight: 700; }

  .pos { color: var(--accent4); font-weight: 700; }
  .neg { color: var(--danger); font-weight: 700; }
  .warn { color: var(--accent2); font-weight: 700; }
  .info { color: var(--accent); font-weight: 700; }
  .purple { color: var(--accent3); font-weight: 700; }

  .footer {
    margin-top: 40px;
    padding-top: 20px;
    border-top: 1px solid var(--border);
    color: var(--muted);
    font-size: 12px;
    text-align: center;
  }

  @media (max-width: 600px) {
    body { padding: 16px 12px; font-size: 14px; }
    h1.title { font-size: 24px; }
    h2 { font-size: 18px; }
    table { font-size: 12px; }
    .formula { font-size: 16px; }
    .small-table td { padding: 4px 2px; font-size: 11px; }
    .def-table td:first-child,
    .retenir-table td:first-child { width: 35%; }
  }

  .table-wrapper { overflow-x: auto; -webkit-overflow-scrolling: touch; }
</style>
</head>
<body>

<h1 class="title">Les marchés concurrentiels</h1>
<p class="subtitle">Dossier de révision · production en concurrence parfaite · partie 5b</p>

<!-- ============ 1. MARCHÉ CONCURRENTIEL ============ -->
<h2>1 · Qu'est-ce qu'un marché concurrentiel ?</h2>

<p>
  La <strong>concurrence</strong> apparaît dès que plusieurs entreprises produisent le même bien
  (ou des <strong>biens substituables</strong>), ce qui donne au consommateur le choix selon
  la qualité ou le prix.
</p>

<div class="def">
  <span class="def-title">Marché parfaitement concurrentiel · 2 caractéristiques</span>
  <strong>①</strong> <span class="info">Atomicité</span> : il y a de <strong>nombreux acheteurs
  et de nombreux vendeurs</strong>, chacun trop petit pour influencer le prix.<br>
  <strong>②</strong> <span class="info">Homogénéité</span> : les biens offerts sont
  <strong>similaires / identiques</strong> entre les vendeurs.
</div>

<p>
  Conséquence : les actions individuelles ont un impact <strong>négligeable</strong> sur le prix
  du marché. Les agents doivent accepter le prix imposé → on dit qu'ils sont
  <strong class="info">preneurs de prix</strong> (<em>price takers</em>).
</p>

<div class="key">
  <span class="key-title">★ À retenir · concurrence vs monopole</span>
  <strong>Monopole</strong> = une seule entreprise, <strong>faiseuse de prix</strong> (price maker).<br>
  <strong>Concurrence parfaite</strong> = nombreuses entreprises, <strong>preneuses de prix</strong>
  (price takers).
</div>

<!-- ============ 2. RECETTE ============ -->
<h2>2 · La recette d'une firme concurrentielle</h2>

<p>
  Quelle que soit la forme du marché, l'entreprise cherche à <strong>maximiser son profit</strong>.
  Mais en concurrence, le prix est <strong>imposé par le marché</strong> : si la laiterie double
  sa production, le prix du lait <strong>ne change pas</strong> et sa recette totale double.
</p>

<div class="table-wrapper">
<table>
  <thead>
    <tr>
      <th>Quantité</th><th>Prix</th><th>Recette totale</th>
      <th>Recette moyenne (RM)</th><th>Recette marginale (RMg)</th>
    </tr>
  </thead>
  <tbody>
    <tr><td>1</td><td>6</td><td>6</td><td>6</td><td>6</td></tr>
    <tr><td>2</td><td>6</td><td>12</td><td>6</td><td>6</td></tr>
    <tr><td>3</td><td>6</td><td>18</td><td>6</td><td>6</td></tr>
    <tr><td>4</td><td>6</td><td>24</td><td>6</td><td>6</td></tr>
    <tr><td>5</td><td>6</td><td>30</td><td>6</td><td>6</td></tr>
    <tr><td>6</td><td>6</td><td>36</td><td>6</td><td>6</td></tr>
  </tbody>
</table>
</div>

<div class="formula">Pour une firme concurrentielle : P = RM = RMg</div>

<p>
  La recette moyenne et la recette marginale sont <strong>toutes deux égales au prix</strong>.
  C'est ce qui différencie la concurrence du monopole (où RMg &lt; P).
</p>

<!-- ============ 3. MAXIMISATION DU PROFIT ============ -->
<h2>3 · La maximisation du profit</h2>

<p>L'entreprise choisit la quantité qui maximise son profit (π = RT − CT).</p>

<div class="table-wrapper">
<table class="small-table">
  <thead>
    <tr>
      <th>Q</th><th>RT</th><th>CT</th><th>Profit</th>
      <th>RMg</th><th>CMg</th><th>Variation profit</th>
    </tr>
  </thead>
  <tbody>
    <tr><td>0</td><td>0</td><td>3</td><td>−3</td><td>—</td><td>—</td><td>—</td></tr>
    <tr><td>1</td><td>6</td><td>5</td><td>1</td><td>6</td><td>2</td><td><span class="pos">+4</span></td></tr>
    <tr><td>2</td><td>12</td><td>8</td><td>4</td><td>6</td><td>3</td><td><span class="pos">+3</span></td></tr>
    <tr><td>3</td><td>18</td><td>12</td><td>6</td><td>6</td><td>4</td><td><span class="pos">+2</span></td></tr>
    <tr><td>4</td><td>24</td><td>17</td><td><strong class="highlight-max">7</strong></td><td>6</td><td>5</td><td><span class="pos">+1</span></td></tr>
    <tr><td>5</td><td>30</td><td>23</td><td><strong class="highlight-max">7</strong></td><td>6</td><td>6</td><td><span class="warn">0</span></td></tr>
    <tr><td>6</td><td>36</td><td>30</td><td>6</td><td>6</td><td>7</td><td><span class="neg">−1</span></td></tr>
    <tr><td>7</td><td>42</td><td>38</td><td>4</td><td>6</td><td>8</td><td><span class="neg">−2</span></td></tr>
    <tr><td>8</td><td>48</td><td>47</td><td>1</td><td>6</td><td>9</td><td><span class="neg">−3</span></td></tr>
  </tbody>
</table>
</div>

<p>
  Profit maximal à <strong>Q = 4 ou 5 litres</strong> (profit = 7 CHF). Au-delà, le coût marginal
  dépasse la recette marginale → produire devient une perte.
</p>

<div class="def">
  <span class="def-title">Règle d'or de la maximisation</span>
  <strong>Tant que RMg &gt; CMg</strong> → produire <strong>plus</strong> fait croître le profit.<br>
  <strong>Quand CMg &gt; RMg</strong> → produire moins est mieux (chaque unité supplémentaire coûte
  plus qu'elle ne rapporte).<br>
  → On s'arrête quand <strong>RMg = CMg</strong>.
</div>

<div class="formula">Q<sub>max</sub> tel que &nbsp; RMg = CMg</div>

<p>
  En concurrence parfaite, comme RMg = P, la condition devient : <strong class="info">P = CMg</strong>.
  L'entreprise ajuste sa production jusqu'à ce que le coût marginal égale le prix du marché.
</p>

<!-- ============ 4. COURBE D'OFFRE ============ -->
<h2>4 · La courbe d'offre = la courbe de coût marginal</h2>

<p>
  Quand le prix passe de P₁ à P₂, la RMg dépasse le CMg au niveau de production actuel.
  L'entreprise augmente donc sa production jusqu'à un nouveau Q₂ tel que CMg = P₂.
</p>

<div class="key">
  <span class="key-title">★ Conclusion fondamentale</span>
  La courbe de <strong>coût marginal</strong> indique la quantité que l'entreprise veut offrir
  à chaque prix → c'est <strong>la courbe d'offre concurrentielle</strong>.
</div>

<h3>Quand l'entreprise doit-elle fermer ?</h3>

<div class="table-wrapper">
<table class="def-table">
  <tbody>
    <tr>
      <td><span class="warn">Court terme</span></td>
      <td>L'entreprise ferme si <strong>P &lt; CMV</strong> (coût variable moyen). Mieux vaut
        ne rien produire que de perdre sur chaque unité. Mais elle <strong>paie encore les coûts
        fixes</strong> (loyer...).</td>
    </tr>
    <tr>
      <td><span class="neg">Long terme</span></td>
      <td>L'entreprise <strong>sort définitivement</strong> du marché si <strong>P &lt; CMT</strong>
        (coût moyen total). À long terme, tous les coûts sont récupérables.</td>
    </tr>
  </tbody>
</table>
</div>

<!-- ============ 5. PROFIT GRAPHIQUE ============ -->
<h2>5 · La mesure graphique du profit</h2>

<p>
  En multipliant et divisant par Q, on peut réécrire le profit :
</p>

<div class="formula">π = RT − CT = (RT/Q − CT/Q) × Q = (P − CMT) × Q</div>

<p>
  Graphiquement, le profit est un <strong>rectangle</strong> :<br>
  <strong>›</strong> Hauteur = (P − CMT) → marge unitaire<br>
  <strong>›</strong> Largeur = Q → quantité produite
</p>

<div class="table-wrapper">
<table class="def-table">
  <tbody>
    <tr>
      <td><span class="pos">Profit positif</span></td>
      <td><strong>P &gt; CMT</strong> → l'entreprise réalise des bénéfices. Le rectangle "profit"
        est au-dessus du CMT.</td>
    </tr>
    <tr>
      <td><span class="neg">Perte</span></td>
      <td><strong>P &lt; CMT</strong> → l'entreprise subit des pertes. Maximiser son profit
        signifie alors <strong>minimiser ses pertes</strong>.</td>
    </tr>
  </tbody>
</table>
</div>

<div class="tip">
  <strong>Astuce visuelle</strong> : sur le graphique, repère d'abord Q<sub>max</sub> à
  l'intersection CMg = P, puis lis le CMT à cette quantité. La différence verticale entre P et
  CMT te donne la marge unitaire.
</div>

<!-- ============ 6. OPTIMUMS ============ -->
<h2>6 · Optimum technique vs optimum économique</h2>

<div class="table-wrapper">
<table class="def-table">
  <tbody>
    <tr>
      <td><span class="info">Optimum technique</span></td>
      <td>Quantité qui <strong>minimise le coût moyen total</strong>. C'est le point où
        <strong>CMg coupe CMT en son minimum</strong>. Maximise le <em>bénéfice unitaire</em>
        (par unité produite).</td>
    </tr>
    <tr>
      <td><span class="warn">Optimum économique</span></td>
      <td>Quantité qui <strong>maximise le profit total</strong>. C'est le point où
        <strong>CMg = RMg</strong> (= P en concurrence). C'est <em>ce que cherche réellement
        l'entreprise</em>.</td>
    </tr>
  </tbody>
</table>
</div>

<div class="key">
  <span class="key-title">★ Attention à ne pas confondre</span>
  L'optimum <strong>technique</strong> maximise le bénéfice <em>par unité</em>, mais pas le
  bénéfice total. L'optimum <strong>économique</strong> (CMg = RMg) est presque toujours à une
  quantité <strong>supérieure</strong>, car continuer à produire reste rentable tant que chaque
  unité supplémentaire rapporte plus qu'elle ne coûte.
</div>

<!-- ============ À RETENIR ============ -->
<h2>★ À retenir absolument</h2>

<div class="table-wrapper">
<table class="retenir-table">
  <tbody>
    <tr>
      <td>Marché concurrentiel</td>
      <td><strong>Nombreux acheteurs + nombreux vendeurs</strong> (atomicité) et
        <strong>biens homogènes</strong>.</td>
    </tr>
    <tr>
      <td>Preneur de prix</td>
      <td>En concurrence parfaite, l'entreprise <strong>subit le prix</strong> du marché. Sa
        courbe de demande est <strong>horizontale</strong>.</td>
    </tr>
    <tr>
      <td>RM = RMg = P</td>
      <td>En concurrence, recette moyenne = recette marginale = prix. La RMg ne dépend pas de Q.</td>
    </tr>
    <tr>
      <td>Règle d'or</td>
      <td>L'entreprise maximise son profit en produisant Q tel que <strong>RMg = CMg</strong>.
        En concurrence : <strong>P = CMg</strong>.</td>
    </tr>
    <tr>
      <td>Courbe d'offre = CMg</td>
      <td>La courbe de coût marginal d'une firme concurrentielle <strong>est sa courbe d'offre</strong>.</td>
    </tr>
    <tr>
      <td>Fermeture court terme</td>
      <td>Si <strong>P &lt; CMV</strong> → fermer temporairement. Les coûts fixes restent à payer.</td>
    </tr>
    <tr>
      <td>Sortie long terme</td>
      <td>Si <strong>P &lt; CMT</strong> → quitter définitivement le marché.</td>
    </tr>
    <tr>
      <td>Mesure du profit</td>
      <td><strong>π = (P − CMT) × Q</strong>. Rectangle dont hauteur = marge unitaire et largeur
        = quantité.</td>
    </tr>
    <tr>
      <td>Optimum technique vs économique</td>
      <td><strong>Technique</strong> : min(CMT), max bénéfice unitaire. <strong>Économique</strong> :
        CMg = RMg, max profit total. <strong>L'entreprise choisit l'économique.</strong></td>
    </tr>
  </tbody>
</table>
</div>

<div class="footer">
  Révisions maturité · OS Économie · CECG Madame de Staël
</div>

</body>
</html>
