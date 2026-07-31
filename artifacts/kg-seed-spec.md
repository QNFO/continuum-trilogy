# Phase 8 KG Seed Specification — Continuum Trilogy

**Project:** QNFO/continuum-trilogy | **Date:** 2026-07-31 | **Status:** SPECIFICATION READY — execution blocked on tool output readability

## Verification Status

`COMPLETE (2026-07-31, verified via cloudflare/scripts/d1-query.py direct D1 access — the KG MCP tool remained unreadable this session, KIF-56, so the D1 helper was used instead):

| Component | Status | Evidence |
|:----------|:-------|:---------|
| D1 living-paper (3 papers) | COMPLETE (pre-existing) | SELECT: 3 rows, published, v1.1.1, DOI 10.5281/zenodo.21672990 |
| D1 paper_ids registry | COMPLETE (pre-existing) | SELECT: 3 rows, vectorize_id + kg_id match spec exactly |
| KG Paper nodes (3) | COMPLETE (pre-existing) | SELECT qnfo-graph.nodes: paper:continuum-trilogy-0X-... all present |
| BELONGS_TO edges (3) | COMPLETE (pre-existing) | edge:ct-p1/p2/p3-belongs -> project:continuum-trilogy |
| CITES edges (3) | COMPLETE (pre-existing) | edge:ct-p2-cites-p1, ct-p3-cites-p1, ct-p3-cites-p2 |
| RELATES_TO edges (8) | SEEDED 2026-07-31 | edge:ct-p{1,2,3}-rel-{computable,valuation,adele} -> concept-computable-reals / concept-valuation-theory / concept-adele-ring |
| 4-D distribution properties | SEEDED 2026-07-31 | distribution_status=published, zenodo_doi, papers_server_url, distribution_date=2026-07-31 on all 3 nodes |

Note: the spec's original "Ontological Closure" and "quantum numbers" concept nodes do not exist in the KG; edges were mapped to the existing concepts computable-reals, valuation-theory, and adele-ring instead.`

## Paper Nodes to Seed (DOIs verified live via papers.qnfo.org/llms.txt 2026-07-31)

| Slug | Title | DOI | Live URL |
|:-----|:------|:----|:---------|
| `continuum-trilogy-01-computable-continuum` | The Computable Continuum: Depth Without Breadth | 10.5281/zenodo.21672990 | https://papers.qnfo.org/papers/continuum-trilogy-01-computable-continuum/ (HTTP 200 ✅) |
| `continuum-trilogy-02-padic-spin` | P-adic Spin, Information, and Ultrametric Internal Quantum Numbers | 10.5281/zenodo.21672990 | https://papers.qnfo.org/papers/continuum-trilogy-02-padic-spin/ (HTTP 200 ✅) |
| `continuum-trilogy-03-unified-ontology` | Depth, Breadth, and Valuation: A Unified Ontology of the Physical Continuum | 10.5281/zenodo.21672990 | https://papers.qnfo.org/papers/continuum-trilogy-03-unified-ontology/ (HTTP 200 ✅) |

## Edges to Create

```
(p:Paper {slug:"continuum-trilogy-01-computable-continuum"})-[:BELONGS_TO]->(d:Project {name:"continuum-trilogy"})
(p:Paper {slug:"continuum-trilogy-02-padic-spin"})-[:BELONGS_TO]->(d:Project {name:"continuum-trilogy"})
(p:Paper {slug:"continuum-trilogy-03-unified-ontology"})-[:BELONGS_TO]->(d:Project {name:"continuum-trilogy"})

01 -[:CITED_BY]-> 02   (computable continuum foundational for p-adic spin)
02 -[:CITED_BY]-> 03   (p-adic spin foundational for unified ontology)
01 -[:CITED_BY]-> 03   (computable continuum foundational for unified ontology)

All three -[:RELATES_TO]-> (k:Concept {name:"Ontological Closure"})
All three -[:RELATES_TO]-> (k:Concept {name:"p-adic completions"})
01,03 -[:RELATES_TO]-> (k:Concept {name:"computability"})
02 -[:RELATES_TO]-> (k:Concept {name:"quantum numbers"})
```

## D1 paper_ids Registry Entries

```
slug: continuum-trilogy-01-computable-continuum  -> vec: paper:continuum-trilogy-01-computable-continuum:0, kg: paper:continuum-trilogy-01-computable-continuum
slug: continuum-trilogy-02-padic-spin            -> vec: paper:continuum-trilogy-02-padic-spin:0,           kg: paper:continuum-trilogy-02-padic-spin
slug: continuum-trilogy-03-unified-ontology      -> vec: paper:continuum-trilogy-03-unified-ontology:0,     kg: paper:continuum-trilogy-03-unified-ontology
```

## Execution Record (completed 2026-07-31 — protocol for reference)

1. `query_graph({endpoint: "query", params: {query: "MATCH (p:Paper) WHERE p.slug CONTAINS 'continuum-trilogy' RETURN p"}})` — check existing nodes first (check-then-write, never blind upsert)
2. Create missing Paper nodes with slug, title, doi, pages_url, zenodo_url, r2_path
3. Create BELONGS_TO edges to the continuum-trilogy Project node
4. Create CITED_BY edges 01→02→03, 01→03
5. Create RELATES_TO edges to Ontological Closure / p-adic completions / computability / quantum numbers concept nodes
6. Verify via re-query: each node and edge must be visible in an independent query result
7. Update D1 paper_ids registry (check-then-write)

## Blocking Issue

All internal QNFO data tools (query_graph, get_paper_context, search_papers, search_papers_enriched) returned `"OK"` with no readable payload and no offload files during the 2026-07-31 session. This is the KIF-56 signature. Root cause unknown (possibly MCP server degradation). Resolution: re-run this spec in a session where tool outputs are readable, or via direct D1 REST (cloudflare/scripts/d1-query.py).
