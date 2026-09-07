---
layout: home
title: "FortiAnalyzer Além dos Relatórios"
---
<section class="hero">
  <div class="eyebrow">SECOPS · DETECTION ENGINEERING · THREAT HUNTING</div>
  <h1>FortiAnalyzer<br><span>Além dos Relatórios</span></h1>
  <p class="hero-lead">Do log à detecção. Da detecção à ação.</p>
  <p class="hero-copy">Uma exploração prática de como o FortiAnalyzer pode apoiar operações de segurança, detecção, investigação, threat hunting, correlação e automação.</p>
  <div class="hero-actions">
    <a class="button button-primary" href="{{ '/start-here/' | relative_url }}">Comece aqui</a>
    <a class="button" href="{{ '/labs/' | relative_url }}">Explorar Labs</a>
  </div>
</section>

<section class="section">
  <div class="section-heading"><span class="section-kicker">THE IDEA</span><h2>O problema não é ter logs. É saber o que fazer com eles.</h2></div>
  <p class="lead">FortiAnalyzer é frequentemente associado a logs e relatórios. Esta iniciativa parte de outra perspectiva: como utilizar os dados e capacidades disponíveis para apoiar uma operação de segurança?</p>
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
  <div class="cards cards-3">
    <a class="feature-card" href="{{ '/secops/' | relative_url }}"><span class="card-label">SECOPS</span><h3>Problemas operacionais</h3><p>Detecção, investigação, hunting, correlação, resposta e automação.</p></a>
    <a class="feature-card" href="{{ '/labs/' | relative_url }}"><span class="card-label">LABS</span><h3>Experimentos práticos</h3><p>Hipótese, implementação, validação, tuning e lições aprendidas.</p></a>
    <a class="feature-card" href="{{ '/detections/' | relative_url }}"><span class="card-label">DETECTIONS</span><h3>Catálogo de detecções</h3><p>Detecções documentadas, versionadas e relacionadas aos seus Labs.</p></a>
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
