# AI Disclosure — augmanitai-periodic

**Synthetic-content marking pursuant to EU AI Act Art. 50 (Regulation 2024/1689).**

## Tool Identification

This corpus was produced with substantial assistance from large language models:

- **large language models** — used for term generation drafts, definitional first-passes, structural-layout proposals, and neighbour-relation suggestions.
- **large language models** — used for routine reformatting, schema-validation passes, JSON-LD assembly, and layout-coordinate bulk transformations.

No other AI systems were used as primary generation tools.

## Authorship Split

Approximate contribution distribution across the 100 terms and the periodic-layout in this corpus:

- **~30% AI draft** — initial term candidates, first-pass definitions, schema scaffolding, structural-neighbour candidates, and machine-readable serialisations were produced by large language models under direct human prompting.
- **~70% human edit** — concept selection, three-axis composition validation, definitional accuracy, layout-coordinate assignment, structural-neighbour verification, ISO 704 / 1087 conformance, and final acceptance were performed by the human author.

The split is intentional and reflects the discipline of the corpus: AI proposes density, the human imposes structure.

## Trade-offs

Using AI as a drafting tool accelerates volume but introduces specific failure modes that the curation discipline absorbs:

- **Synonym drift** — LLMs propose near-duplicates; the human pass collapses these to canonical terms.
- **False precision** — generated definitions can sound rigorous while being vague; the human pass demands operational distinctions.
- **Citation hallucination** — any reference to external work is verified manually against live sources before publication.
- **Layout overfitting** — an AI will gladly place every term somewhere on the periodic grid; the human pass leaves explicit gaps where no term yet earns the position.

Human curation is primary, not ornamental. The periodic-layout in particular is a human-authored interpretation of the corpus's structural pattern — the AI proposes candidate positions, the human accepts, refuses, or relocates.

## Audit Trail

Every published file in this repository is anchored by:

- **Multi-Hash** — SHA-256, SHA-512, SHA3-256, BLAKE3 stored in `manifests/MULTI_HASH.json`.
- **OpenTimestamps** — `.ots` proofs in `manifests/` anchored across four independent calendar servers.
- **DOI** — registered via Zenodo, DataCite-immutable publication date.

The combination forms a defensive-publication chain.

## Reproducibility

The repository is self-contained. An independent party can:

1. Verify file integrity against `MANIFEST.sha256`.
2. Verify timestamp against the OpenTimestamps proof.
3. Re-derive the JSON-LD graphs from the canonical JSON dumps.
4. Re-derive `llms-full.txt` from the JSON entries.
5. Re-derive the periodic-layout visualisation from `api/periodic.json`.

No proprietary tooling is required.

## License

This disclosure and the corpus are released under **CC BY-NC-ND 4.0** — Creative Commons Attribution-NonCommercial-NoDerivatives 4.0 International.

---

*Disclosure version: 1.0. Maintainer: Andreas Ehstand (Independent Researcher). Contact: ehstand.schule@gmail.com.*
