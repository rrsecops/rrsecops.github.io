---
layout: default
title: "Research"
permalink: /research/
---
<div class="page-header"><span class="section-kicker">RESEARCH</span><h1>Research & Field Notes</h1><p>Reflexões, experimentos e aprendizados que não cabem necessariamente em um único Lab.</p></div>
<div class="post-list">{% assign items = site.research | sort: "date" | reverse %}{% for item in items %}<article class="post-card"><div class="post-meta">{{ item.date | date: "%d/%m/%Y" }} · {{ item.type | default: "RESEARCH" }}</div><h3><a href="{{ item.url | relative_url }}">{{ item.title }}</a></h3><p>{{ item.description }}</p></article>{% else %}<div class="empty-state">Os primeiros estudos serão publicados aqui.</div>{% endfor %}</div>
