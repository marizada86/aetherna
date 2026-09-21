---
id: "SCOPE-001"
type: "requirement"
title: "Escopo inicial (v0: fundação + cultura grega)"
status: "approved"
created: "2026-09-21"
reviewed: "2026-09-21"
relations:
  - type: "supports"
    target: "VIS-001"
sources: []
---

# Escopo inicial

## Statement (proposto)

**Ordem de trabalho:** primeiro construir a missão "A Ilíada" (cultura grega incluída); só depois, com ela pronta, **discriminar o que é o "jogo base"** (o que vira open source e reutilizável). Nada do núcleo é generalizado antes disso.

**Dentro do escopo v0**
1. Esqueleto técnico Godot 4 (DEC-001): câmera top-down, movimento por clique, habilidades Q/W/E e ultimate R.
2. Cultura Grega necessária à missão: panteão, personagens, locais, unidades, arquitetura, com fontes históricas/literárias.
3. Pipeline de assets Tripo Studio → Godot com convenções.
4. Estrutura de missão (cenas, gatilhos, diálogos, bosses) suficiente para a Ilíada.
5. A missão "A Ilíada", baseada **somente** no que o poema de Homero narra (cólera de Aquiles até o funeral de Heitor; a queda de Troia, a morte de Aquiles e o cavalo ficam fora). Definida em spec própria.

**Fora do escopo v0**
- Definição formal do jogo base e liberação open source (após a Ilíada).
- Demais 8 culturas, MMO/economia/Hard Wipe (fase futura), Lore Market, multiplayer.
- Licenças e mecanismo de ativação das campanhas pagas (decidir no futuro).

## Decisões do dono (2026-09-21)

- Vários modos de jogo no futuro; **escopo inicial de todos: single-player offline**.
- "A Ilíada": single-player com **dificuldade de bosses estilo soulslike** (padrões legíveis, punição, aprendizado). A estrutura do jogo NÃO é soulslike: controles e loop são de MOBA/ARPG.
- Câmera **top-down estilo MOBA**; movimento por clique; habilidades **Q/W/E**, ultimate **R**.
- **Itens (6 utilizáveis) e mochila (3 espaços): adiados.** A princípio o jogo não tem itens nem equipáveis.
- **Sem personagem criado pelo jogador.** O jogador escolhe um personagem já existente na Ilíada, já montado; o que acontece com ele segue os desfechos da própria história.
- A guerra é dividida em **arcos e capítulos**; em cada arco o jogador escolhe **jogar de grego ou de troiano**. Um mesmo personagem é jogável de um lado e **boss** do outro (ver DEC-002 rascunho).
- **Fonte:** `D:\dev\Vaults\iliada` (Ilíada, tradução de Frederico Lourenço, banco Obsidian com notas por canto e fichas de ~750 personagens).
- **Ordem de arte:** pesquisar o visual dos personagens principais e criar nossa versão, um por um, começando pelas imagens (ChatGPT); o 3D vem depois.
- Estilo visual e de jogabilidade referenciado em *No Rest for the Wicked* (pictórico, ARPG isométrico).
- Engine: **Godot 4 com GDScript** (ver DEC-001).
- Campanhas **vendidas dentro do jogo**; núcleo aberto, conteúdo das campanhas pagas fora do repositório aberto, empacotado e ativado por licença.

## Open questions

1. Licença do código e do conteúdo aberto: adiado.
2. Ativação/empacotamento das campanhas pagas: adiado.
3. Papel das deidades no jogo (ex.: R como bênção divina): a definir na spec da Ilíada.
4. Intervenção divina da Ilíada: será tratada de forma **estruturada** (regras/dados explícitos, não ad hoc). Formato a detalhar na spec da Ilíada.

## Revisões

- 2026-09-21 (errata do dono): a missão inicial passa de "A Guerra de Troia" para "A Ilíada", limitada ao que o poema narra. Ajustes em VIS-001 e SCOPE-001.

## Review record

- Proposed by: Claude
- Reviewed by: Guilherme
- Approval decision: approved em 2026-09-21
