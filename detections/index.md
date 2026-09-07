---
layout: default
title: "Detection Catalog"
permalink: /detections/
---
<div class="page-header"><span class="section-kicker">KNOWLEDGE BASE</span><h1>Detection Catalog</h1><p>Um catálogo versionado das hipóteses de detecção exploradas pelo projeto.</p></div>
<div class="catalog-note">Status não significa garantia de funcionamento em qualquer ambiente. Cada detecção deve ser validada e ajustada ao contexto operacional.</div>
<div class="cards cards-2">{% assign detections = site.detections | sort: "detection_id" %}{% for detection in detections %}<a class="feature-card" href="{{ detection.url | relative_url }}"><span class="card-label">{{ detection.detection_id }} · {{ detection.status }}</span><h3>{{ detection.title }}</h3><p>{{ detection.description }}</p></a>{% else %}<div class="empty-state">Nenhuma detecção publicada ainda.</div>{% endfor %}</div>
