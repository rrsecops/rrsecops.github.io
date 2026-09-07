---
title: "Brute Force"
detection_id: "DET-001"
description: "Hipótese de identificação de comportamento compatível com tentativas repetitivas de autenticação."
status: "IDEA"
category: "Authentication"
fortianalyzer_version: "7.4.1"
mitre:
  - "T1110"
---
> **Status: IDEA** — esta detecção ainda não foi validada.

## Objetivo
Identificar comportamento compatível com tentativas repetitivas de autenticação.

## Hipótese
Um volume elevado de falhas de autenticação associado à mesma origem dentro de uma janela definida pode representar comportamento suspeito.

## Data Sources
A fonte exata e os campos necessários deverão ser definidos no LAB-001.

## Detection Logic
A lógica deverá ser construída e testada no laboratório antes de qualquer recomendação operacional.

## False Positives
Ainda não avaliados.

## Tuning
Ainda não definido.

## Investigation
Após um disparo, a investigação deverá buscar contexto adicional antes de qualquer decisão de resposta.

## MITRE ATT&CK
**T1110 — Brute Force**

## Related Lab
[LAB-001 — Brute Force Detection](/labs/lab-001-brute-force/)
