---
layout: default
title: "Detection Labs"
permalink: /labs/
---
<div class="page-header"><span class="section-kicker">PRACTICE</span><h1>Detection Labs</h1><p>Experimentos práticos: hipótese, implementação, validação, tuning e lições aprendidas.</p></div>
<div class="cards cards-2">{% assign labs = site.labs | sort: "lab_id" %}{% for lab in labs %}<a class="feature-card" href="{{ lab.url | relative_url }}"><span class="card-label">{{ lab.lab_id }} · {{ lab.status }}</span><h3>{{ lab.title }}</h3><p>{{ lab.description }}</p></a>{% else %}<div class="empty-state">Nenhum Lab publicado ainda.</div>{% endfor %}</div>
