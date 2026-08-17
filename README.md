<h1 align="center">
  <strong>Lithography Research Corpus</strong>
</h1>
<h3 align="center">Semiconductor lithography: EUV, DUV, High-NA, equipment, manufacturing nodes, export controls, and market dynamics</h3>

### 🔗 Links

- **GitHub**: https://github.com/tobias-weiss-ai-xr/lithography-research
- **License**: https://github.com/tobias-weiss-ai-xr/lithography-research/blob/main/LICENSE
- **CI**: https://github.com/tobias-weiss-ai-xr/lithography-research/actions/workflows/validate.yml
- **Robotics**: https://github.com/tobias-weiss-ai-xr/robotics-research
- **DevOps**: https://github.com/tobias-weiss-ai-xr/devops-research


> 🔬 **Lithography research corpus:** EUV, DUV immersion, High-NA, nanoimprint,
> multi-patterning, equipment makers, manufacturing nodes, export controls,
> photoresists, optics, and market dynamics — analyzed with the same pipeline as
> the other `*-research` corpus repos.

<p align="center">
  <img src="https://raw.githubusercontent.com/tobias-weiss-ai-xr/lithography-research/main/assets/visualizations/category_distribution.png" alt="Teaser" width="600" />
</p>

---

## What you get

| Capability | How |
|------------|-----|
| 📄 **Curated corpus** | `papers.yaml` is the source of truth — one structured entry per paper |
| ✅ **Auto-validation** | `scripts/validate_papers.py` checks schema, duplicates, URL normalization, LaTeX artifacts |
| 🧾 **Auto-generated README** | `scripts/generate_readme.py` renders the paper list grouped by your taxonomy |
| 📊 **Statistics & trends** | `scripts/standard_stats.py` → `statistics.json` (momentum, gaps, bursts, venues, authors) |
| 🔍 **Literature review report** | `scripts/analysis/generate_reports.py` → `docs/research/literature_review.md` + `trends.md` |
| 🧭 **Topic planning** | `tools/topic_planner.py`, `tools/trend_scanner.py`, `tools/landscape_analyzer.py`, `tools/brief_generator.py` |
| 🔎 **New paper discovery** | `scripts/fetch/fetch_new_papers.py` (arXiv), `fetch_other_sources.py` (dblp/crossref/europepmc), `fetch_openalex_bulk.py` |
| 🐙 **GitHub repos discovery** | `scripts/fetch/fetch_github_repos.py` (config-driven via `github_queries` in taxonomy.yaml) |
| 🦊 **GitLab projects discovery** | `scripts/fetch/fetch_gitlab_repos.py` (config-driven via `gitlab_queries` in taxonomy.yaml) |
| 🏠 **Codeberg repos discovery** | `scripts/fetch/fetch_codeberg_repos.py` (config-driven via `codeberg_queries` in taxonomy.yaml) |
| 🖥️ **GitHub Pages site** | `docs/index.html` — searchable, filterable paper browser |
| 📰 **Manual facts & analysis** | `FACTS.md` — curated timeline, player tracking, and synthesis |

## 🚀 Quick Start

```bash
# 1. Clone
git clone https://github.com/tobias-weiss-ai-xr/lithography-research.git
cd lithography-research

# 2. Install dependencies
pip install -r requirements.txt

# 3. Validate + generate
python3 scripts/validate_papers.py
python3 scripts/generate_readme.py
python3 scripts/standard_stats.py
python3 scripts/analysis/generate_reports.py
```

## 📖 How it works

```
config/taxonomy.yaml ──► papers.yaml ──► validate_papers.py
                          │   ▲              │
                          ▼   └── fetch_* ───┘
                   generate_readme.py ──► README.md (auto)
                          │
                          ▼
                  standard_stats.py ──► statistics.json, docs/papers.json
                          │
                          ▼
              analysis/generate_reports.py ──► docs/research/*.md
```

