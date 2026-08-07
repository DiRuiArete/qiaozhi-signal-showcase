# Qiaozhi Signal · 侨知信号

🇺🇸 **English** | [🇨🇳 中文](README.zh-CN.md)

A global signal terminal built on public data. WeChat Mini Program, live in production.

> Project showcase. Source code is in a private repository.

---

## Demo

<a href="assets/demo.mp4"><img src="assets/cover.jpg" width="260" alt="Qiaozhi Signal demo video" /></a>

▶︎ [Play the full demo](assets/demo.mp4) (2 min)

**Try it**: scan the code in WeChat

<img src="assets/qr.png" width="160" alt="Qiaozhi Signal Mini Program code" />

---

## Product

**How the world sees the future · Finding signal in the noise**

Aggregates global public event data and real-world risk, then runs it through collection → translation → classification → filtering → visualization, producing a searchable signal library. Built for people working across borders and anyone tracking global macro trends.

- **Signal globe** — a 3D earth showing worldwide signal distribution, with three independent layers and per-hazard toggles
- **Three signal types** — Consensus (market expectations) · Global Direction (governance trends) · Reality (earthquakes, wildfires, floods and other real-world risk)
- **24h movers** — signals ranked by the largest expectation shift in the past day
- **Searchable database** — filter by category, keyword, or deadline
- **Synced every 4 hours** — refreshed by a scheduled build pipeline

---

## Engineering highlights

- **Multi-source collection and filtering** — ~2,000 candidates per run pass through layered gates that strip noise, gambling-shaped markets and unsuitable content, leaving roughly 300 high-value signals
- **A definition of "signal"** — anchored on *an unexpected, observable, non-personal change in world state*; implemented as freshness half-lives, materiality thresholds, and zero-information filters
- **Translation pipeline** — batched AI translation with source-text hash caching, so only new or changed items are translated
- **3D rendering** — Three.js globe using shape and color as dual encoding for signal type, with screen-space picking to keep dense clusters individually tappable
- **Compliance gate** — static scanning at build time; non-conforming output is refused rather than published (fail-closed)

---

## Stack

WeChat Mini Program (native) · Three.js · Tencent CloudBase (cloud functions + database) · Node.js · GitHub Actions

---

## My role

Built end to end, solo:

Product definition · Signal selection criteria · Information architecture · UI design system · 3D visualization · Frontend · Data pipeline · AI integration · Content compliance strategy · Launch

---

## Disclaimer

This product is a read-only information display tool. It provides no trading functionality. All content comes from public data sources, is for reference only, and does not constitute investment advice.

---

## Contact

diruiarete@gmail.com
