---
id: "VIS-001"
type: "vision"
title: "Aetherna: plataforma open source de mitologia jogável"
status: "approved"
created: "2026-09-21"
reviewed: "2026-09-21"
relations:
  - type: "supports"
    target: "CON-001"
sources:
  - "research/legacy-gdd (commit 87e671c)"
---

# Aetherna: plataforma open source de mitologia jogável

## Statement

Aetherna é um jogo 3D pictórico estilizado cujo **motor base é aberto à comunidade**, e cujo conteúdo é organizado em **culturas/mitologias**, **lore** e **campanhas (missões/fases/histórias)**.

- O jogo base é liberado como open source assim que estiver pronto e jogável.
- Qualquer pessoa pode criar lore baseada nas mitologias disponíveis.
- Campanhas autorais do dono do projeto são pagas; a primeira é **"A Ilíada"** (poema de Homero; só o que o poema narra).
- Por isso a primeira cultura implementada é a **grega**.
- Deidades e informações culturais têm base na história/registro humano (fontes citadas), não em invenção livre.
- O MMO sandbox hardcore original (Nômade → Cidade, economia, Hard Wipe) vira uma **campanha/fase futura**, não o jogo base.

## Rationale

Separar "plataforma aberta" de "conteúdo de campanha" permite comunidade e monetização sem pay-to-win. A cultura grega serve de vertical slice do sistema de culturas.

## Consequences

- O conteúdo deve ser data-driven, para lore da comunidade sem alterar o motor, mas a generalização só ocorre após a Ilíada.
- A Ilíada é construída primeiro; o "jogo base" será discriminado depois dela, extraindo o que for reutilizável.

## Open questions

Ver SCOPE-001.

## Review record

- Proposed by: Claude (a partir do pedido de Guilherme)
- Reviewed by: Guilherme
- Approval decision: approved em 2026-09-21