- **Never edit README.md directly** — it is generated from `papers.yaml`.
- The **taxonomy lives in one place** (`config/taxonomy.yaml`); every script reads it via `scripts/research_config.py`.
- **CI (validate.yml)** runs on every push/PR and weekly to discover new papers.
- **Distributed fetching** via [research-runner](https://github.com/tobias-weiss-ai-xr/research-runner) spreads API load across 5 hosts with separate public IPs.

## 🧪 Local pipeline (all in one)

```bash
# Full pipeline (validate → README → stats → reports)
python3 scripts/validate_papers.py && \
python3 scripts/generate_readme.py && \
python3 scripts/standard_stats.py && \
python3 scripts/analysis/generate_reports.py
```

## 🤖 Agentic workflow (AGENTS.md)

This repo is designed to be driven by coding agents (OpenCode, Claude Code, …):

- **Spec-style guardrails** in `AGENTS.md` — agents know the pipeline, never edit README, always re-validate.
- **One config file** to change → one re-run to verify (low context cost for agents).
- **Auto-validation** gives agents an objective pass/fail signal.
- **Weekly discovery** keeps the corpus fresh without human babysitting.

## 📊 Corpus Statistics

**651 papers** across **7 categories**.  
Sources: **arXiv** 4 (0%) · **DOI** 634 (97%) · **Other** 13 (1%).  
Full paper list: [GitHub Pages site](https://tobias-weiss-ai-xr.github.io/lithography-research).

### Top categories

| Category | Papers | Recent | |
|----------|--------|--------|-|
| technology | **288** | 0 | ████████████ |
| materials | **144** | 0 | ██████░░░░░░ |
| manufacturing | **97** | 0 | ████░░░░░░░░ |
| survey | **56** | 0 | ██░░░░░░░░░░ |
| equipment | **47** | 0 | █░░░░░░░░░░░ |
| geopolitics | **18** | 0 | ░░░░░░░░░░░░ |
| market | **1** | 0 | ░░░░░░░░░░░░ |


### By year

| Year | Papers | |
|------|--------|-|
| 2024 | 218 | ██████████░░ |
| 2025 | 242 | ████████████ |
| 2026 | 115 | █████░░░░░░░ |


### Momentum (hottest categories)

| Category | Total | Rate | Recent | Score |
|----------|-------|------|--------|-------|
| Survey | 56 | 2.1/mo | 45% | 137 |
| Equipment | 47 | 1.9/mo | 49% | 113 |
| Geopolitics | 18 | 1.2/mo | 78% | 78 |
| Materials | 144 | 4.1/mo | 34% | 32 |
| Manufacturing | 97 | 2.0/mo | 25% | -14 |


### Trending keywords

| Keyword | Papers | Burst |
|---------|--------|-------|
| self-sufficiency | 2 | 3.21 |
| export control | 15 | 2.78 |
| immersion | 11 | 1.17 |
| photoresist | 149 | 1.10 |
| multi-patterning | 6 | 1.07 |
| line edge roughness | 64 | 1.00 |
| nanoimprint | 108 | 0.98 |
| optical proximity correction | 66 | 0.97 |


### Top venues

| Venue | Papers |
|-------|--------|
| Journal of Micro/Nanopatterning Materials and Metrology | 33 |
| Zenodo (CERN European Organization for Nuclear Research) | 16 |
| Micromachines | 12 |
| Japanese Journal of Applied Physics | 11 |
| Applied Optics | 8 |
| Journal of Photopolymer Science and Technology | 8 |
| SSRN Electronic Journal | 8 |
| Advanced Functional Materials | 7 |


### Research gaps (thinnest cells)

| Cell | Papers |
|------|--------|
| `equipment/multi-patterning` | 1 |
| `equipment/duv` | 1 |
| `manufacturing/multi-patterning` | 1 |
| `materials/multi-patterning` | 1 |
| `materials/nanoimprint` | 1 |



*Generated 2026-08 by `scripts/standard_stats.py`.*


## 📖 Citation

If you use this corpus in your work, please cite:

```bibtex
@software{lithography_research,
  author = {Tobias Weiss},
  title = {Lithography Research Corpus},
  year = {2026},
  url = {https://github.com/tobias-weiss-ai-xr/lithography-research},
}
```

## 📄 License

This project is licensed under the MIT License — see [LICENSE](LICENSE) for details.
