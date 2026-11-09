# Upstage Studio — Mid-Market Developer Research

Market research for **Upstage Studio**: who buys at mid-market, how competitors price, where the gaps are, and what questions the CPO should be asking.

Research was conducted with [Nimble](https://nimbleway.com) and synthesized into a single self-contained HTML report.

## Report

Open [`docs/index.html`](docs/index.html) in any browser — no server needed, all charts embedded.

Sections: Tech Stack (Python vs JS) · Competitor Pricing (8 tools) · Pricing Gap Analysis · Buyer Reviews & Pain Points · Self-Serve Playbook · Buyer Persona · 3 Sharp Questions for the CPO

GitHub Pages: `https://devtinapark.github.io/upstage-research/`

## Structure

| Path | Contents |
|------|----------|
| `research/01-landscape/` | Competitor discovery, raw + parsed findings |
| `upstage-research/` | Nimble-generated findings, parsed CSVs, report |
| `scripts/` | Reproducible Nimble commands (01–04 + analysis) |
| `docs/index.html` | Final report (GitHub Pages) |

## Reproducing

Requires the [Nimble CLI](https://docs.nimbleway.com/) and `NIMBLE_API_KEY` in your environment.

```bash
export NIMBLE_API_KEY="your_key"
./scripts/01-landscape.sh   # → research/01-landscape/raw/
# ... repeat for 02–04
python scripts/build_report.py  # → docs/index.html
```
