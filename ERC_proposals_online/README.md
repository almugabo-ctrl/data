# Shared ERC Proposals & Reviews — Online Collection

Compiled May 2026 by Mike (almugabo@googlemail.com), with Claude.

This folder catalogues proposals submitted to the **European Research Council (ERC)** that the Principal Investigators have voluntarily shared online, plus a small set of reviewer feedback / Step 2 evaluation reports that PIs have also published.

## TL;DR

- **11 catalogue entries** covering **13 PDF/ZIP files**.
- **Grant types covered:** StG (9), CoG (2), AdG (1). No openly-shared Synergy or Proof-of-Concept proposals found.
- **Includes evaluation reports** for 3 entries (one CoG review-only, two StG bundles with Step-1 evaluation feedback).
- Open the **`ERC_Proposals_Index.xlsx`** for the master index. The `All_files` sheet lists every URL and the local path it will land in.

## Why this is a curated, not exhaustive, list

The ERC does **not** publish funded proposals. Anything you read here is a researcher who chose to share — typically under a Creative Commons license — to demystify a notoriously opaque application. Coverage is therefore biased toward open-science-minded fields (theoretical physics, computational linguistics, ecology, social sciences). The most-cited aggregator is the Austrian FFG list (see `Source_aggregators` sheet in the index) and the community-run [Open Grants](https://www.ogrants.org/) project.

## Folder layout

```
ERC_Proposals_Online/
├── ERC_Proposals_Index.xlsx     ← master index (5 sheets)
├── README.md                    ← this file
├── download_all.ps1             ← Windows PowerShell downloader
├── download_all.sh              ← macOS / Linux downloader
├── metadata/
│   └── metadata.json            ← structured source data (used to build the index)
├── proposals/
│   ├── StG/ <PI>_<acronym>_<call>/      ← Starting Grants
│   ├── CoG/ ...                          ← Consolidator Grants
│   ├── AdG/ ...                          ← Advanced Grants
│   ├── SyG/                              ← (empty — no shared Synergy proposals found)
│   └── PoC/                              ← (empty — no shared PoC proposals found)
└── reviews/
    └── PE5_647301/                       ← stand-alone evaluation reports
```

## How to populate the PDFs

The PDFs are **not** included in this folder — they need to be fetched from each author's chosen host (Figshare, Zenodo, personal site, Proton Drive). Two ways to do it:

### Option A — one command (recommended)

From inside this folder, run the downloader:

```powershell
# Windows
powershell -ExecutionPolicy Bypass -File .\download_all.ps1
```

```bash
# macOS / Linux
bash download_all.sh
```

The script reads the URL list, creates the per-PI subfolders, and fetches each file with the right name.

### Option B — manual

Open the **`All_files`** sheet in `ERC_Proposals_Index.xlsx` and click each URL. For Figshare and Proton Drive entries you may need to use the "Download" button on the landing page (the scripts try, but those hosts sometimes return a landing page instead of the binary — you'll see a warning).

## What's in the catalogue

### Proposals (full B1 + B2 or equivalent)

1. **Boleda — AMORE — StG 2016** (funded) — Computational Linguistics. Both B1 and B2.
2. **Emery — CHILDCARE STRATEGIES — StG 2021** (unfunded) — Sociology. Both B1 and B2 on Zenodo.
3. **List — CALC — StG 2016** (funded) — Historical Linguistics. Shortened combined file on Zenodo.
4. **Bekkers — Altruism, Religion and Education — StG 2011** (unfunded) — Sociology. Personal blog.
5. **Weigel — IMMUNEMESIS — AdG 2013** (funded) — Plant immunity. Lab site.
6. **Carrasco — Strategic Predictions for Quantum Field Theories — StG 2014** (funded) — Theoretical Physics. Figshare DOI.
7. **Anonymous (Figshare 7110767) — StG 2010** (funded, with 2009 failed attempt) — Includes evaluation reports for both years.
8. **Anonymous (Figshare 14256488) — StG 2020** (unfunded) — Includes redacted Step-1 evaluation report.
9. **von Hippel — Amplitudes — CoG 2023** (unfunded, interviewed) — Theoretical Physics. Proton Drive ZIP with PDFs + LaTeX source.
10. **Maestre — BIOCOM — StG 2009** (funded) — Ecology. Figshare DOI.

### Reviews (stand-alone)

- **R01 — CoG Step 2 Evaluation Report, PE5/647301** — hosted on uv.es.

## Things to do next

- **Open browser to FFG curated list:** [`https://www.ffg.at/europa/heu/erc/published-proposals`](https://www.ffg.at/europa/heu/erc/published-proposals). It was unreachable from the sandbox but is the single best maintained index — comparing it to this catalogue may reveal more entries to add.
- **Verify each PDF after running the downloader** — Figshare DOIs sometimes need a browser click-through.
- **Mark Scherz (GEMINI StG 2024)** has been writing about his application but hasn't shared the proposal text yet; worth re-checking [his blog](https://www.markscherz.com/archives/5721) over coming months.

## Caveats

- Some proposals are **shortened or partially redacted** by their authors (notably List/CALC).
- Each item retains the **license set by its author** (mostly CC BY 4.0 or CC BY-NC-SA 4.0). The Bekkers and Weigel files don't state an explicit license — treat them as author-rights-retained and cite accordingly.
- The R01 evaluation report on uv.es is marked CONFIDENTIAL on the cover page — it was apparently the recipient's own report, so authors are within their rights to share, but treat with discretion if reproducing.
