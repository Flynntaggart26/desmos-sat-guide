# Desmos for SAT — Graph Your Way to 750+ Math

> The missing manual for the Desmos calculator built into Bluebook Digital SAT Math. 30+ copy-paste inputs, 10 worked SAT examples, 15 speed drills, and a 1-page cheatsheet. From zero to faster-than-algebra in 7 days.

<p>
  <a href="https://github.com/Flynntaggart26/desmos-sat-guide"><img src="https://img.shields.io/github/stars/Flynntaggart26/desmos-sat-guide?style=social" alt="stars" /></a>
  <img src="https://img.shields.io/badge/Desmos-Bluebook_Test_Mode-blue" alt="desmos" />
  <img src="https://img.shields.io/badge/SAT-Digital_Math-green" alt="sat math" />
  <img src="https://img.shields.io/badge/Level-Beginner_to_800-orange" alt="level" />
  <img src="https://img.shields.io/github/last-commit/Flynntaggart26/desmos-sat-guide" alt="last commit" />
  <img src="https://img.shields.io/badge/License-MIT-lightgrey" alt="license" />
  <img src="https://img.shields.io/badge/PRs-welcome-brightgreen" alt="prs" />
</p>

**Why Desmos?** 30% of Digital SAT Math is faster graphed than solved. Systems, quadratics, exponents, stats — 20 seconds vs 2 minutes. This repo shows exact inputs to type, when NOT to graph, and how to practice in 10 min/day.

