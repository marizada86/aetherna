---
id: "DEC-003"
type: "decision"
title: "Progressão de personagens por Conquistas"
status: "approved"
created: "2026-09-21"
reviewed: "2026-09-21"
relations:
  - type: "supports"
    target: "DEC-002"
sources: []
---

# Progressão por Conquistas

## Statement (proposto)

1. A progressão é feita **por Conquistas**, não por itens, nível ou experiência.
2. Para melhorar um personagem, o jogador **joga com ele e cumpre suas Conquistas**; o personagem fica mais forte.
3. O personagem **nunca perde conquistas**. Ao rejogar um canto anterior com mais conquistas, ele entra **mais forte**.
4. Cada canto define suas Conquistas por herói disponível (REQ-003).

## Rationale

Combina com personagens fixos e sem equipamentos: o poder vem da maestria do jogador.

## Consequences (recomendações a validar)

- **Bosses e desfechos canônicos têm força fixa.** O boss "espelho" (ex.: Diomedes contra um jogador troiano) não herda as conquistas do jogador.
- **Bônus modestos e com teto**, para não anular a dificuldade estilo soulslike ao rejogar cantos antigos.
- **Conquistas são opcionais**: vencer o canto continua sendo a única exigência de desbloqueio (DEC-002).
- Conquistas por personagem, compartilhadas entre cantos (Diomedes do Canto 5 fica mais forte no 8).
- Formato de conquista: id, herói, canto, condição, bônus. Dado em JSON.

## Open questions

- Um mesmo herói tem tipos de bônus (dano, vida, cooldown, habilidade nova)?
- Há teto global de bônus por herói?
- Conquistas de HQ existem (ex.: ler tudo)?

## Review record

- Proposed by: Claude
- Reviewed by: Guilherme
- Approval decision: approved em 2026-09-21, conforme recomendações
