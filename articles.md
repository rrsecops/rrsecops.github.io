---
layout: default
title: "Articles"
permalink: /articles/
---
<div class="page-header"><span class="section-kicker">ARTICLES</span><h1>Artigos</h1><p>Conceitos, análises e perspectivas de SecOps.</p></div>
<div class="post-list">{% for post in site.posts %}<article class="post-card"><div class="post-meta">{{ post.date | date: "%d/%m/%Y" }} · {{ post.category | default: "ARTICLE" }}</div><h3><a href="{{ post.url | relative_url }}">{{ post.title }}</a></h3><p>{{ post.excerpt | strip_html | truncate: 220 }}</p></article>{% else %}<div class="empty-state">Nenhum artigo publicado ainda.</div>{% endfor %}</div>
