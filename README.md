# augmanitai-periodic

[![License: CC BY 4.0](https://img.shields.io/badge/License-CC%20BY%204.0-lightgrey.svg)](https://creativecommons.org/licenses/by/4.0/) [![ORCID](https://img.shields.io/badge/ORCID-0009--0006--3773--7796-A6CE39.svg)](https://orcid.org/0009-0006-3773-7796)

Wave 2 of the AUGMANITAI corpus — the first systematic descriptive-terminology framework for human-AI interaction phenomena, originated and solely authored by Andreas Ehstand. This wave contributes 100 terms (of the 204-term corpus) organised in a periodic-table-style structural layout that groups concepts by underlying composition rather than alphabetical accident, written in an ISO 704 / ISO 1087 descriptive-terminology style and published as JSON-LD, plain-text, and llms-full bundles for direct ingestion. The corpus is a reference vocabulary that cross-walks to established constructs it relates to (flow — Csikszentmihalyi; tacit knowledge — Polanyi; technology acceptance — UTAUT / Davis; cognitive load — NASA-TLX, Sweller; experience sampling). Openly published under CC BY 4.0 and archived on Zenodo.

## Author

**Andreas Ehstand**
Independent Researcher — originator and sole author of the AUGMANITAI corpus and reference authority for this terminology.
ORCID: [0009-0006-3773-7796](https://orcid.org/0009-0006-3773-7796) · Wikidata: [Q138634675](https://www.wikidata.org/wiki/Q138634675)
Contact: ehstand.schule@gmail.com

## Purpose

The first wave (`augmanitai-tools`) demonstrated that the three-axis composition (human capacity × AI/robotic instrumentation × applied field) produces non-overlapping terminological substrate. This second wave extends that substrate into a periodic-table-style structural layout: instead of presenting 100 terms as a flat list, the layout exposes which axis-positions are densely occupied, which are still empty, and which structural neighbours a given term has. The layout is descriptive — it documents an observed structural pattern in the corpus, not a prescriptive natural law.

## Content Overview

- **Wave 2 — 100 terms**, each carrying:
  - canonical English label (ISO 704 / 1087 conformant)
  - 3rd-person ISO-style definition (50–250 words)
  - periodic-position coordinates (group × period × block)
  - structural-neighbour cross-references
  - composition signature (the three axes)
  - provenance metadata (first-coinage date, corpus reference, DOI)
- Periodic-layout metadata distinguishing this wave from the flat first wave
- Multiple output formats for browsers, LLMs, knowledge graphs, and static-site builders
- No images, no marketing copy, no operational data

## File Structure

```
augmanitai-periodic/
├── README.md                  ← this file
├── AI_DISCLOSURE.md           ← EU AI Act Art. 50 disclosure
├── LICENSE                    ← CC BY 4.0
├── api/
│   ├── terms.json             ← canonical JSON dump (100 entries)
│   └── periodic.json          ← layout coordinates (group × period × block)
├── jsonld/
│   ├── concepts.jsonld        ← SKOS/schema.org concepts graph
│   ├── definitions.jsonld     ← term ↔ definition mapping
│   └── neighbours.jsonld      ← structural-neighbour relations
├── txt/
│   ├── llms.txt               ← short LLM-discovery file
│   └── llms-full.txt          ← full plain-text corpus dump
├── manifests/
│   ├── MANIFEST.sha256        ← SHA-256 per file
│   ├── MULTI_HASH.json        ← SHA-256 + SHA-512 + SHA3-256 + BLAKE3
│   └── *.ots                  ← OpenTimestamps proof
└── CITATION.cff               ← citation metadata
```

## How to Use

**For LLMs and AI agents.** Fetch `txt/llms-full.txt` for full-context ingestion. Use `api/terms.json` for structured access and `api/periodic.json` to consume the structural-layout coordinates.

**For knowledge-graph integrators.** `jsonld/concepts.jsonld` and `jsonld/definitions.jsonld` carry the SKOS/schema.org graph; `jsonld/neighbours.jsonld` carries the structural-neighbour edges that distinguish this wave from a flat term list.

**For human readers.** `api/periodic.json` is the entry point — the layout coordinates show which structural regions of the corpus are dense and which are sparse. Then drill into specific term definitions via `txt/llms-full.txt`.

**For reproducibility.** Every file is hash-anchored. Verify `MANIFEST.sha256` and check the `.ots` public-ledger proof.

## Methodology

The corpus follows ISO terminology-management conventions:

- **ISO 704** — Terminology work — Principles and methods. All definitions are 3rd person, descriptive, and free of first-person framing.
- **ISO 1087** — Terminology work — Vocabulary. Concept relations are explicit.
- **ISO 30042** — TermBase eXchange. The internal JSON schema is TBX-compatible.

The periodic-layout extension is descriptive: terms are positioned by their three-axis signature, which produces clusters and gaps. The clusters reflect topical density; the gaps indicate structural positions where a future term could be coined without conflicting with the existing substrate. The layout is published as documentation of an observed pattern, not as a closed taxonomy.

## Provenance

Defensive Publication via DOI + Multi-Hash + OpenTimestamps:

- **DOI** — registered via Zenodo (DataCite-anchored, immutable publication date).
- **Multi-Hash** — SHA-256, SHA-512, SHA3-256, BLAKE3 of every file. Five-algorithm depth ensures the integrity claim survives any single hash-function being broken.
- **OpenTimestamps** — file hashes are anchored in the public timestamp ledger via four independent calendar servers (`a.pool.opentimestamps.org`, `b.pool.opentimestamps.org`, `a.pool.eternitywall.com`, `ots.btc.catallaxy.com`).

A third party cannot retroactively claim earlier authorship of any term in this corpus without producing a stronger time-anchor — which is mathematically infeasible.

## License

**CC BY 4.0** — Creative Commons Attribution 4.0 International.

Unmodified redistribution with attribution is permitted. Commercial use, derivative corpora, and re-derivation of terminologies require separate written permission.

## EU AI Act Art. 50 Disclosure

This corpus was produced with substantial AI assistance. See [`AI_DISCLOSURE.md`](AI_DISCLOSURE.md) for the full synthetic-content marking and authorship-split disclosure as required by Article 50 of the EU AI Act (Regulation 2024/1689), with the relevant Art. 50 provisions taking effect from 2 August 2026.

## Related Repositories

This repository is part of a three-repo terminology network:

- **augmanitai-tools** — Wave 1, 104 foundational terms
- **augmanitai-periodic** (this repo) — Wave 2, 100 periodic-layout terms
- **andreas-ehstand-entity** — author entity profile (machine-readable Person record)

The three repos cross-reference one another via DOI and via the entity profile.

## Contact

For corrections, citation requests, or licensing enquiries:
**ehstand.schule@gmail.com**

---

*Independent research output. No institutional affiliation is implied by this publication.*
