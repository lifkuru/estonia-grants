# 🇪🇪 Estonian business support register

**An open, source-linked list of grants and loans for Estonian companies** — EIS, PRIA, KIK, RTK and Kultuurkapital — with the one thing official pages don't show side by side: **how fast the application windows close.**

👉 **Browse it: [lifkuru.github.io/estonia-grants](https://lifkuru.github.io/estonia-grants/)** · data: [`data/measures.csv`](data/measures.csv), [`data/windows.csv`](data/windows.csv)

| | |
|---|---|
| Measures tracked | **77** (70 grants, 7 loans) |
| Open right now | **47** · upcoming 10 · closed 18 |
| By administrator | EIS 44 · PRIA 14 · KIK 13 · RTK 5 · Kultuurkapital 1 |
| First-come-first-served (`jooksev`) | 33 of 53 with a known mode (62 %) |
| Last checked | 2026-09-23 |

### Why this exists
On **24 August 2026** the *Tehisaru kasutuselevõtmise toetus* (AI adoption grant, €20 000 per company) opened at 09:00. By 11:15 applications exceeded the budget; at 16:00 it closed. Of the 16 windows in [`windows.csv`](data/windows.csv) with a known duration, **4 closed within 14 days** — faster than most companies can assemble their documents. Knowing *when* a measure opens matters as much as knowing that it exists.

### Data
`data/measures.csv`

| column | meaning |
|---|---|
| `name_et` | official name (Estonian) |
| `body` | administrator: EIS, PRIA, KIK, RTK, Kultuurkapital |
| `max_grant` | maximum amount per project, € (`unknown` if not published) |
| `support_rate` | share of eligible costs covered, % |
| `mode` | `jooksev` = rolling / first come first served, `voor` = call with deadline |
| `turnover_threshold` | minimum turnover required, € (where stated) |
| `status` | open · upcoming · closed · unknown |
| `opens`, `closes` | window dates when known |
| `source_url` | official page — **always check it before applying** |
| `checked_on` | date the row was last verified |
| `instrument` | `toetus` (grant) or `laen` (loan) |

`data/windows.csv` — history of past application windows (opened, closed, days open, budget, oversubscribed, source).

Rules we follow: every row links to an official source; `unknown` is never turned into 0; nothing is estimated.

### Contribute
Spotted a change on an official page? Open an issue or a pull request with the source link.

### Disclaimer
Informational only — not legal or financial advice. Conditions change; the administrator's page is the source of truth.

---

**Kokkuvõte (ET):** avatud register Eesti ettevõtete toetustest ja laenudest (EIS, PRIA, KIK, RTK, Kultuurkapital), iga rida viitab ametlikule allikale. Näitab ka, kui kiiresti taotlusvoorud sulguvad.

**Кратко (RU):** открытый реестр мер поддержки для эстонских компаний (EIS, PRIA, KIK, RTK, Kultuurkapital) со ссылками на официальные источники и историей того, как быстро закрываются окна подачи.

---

Maintained by **[lifkuru](https://lifkuru.com)** — AI that actually works for SMEs in Estonia and the Baltics. Need help preparing an application or automating the paperwork? info@lifkuru.com

Data: CC BY 4.0 · Code: MIT
