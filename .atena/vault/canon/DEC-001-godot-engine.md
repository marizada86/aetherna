---
id: "DEC-001"
type: "decision"
title: "Godot 4 + GDScript como engine, com fluxo code-first"
status: "approved"
created: "2026-09-21"
reviewed: "2026-09-21"
relations:
  - type: "supports"
    target: "VIS-001"
  - type: "supports"
    target: "CON-001"
sources: []
---

# Godot 4 + GDScript como engine, com fluxo code-first

## Statement

O jogo usa **Godot 4** (GDScript). Todo o projeto é mantido em texto (cenas `.tscn`, recursos `.tres`, JSON, shaders) e escrito por IA. O editor é opcional.

Princípios:
1. Conteúdo data-driven (culturas, deidades, itens, habilidades, campanhas).
2. Cenas montadas por script; nada que dependa só de ajuste manual no editor.
3. Verificação automática: testes GUT, execução headless e capturas de tela por CLI.
4. Simulação (combate, stats, itens) separada da apresentação.
5. Assets do Tripo (glTF) importados com convenções fixas de escala, origem e materiais.

## Rationale

Licença MIT (compatível com open source), formatos em texto, CLI/headless, importação nativa de glTF, shaders para o visual pictórico.

## Consequences

- Visual estilo *No Rest for the Wicked* exige shaders/iluminação customizados (risco de arte técnica).
- Versão exata do Godot e do GUT a fixar na primeira spec (dependências seguem `allowlist-with-plan`).

## Open questions

- Versão fixada: Godot 4.7.2-stable, em D:Godot (console: Godot_v4.7.2-stable_win64_console.exe). Confirmado com --version em 2026-09-21.
- Instalar o Godot localmente é ação de instalação: exige aprovação.

## Review record

- Proposed by: Claude
- Reviewed by: Guilherme
- Approval decision: approved em 2026-09-21