Part of the SAT system: [`sat-study-tutor`](https://github.com/Flynntaggart26/sat-study-tutor) — full study plans + sources. Use this repo for the calculator skill alone.

---

## Table of Contents

- [Start in 5 Minutes](#-start-in-5-minutes)
- [What You Get](#-what-you-get)
- [Top 10 Inputs TL;DR](#-top-10-inputs-tldr)
- [When to Graph vs Algebra](#-when-to-graph-vs-algebra)
- [Repository Structure](#-repository-structure)
- [7-Day Speed Plan](#-7-day-speed-plan)
- [Worked Examples](#-worked-examples)
- [FAQ](#-faq)
- [Contributing](#-contributing)
- [License](#-license)

---

## 🚀 Start in 5 Minutes

1. Open [desmos.com/calculator](https://www.desmos.com/calculator) (practice) — Bluebook uses same engine in test mode.
2. Type these 3 now:
   ```
   y=2x+3
   y=-x+5
   ```
   Click the intersection → that point solves the system. That's 4 SAT Qs per test.
3. Read [`cheatsheets/1-page.md`](cheatsheets/1-page.md) — print it.
4. Do Day 1 in [`practice/drills.md`](practice/drills.md) (10 min: lines + intersection).
5. Log method per Q in [`templates/desmos-log.csv`](templates/desmos-log.csv): algebra vs Desmos faster?

> Rule: if algebra >60s, graph it. If Desmos >60s (simple `2x+4=10`), do it by hand.

---

## ✨ What You Get

- **Guides:** setup + lines/systems + quadratics/functions + stats/geometry + timing strategy — [`guides/`](guides/)
- **10 worked SAT-style examples** with exact keystrokes + screenshots-described steps — [`examples/`](examples/)
- **Cheatsheets:** 1-page printable + keyboard shortcuts + test-day checklist — [`cheatsheets/`](cheatsheets/)
- **Practice:** 15 drills (10 min each) + self-test + log — [`practice/drills.md`](practice/drills.md)
- **Data:** [`data/tricks.json`](data/tricks.json) — every trick as JSON (input, use, trap)

---

## ⚡ Top 10 Inputs TL;DR

| # | Type this | Solves |
|---|-----------|--------|
| 1 | `y=mx+b` with sliders | Slope/intercept feel |
| 2 | `y1=...`, `y2=...` → click intersection | Any system |
| 3 | `y=ax^2+bx+c` | Roots = x-intercepts, vertex = max/min |
| 4 | Table (`+` → Table) + enter x choices | Test A-D without algebra |
| 5 | `y1=LHS`, `y2=RHS` overlap check | Equivalent expressions |
| 6 | `y>mx+b` shade | Inequalities, verify with (0,0) |
| 7 | `(x-h)^2+(y-k)^2=r^2` | Circle center/radius check |
| 8 | `mean([...])`, `median([...])` | Stats verify |
| 9 | `y=a*b^x` slider | Exponential growth vs quadratic |
| 10 | `LHS-RHS` → zeros | Any equation's solutions |

Full 30 with traps: [`cheatsheets/1-page.md`](cheatsheets/1-page.md).

---

## ⚖️ When to Graph vs Algebra

| Graph (Desmos faster) | Algebra (hand faster) |
|-----------------------|----------------------|
| Systems (2 lines/quadratic-line) | One-step linear `2x+4=10` |
| Quadratics: roots/vertex | Simple factoring `x²+5x+6` if instant |
| Equivalents (plug x=2 + graph check) | Exponent rules you know cold |
| Inequalities + shade verify | Stats definitions (median vs mean) |
| Circle center/radius verify | Percent of a number |

Test: redo 5 old misses both ways, time each. Keep faster method in log.

---

## 🗂️ Repository Structure

```text
desmos-sat-guide/
├── guides/
│   ├── getting-started.md      # Bluebook vs web, test mode
│   ├── algebra-systems.md      # lines, intersection, sliders
│   ├── quadratics-functions.md # vertex, roots, transforms
│   ├── stats-geometry.md       # tables, mean/median, circles
│   └── timing-strategy.md      # 60-sec rule, flagging
├── examples/
│   ├── 01-system.md
│   ├── 02-quadratic-roots.md
│   ├── 03-vertex.md
│   ├── 04-equivalent.md
│   ├── 05-exponent.md
│   ├── 06-inequality.md
│   ├── 07-circle.md
│   ├── 08-stats.md
│   ├── 09-table-test.md
│   └── 10-mixed.md
├── cheatsheets/
│   ├── 1-page.md               # print this
│   └── shortcuts.md
├── practice/
│   └── drills.md               # 15 x 10-min drills + self-test
├── templates/
│   └── desmos-log.csv
├── data/tricks.json
├── CONTRIBUTING.md
└── LICENSE
```

---

## 📅 7-Day Speed Plan (10 min/day)

| Day | Drill (in `practice/drills.md`) | Win |
|-----|---------------------------------|-----|
| 1 | Lines + sliders | Graph any line in 15s |
| 2 | Systems intersection | Solve 2x2 in 20s |
| 3 | Quadratics roots/vertex | Read answers off graph |
| 4 | Tables + plug choices | Test A-D without solving |
| 5 | Inequalities + circles | Shade + center/radius |
| 6 | Mixed 10Q timed | Know graph-vs-hand per Q |
| 7 | Self-test + log review | ≤30s avg on graphable Qs |

---

## 📚 Worked Examples

Each file = SAT-style Q + exact inputs + what to click + trap. Start: [`examples/01-system.md`](examples/01-system.md) → [`examples/02-quadratic-roots.md`](examples/02-quadratic-roots.md) → [`examples/10-mixed.md`](examples/10-mixed.md).

---

## 🙋 FAQ

**Is Bluebook Desmos same as web?** Same engine, fewer features (no internet, test settings). Practice at desmos.com/calculator, then verify in Bluebook preview.

**Can I use my own calculator?** Yes, but Desmos is faster for graphs. Bring backup, practice Desmos-first.

**Desmos for RW?** No — Math only. RW is logic/grammar.

**How long to fluency?** 7 days x 10 min for basics, 3 weeks to automatic. Log every Q or you’ll revert to slow algebra under pressure.

**What if graphing gives weird zoom?** Settings → square grid, zoom `+`/`-`. Always verify with table/plug-back.

---

## 🤲 Contributing

See [`CONTRIBUTING.md`](CONTRIBUTING.md). New trick needs: title, exact input, SAT use case, when slower than hand, 1 example. Small PRs merge fastest.

---

## 📄 License

MIT — see [LICENSE](LICENSE). Desmos belongs to Desmos/College Board. Original tutorials + inputs only.

---

⭐ Star this + [`sat-study-tutor`](https://github.com/Flynntaggart26/sat-study-tutor) (full plans) if it saved you time.
