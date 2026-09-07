---
title: "Brute Force Detection"
lab_id: "LAB-001"
description: "Transformando comportamento de autenticação em uma hipótese de detecção."
status: "PLANNED"
difficulty: "Intermediate"
fortianalyzer_version: "7.4.1"
mitre:
  - "T1110"
---
> **Status: PLANNED** — placeholder editorial. A implementação detalhada será publicada após validação.

## Cenário
Um ambiente apresenta múltiplas falhas de autenticação provenientes de uma mesma origem em uma janela temporal curta.

## Pergunta de segurança
> Esse comportamento é apenas ruído ou existe evidência suficiente para tratá-lo como uma hipótese de brute force?

## Hipótese
Uma concentração de falhas de autenticação associada à mesma origem dentro de uma janela definida pode indicar comportamento compatível com tentativa de brute force.

## Detection Logic
A lógica final deverá ser construída e testada no laboratório antes de qualquer recomendação operacional.

## Validação
O teste deverá considerar cenário de disparo, comportamento normal, múltiplas origens, usuários legítimos e variações de janela temporal.

## False Positives
Documentar os casos observados durante os testes e as decisões de tuning.

## Relação com a Detection
Quando validado, este Lab deverá produzir **DET-001 — Brute Force**.
