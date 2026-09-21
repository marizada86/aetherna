---
id: "DEC-002"
type: "decision"
title: "Estrutura da campanha: 24 cantos, dois trilhos, HQs e boss canônico"
status: "approved"
created: "2026-09-21"
reviewed: "2026-09-21"
relations:
  - type: "supports"
    target: "SCOPE-001"
  - type: "supports"
    target: "VIS-001"
sources:
  - "research/iliada-eventos-por-lado.md"
  - "research/iliada-canto-a-canto.md"
  - "D:\dev\Vaults\iliada (Ilíada, trad. Frederico Lourenço)"
---

# Estrutura da campanha

## Statement

1. **24 fases, uma por canto** da Ilíada, como base (adaptável se necessário). O poema termina no funeral de Heitor.
2. O jogador escolhe **ser Grego ou Troiano** e joga a lore daquele lado. Todo canto pode ser jogado dos dois lados.
3. **Desbloqueio:** o canto N de um lado só libera ao vencer o canto N-1 **do mesmo lado**. Os trilhos grego e troiano são independentes, com progresso salvo separadamente. Qualquer canto liberado pode ser rejogado.
4. **Personagens fixos.** O jogador escolhe um personagem já existente da Ilíada, já montado. Não há criação de personagem, itens ou equipáveis nesta fase. O que acontece com o personagem segue os desfechos do poema (ex.: o buff de Diomedes no Canto 5).
5. **Espelhamento:** o personagem jogável de um lado é boss quando o jogador está do outro, usando os mesmos dados.
6. **Boss canônico:** "vencer" significa **cumprir o objetivo histórico do canto**, não sobreviver. Quando o poema decide o desfecho (ex.: mortes de Pátroclo, Sarpédon e Heitor), o combate é desenhado com uma condição de cumprimento (dano, fases, resistir N tempo) seguida de cena que mostra o fim canônico.
7. **Cantos sem combate viram HQs.** Formato provisório: 1, 2, 6, 9, 19 e 24 como HQ; 10 (furtividade), 23 (jogos fúnebres, minigames) e 18 (segmento curto misto) com formato próprio. Os demais são de combate.
7b. **HQs não têm escolha de herói:** são apenas para o jogador ler e entender a história do canto (2026-09-21).
8. **HQ e progressão:** basta **iniciar** a HQ para considerá-la concluída. Se o jogador pular, aparece a confirmação "Tem certeza de que deseja pular?", e ele pode pular e continuar sem penalidade.
9. **Cantos sem lado troiano no poema (1, 9, 19, 23):** viram HQs curtas do ponto de vista de Troia, baseadas em reação. Devem ser conteúdo original, não trechos do poema.
10. **Variação de objetivos** nos cantos 11 a 17 (defesa de posição, guerra de posições, fuga e retomada, tempo contra o incêndio das naus, escolta e disputa do corpo) para evitar repetição.
11. **Ordem de construção difere da ordem de jogo:** primeiro o sistema de HQ (Canto 1), depois o **Canto 5 (Diomedes)** como vertical slice de combate, depois o restante.
12. **Kits reutilizáveis:** um kit por personagem (Q/W/E/R), com variações por canto.
13. **Textos e HQs são escritos por nós.** A tradução de Frederico Lourenço tem copyright e não entra no repositório.

## Rationale

Personagens fixos permitem kits desenhados à mão, bosses com padrões legíveis (dificuldade estilo soulslike) e fidelidade ao poema. O "boss canônico" evita frustrar o jogador com desfechos que o texto já decidiu. Fazer HQ primeiro valida o pipeline de arte cedo.

## Consequences

- Cada personagem precisa de kit de jogador e de fase de boss, balanceados nos dois papéis.
- Modelo de dados por canto e lado: objetivo, personagem, estado (ferido, buff divino, morto) e condição de cumprimento.
- Cada canto tem dois roteiros (grego e troiano), o que dobra o trabalho de narrativa.

## Open questions

- Elenco por canto: proposta em REQ-003 (rascunho).
- Papel das deidades no jogo e intervenção divina estruturada: definir na spec da Ilíada.
- Mapeamento fino de capítulos dentro de cada canto.

## Review record

- Proposed by: Claude
- Reviewed by: Guilherme
- Approval decision: approved em 2026-09-21, com a alteração do item 8 (HQ conta ao iniciar, pular só pede confirmação).
