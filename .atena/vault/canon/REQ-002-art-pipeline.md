---
id: "REQ-002"
type: "requirement"
title: "Pipeline de arte: conceito (ChatGPT) e 3D (Tripo Studio)"
status: "approved"
created: "2026-09-21"
reviewed: "2026-09-21"
relations:
  - type: "supports"
    target: "SCOPE-001"
  - type: "supports"
    target: "DEC-001"
sources: []
---

# Pipeline de arte

## Statement (proposto)

Cada asset percorre: **ficha (dados) → prompt de conceito (ChatGPT) → imagem aprovada → prompt 3D (Tripo) → glTF → importação no Godot → validação**. Claude escreve fichas e prompts; o dono executa nas ferramentas externas e devolve os arquivos.

### Estrutura de pastas (no projeto)

```text
art/
  style-bible.md          # regras visuais únicas, colada no início de todo prompt
  manifest/               # 1 arquivo YAML por asset (ficha)
  prompts/concept/        # prompt gerado por asset (ChatGPT)
  prompts/3d/             # prompt gerado por asset (Tripo)
  concept/                # imagens aprovadas (entrada do Tripo)
  source/                 # glTF/GLB baixados do Tripo (originais)
assets/                   # resultado importado no Godot
```

### Ficha de asset (manifest)

```yaml
id: char-achilles
category: character | enemy-boss | prop | building | weapon | environment-kit | vfx
name: Aquiles
source_refs: ["Ilíada, Canto XVI-XXII"]   # base histórica/literária obrigatória
era_notes: "armadura de bronze, período micênico/Idade do Bronze tardia"
silhouette: "..."
palette: ["bronze", "vermelho-púrpura", "..."]
gameplay: {scale_m: 1.9, needs_rig: true, animations: [idle, walk, attack, hit, death]}
concept_status: pending | approved
model_status: pending | approved
```

### Prompt de conceito (ChatGPT) — template

1. **Bloco fixo:** conteúdo do style-bible (pintura digital, estilo *No Rest for the Wicked*, luz dramática, câmera top-down 3/4).
2. **Bloco do asset:** ficha traduzida em descrição visual + fundamento histórico (armaduras, cerâmica, arquitetura do Bronze Tardio).
3. **Formato de saída (para servir ao Tripo):** um único objeto, fundo neutro liso, **vista frontal e 3/4 em pose neutra** (personagens em **A-pose/T-pose**), sem sombra projetada, sem texto, sem cenário.
4. **Regras negativas:** sem elementos anacrônicos (ferro tardio, armaduras medievais, armas de época errada).

### Prompt 3D (Tripo) — template

- Entrada: imagem aprovada (image-to-3D) + descrição curta em texto.
- Parâmetros a registrar por asset: modo (modelo/rig), poly budget, PBR, A-pose, pontos de retopologia.
- Personagens: gerar com rig automático do Tripo e testar animações básicas; bosses, revisão manual mais rigorosa.

### Convenções Godot

- Escala em metros, origem nos pés (personagens) ou base (props), eixo Y para cima, GLB.
- Nomes: `char_*`, `boss_*`, `prop_*`, `bld_*`, `wpn_*`.
- Um script de importação aplica escala, materiais e colisão a partir do manifest.
- Validação automática: presença de arquivo, bounding box, contagem de triângulos, rig e animações exigidas.

## Consequences

- Uma imagem por asset é o contrato entre ChatGPT e Tripo: sem imagem aprovada, não há 3D.
- O style-bible vira fonte única de coerência visual e precisa ser aprovado antes dos prompts em massa.
- Termos e licença do Tripo/ChatGPT para uso comercial e open source precisam ser verificados (CON-001).

## Decisões do dono (2026-09-21)

- **Fase 1: apenas imagens de personagens** (ChatGPT). O 3D (Tripo) vem depois, e o formato da entrada 3D será estruturado só então.
- **Uma imagem por asset** por enquanto.
- Método: pesquisar o visual de cada personagem principal (texto da Ilíada + arqueologia/iconografia do Bronze Tardio) e criar a **nossa versão**, um por um.
- As fichas de personagem do vault da Ilíada têm seção "Referências Visuais", ponto de partida da pesquisa.

## Open questions

- Rig no Tripo ou outra ferramenta: decidir na fase 3D.
- Limites de polígonos: decidir na fase 3D.

## Review record

- Proposed by: Claude
- Reviewed by: Guilherme
- Approval decision: approved em 2026-09-21
