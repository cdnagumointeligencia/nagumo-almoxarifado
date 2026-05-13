# Graph Report - ControleAlmoxarifado  (2026-05-12)

## Corpus Check
- 2 files · ~35,817 words
- Verdict: corpus is large enough that graph structure adds value.

## Summary
- 16 nodes · 19 edges · 3 communities (2 shown, 1 thin omitted)
- Extraction: 100% EXTRACTED · 0% INFERRED · 0% AMBIGUOUS
- Token cost: 0 input · 0 output

## Graph Freshness
- Built from commit: `90fbb214`
- Run `git rev-parse HEAD` and compare to check if the graph is stale.
- Run `graphify update .` after code changes (no API cost).

## Community Hubs (Navigation)
- [[_COMMUNITY_Community 0|Community 0]]
- [[_COMMUNITY_Community 1|Community 1]]
- [[_COMMUNITY_Community 2|Community 2]]

## God Nodes (most connected - your core abstractions)
1. `analisar_imagem()` - 5 edges
2. `main()` - 3 edges
3. `extrair_texto()` - 3 edges
4. `analisar_cores()` - 3 edges
5. `analisar_layout()` - 3 edges
6. `analisarComOpenAI()` - 2 edges
7. `analisarComOllama()` - 2 edges
8. `__dirname` - 1 edges
9. `CONFIG` - 1 edges
10. `analisar_imagem.py — Analisa imagens de layout web e gera descrição detalhada pa` - 1 edges

## Surprising Connections (you probably didn't know these)
- `analisar_imagem()` --calls--> `analisar_layout()`  [EXTRACTED]
  analisar_imagem.py → analisar_imagem.py  _Bridges community 2 → community 0_

## Communities (3 total, 1 thin omitted)

### Community 0 - "Community 0"
Cohesion: 0.32
Nodes (7): analisar_cores(), analisar_imagem(), extrair_texto(), analisar_imagem.py — Analisa imagens de layout web e gera descrição detalhada pa, Pipeline completo de análise., Extrai textos da imagem com bounding boxes., Extrai paleta de cores dominante e regiões-chave.

### Community 1 - "Community 1"
Cohesion: 0.47
Nodes (5): analisarComOllama(), analisarComOpenAI(), CONFIG, __dirname, main()

## Knowledge Gaps
- **7 isolated node(s):** `__dirname`, `CONFIG`, `analisar_imagem.py — Analisa imagens de layout web e gera descrição detalhada pa`, `Extrai textos da imagem com bounding boxes.`, `Extrai paleta de cores dominante e regiões-chave.` (+2 more)
  These have ≤1 connection - possible missing edges or undocumented components.
- **1 thin communities (<3 nodes) omitted from report** — run `graphify query` to explore isolated nodes.

## Suggested Questions
_Questions this graph is uniquely positioned to answer:_

- **Why does `analisar_imagem()` connect `Community 0` to `Community 2`?**
  _High betweenness centrality (0.133) - this node is a cross-community bridge._
- **What connects `__dirname`, `CONFIG`, `analisar_imagem.py — Analisa imagens de layout web e gera descrição detalhada pa` to the rest of the system?**
  _7 weakly-connected nodes found - possible documentation gaps or missing edges._