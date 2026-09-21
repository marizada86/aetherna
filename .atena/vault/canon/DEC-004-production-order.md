---
id: "DEC-004"
type: "decision"
title: "Ordem de produção: canto a canto, roteiro antes da arte"
status: "approved"
created: "2026-09-21"
reviewed: "2026-09-21"
relations:
  - type: "supports"
    target: "DEC-002"
  - type: "supports"
    target: "REQ-002"
sources: []
---

# Ordem de produção

## Statement (proposto)

A produção avança **um canto por vez**, em duas etapas:
1. **Roteiro** do canto (batalha ou HQ), nos dois lados.
2. **Imagens dos personagens** envolvidos naquele canto (fichas e prompts do REQ-002), somente depois do roteiro.

O canto seguinte só começa quando o anterior tiver roteiro e imagens concluídos. Cada canto é uma spec do ADD.

## Consequences

- Ficha de personagem é criada na primeira vez em que ele aparece; nos cantos seguintes só são acrescentadas variações (ferido, armado, etc.).
- O roteiro é texto próprio e usa o vault como referência externa (sem citar a tradução).
- Ordem do vertical slice em DEC-002 (item 11) permanece: sistema de HQ, depois Canto 5.

## Decisões adicionais (2026-09-21)

- Roteiros ficam em `story/canto-NN/` no projeto do jogo.
- Idioma inicial: **português do Brasil**; versão em inglês depois (texto em arquivos de tradução, sem texto fixo no código).

## Open questions

- Formato do roteiro de batalha: fases, objetivo, boss, deidades envolvidas, conquistas.
- Formato do roteiro de HQ: painéis, texto, personagens por painel.

## Review record

- Proposed by: Claude
- Reviewed by: Guilherme
- Approval decision: approved em 2026-09-21, conforme recomendações
