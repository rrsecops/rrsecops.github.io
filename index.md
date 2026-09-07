---
layout: home
title: "Renildo Rocha | Blue Team & SecOps"
---
<section class="hero">
  <div class="eyebrow">BLUE TEAM · SECOPS · DETECTION ENGINEERING</div>
  <h1>Renildo Rocha</h1>
  <p class="hero-lead">Operações de Segurança Defensiva.</p>
  <p class="hero-copy">Explorando o ofício de Blue Team, engenharia de detecção e resposta a ameaças. Este espaço é dedicado a documentar estudos, laboratórios e cenários práticos para elevar o nível da operação.</p>
  <div class="hero-actions">
    <a class="button button-primary" href="{{ '/start-here/' | relative_url }}">Comece aqui</a>
    <a class="button" href="{{ '/articles/' | relative_url }}">Últimos Artigos</a>
  </div>
</section>

<section class="section highlight-series">
  <div class="section-heading"><span class="section-kicker">SÉRIE EM DESTAQUE</span><h2>FortiAnalyzer Além dos Relatórios</h2></div>
  <p class="lead">Do log à detecção. Da detecção à ação. Uma exploração prática de como utilizar as capacidades do FortiAnalyzer para apoiar a operação de segurança.</p>
  
  <div class="cards cards-3">
    <a class="feature-card" href="{{ '/secops/' | relative_url }}"><span class="card-label">SECOPS</span><h3>Visão Operacional</h3><p>Detecção, investigação, hunting, correlação e automação.</p></a>
    <a class="feature-card" href="{{ '/labs/' | relative_url }}"><span class="card-label">LABS</span><h3>Experimentos</h3><p>Hipótese, implementação, validação, tuning e lições aprendidas.</p></a>
    <a class="feature-card" href="{{ '/detections/' | relative_url }}"><span class="card-label">DETECTIONS</span><h3>Catálogo</h3><p>Detecções documentadas, versionadas e relacionadas aos Labs.</p></a>
  </div>
</section>

<section class="lifecycle">
  <div class="section-heading"><span class="section-kicker">SECOPS LIFECYCLE</span><h2>Do dado à ação</h2></div>
  <div class="flow">
    <div class="flow-step"><strong>01</strong><span>LOGS</span></div><div class="flow-arrow">→</div>
    <div class="flow-step"><strong>02</strong><span>DETECT</span></div><div class="flow-arrow">→</div>
    <div class="flow-step"><strong>03</strong><span>CORRELATE</span></div><div class="flow-arrow">→</div>
    <div class="flow-step"><strong>04</strong><span>INVESTIGATE</span></div><div class="flow-arrow">→</div>
    <div class="flow-step"><strong>05</strong><span>RESPOND</span></div><div class="flow-arrow">→</div>
    <div class="flow-step"><strong>06</strong><span>AUTOMATE</span></div>
  </div>
</section>

<section class="section">
  <div class="section-heading inline"><div><span class="section-kicker">LATEST ARTICLES</span><h2>Últimos artigos</h2></div><a href="{{ '/articles/' | relative_url }}">Ver todos →</a></div>
  <div class="post-list">
  {% for post in site.posts limit:3 %}
    <article class="post-card"><div class="post-meta">{{ post.date | date: "%d/%m/%Y" }} · {{ post.category | default: "ARTICLE" }}</div><h3><a href="{{ post.url | relative_url }}">{{ post.title }}</a></h3><p>{{ post.excerpt | strip_html | truncate: 180 }}</p></article>
  {% else %}<div class="empty-state">Os primeiros artigos serão publicados aqui.</div>{% endfor %}
  </div>
</section>

<section class="manifesto-callout"><span class="section-kicker">A QUESTION TO KEEP</span><blockquote>“O que podemos detectar, investigar e aprender com os dados que já temos?”</blockquote></section>
