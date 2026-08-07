---
schema: memory/v1
id: 01KZF1RQKNM3YH6Z4RA929FHJR
type: decision
title: Решение по шардированию заказов
author:
  slug: ilia-trusov-c8a60c33
  name: Ilia Trusov
  role: backend-engineer
source:
  kind: agent_chat
  agent: mcp
created_at: '2026-08-07T21:23:48Z'
valid_from: '2026-08-07T21:23:48Z'
valid_to: '2026-08-07T21:24:55Z'
supersedes: []
status: superseded
visibility: team
index: true
tags:
- sharding
scope: brief
---

## Контекст
Таблица orders выросла до 400 ГБ.

## Решение
Шардируем orders по customer_id, 16 шардов.

## Обоснование
Почти все запросы идут по клиенту.
