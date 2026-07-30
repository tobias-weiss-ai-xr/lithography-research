# Lithography Research — Detailed Facts

## 1. Breaking News: Aishengna DUV Immersion (2026-07-28)

**Sources:** The Information → Reuters → heise.de (Mark Mantel)

- **Shanghai Aishengna Electronic Technology Group** (state-owned, founded Aug 2023)
- Linked to **Yuliangsheng** (same address) — DUV immersion prototype rumors since 2025
- Claims: 5 DUV immersion systems in 2026, 20 in 2027
- ASML stock dropped 12% on the news
- Potential customers: SMIC, Huawei, Hua Hong, CXMT
- But: even 20 systems is a fraction of ASML's ~169 DUV/yr planned for 2027
- Known unknowns: resolution, throughput (wafers/hr), overlay accuracy, yield

## 2. Chinese EUV Prototype (Reuters, Dec 2025)

**Source:** heise.de — "Report: China is said to have a functioning EUV lithography system"

### What exists

- First functioning EUV prototype completed **early 2025**
- Built from **reverse-engineered ASML parts** (both DUV and EUV systems)
- **Cannot produce functioning chips yet**

### Huawei's Role

- Core of China's semiconductor efforts: design → equipment → production → integration
- Poaching ASML engineers since **at least 2020**, targeting Chinese employees
- Team of ex-ASML staff working under **false names**
- Key hire: **Lin Nan** — formerly head of light source technology at ASML
- ~100 university graduates constantly disassembling/reassembling ASML components

### Key Bottlenecks

1. **Zeiss mirrors:** ASML's only EUV mirror supplier is Zeiss SMT (Germany). Mirror surface tolerance: imagine Earth's surface — largest deviation = a toy car. Chinese suppliers cannot match this.
2. **Prototype is crude:** much larger footprint than ASML EUV
3. **No chip production capability yet**

### Timeline Perspective

| Milestone | ASML | China |
|-----------|------|-------|
| First prototype | 2001 | early 2025 |
| Research installation | 2006 | ? |
| First commercial use | 2018 (Samsung 7LPP, TSMC N7+) | target 2028 (unrealistic per participants) |
| Gap: prototype → commercial | ~17 years | ? |

ASML nearly ran out of money during EUV development. Even with poached engineers, China faces years of work.

## 3. Chinese Self-Assessment (Mar 2026)

**Source:** *Chinese Science & Technology Review* — heise.de "Chinese physicists demand their own ASML"

### Authors

- **Wang Yangyuan** — SMIC co-founder, now Peking University professor (lead author)
- **Chen Nanxiang** — YMTC (largest Chinese flash memory) CEO
- **Zhao Jinrong** — Naura Technology (semiconductor equipment) CEO
- **Liu Weiping** — Empyrean Technology (EDA tools) CEO

### Key Findings

| Statement | Implication |
|-----------|-------------|
| Industry "small, scattered and weak" | Too fragmented, not targeting resources |
| "Shed illusions" | No quick catch-up expected |
| 28nm consolidate (2026-2030) | This is the current baseline |
| 14nm stable production | Still working on yield — question marks for years |
| 7nm fully Chinese trial operation | Target for 2030 — TSMC will be at A14 ("1.4nm") by then |
| EUV components exist but integration fails | Having parts ≠ having a working system |

### Recommended Actions

1. **Consolidation** — merge semiconductor companies to reduce fragmentation
2. **"Team fight"** instead of "everyone fighting for themselves"
3. Better integrated **EDA tools**
4. New public platform with modern process technology
5. Incentives for fault tolerance, testing, verification along value chain

## 4. SMIC Process Evolution

### N+1 (2022?)
- First iteration of SMIC's advanced node
- Limited production

### N+2 (Kirin 9000S, 2023)
- 7nm class, using ASML DUV + multi-patterning
- Heavily based on TSMC N7 (copy)
- Surprised the world when it appeared in Huawei Mate 60 Pro

### N+3 (Kirin 9030/9030 Pro, Dec 2025)
- Improved 7nm class
- TechInsights: "significantly worse scaling than TSMC/Samsung 5nm"
- Comparable to **TSMC N7 (2018)**
- Requires up to **4x multi-patterning** — highest yet
- Each additional exposure pass reduces yield and increases cost
- Only viable through state subsidies

### Performance Comparison

| Metric | Kirin 9030 Pro | Apple A19 Pro | Snapdragon 8 Elite |
|--------|---------------|--------------|-------------------|
| Geekbench 6 Single | 1131 | ~4000 | ~3200 |
| Geekbench 6 Multi | 4277 | ~10000 | ~10000 |
| Max clock | ~2.8 GHz | >4.0 GHz | >4.0 GHz |
| Node | SMIC N+3 (7nm) | TSMC N3P (3nm) | TSMC N3E (3nm) |

## 5. ASML — the Benchmark

### Current Production (mid-2026)

| System Type | 2025 Actual | 2026 Plan | 2027 Target | Unit Cost |
|-------------|------------|-----------|-------------|-----------|
| EUV (Low-NA) | ~60 | ~65 | ~85 (+30%) | €170-200M |
| EUV High-NA | few | ramp | ramp | ~€350M |
| DUV immersion | ~120 | ~130 | ~169 (+30%) | ~€60M |
| DUV dry | existing | continued | continued | lower |

### Financials (Q2 2026)

- Revenue: >€9.3B
- Net profit: ~€2.9B (+6% QoQ)
- R&D: ~€1.3B (record)
- 2026 forecast: €43-45B (from earlier €36-40B)
- 2025 actual: €32.7B

### Overlay Accuracy

| ASML Model | Overlay | Available to China? |
|------------|---------|---------------------|
| NXT:2150i | <1.0 nm (atomic scale) | No (banned since 2023) |
| NXT:2100i | ~1.0 nm | No |
| NXT:2050i | ~1.2 nm | No |
| NXT:2000i | ~1.4 nm | No |
| NXT:1980Di | ~1.6 nm | Yes — older gen allowed |

Atomic-scale overlay is critical for multi-patterning. Each additional patterning step compounds alignment errors.

### Supply Chain Dependency

- **Zeiss SMT** (Germany) — sole supplier of EUV mirrors and complex optics
- **Trumpf** (Germany) — EUV laser source (CO₂ laser, tin droplet system)
- 5000+ suppliers total, 100,000+ parts per EUV system
- Scaling requires these partners to scale too

## 6. Chinese Domestic Equipment Ecosystem

| Company | Specialty | Status |
|---------|-----------|--------|
| **SMEE** (Shanghai Micro) | DUV dry lithography (90nm→28nm) | 28nm delivery since end of 2023 |
| **Aishengna** | DUV immersion lithography | Prototype → early production (2026) |
| **Yuliangsheng** | DUV immersion (linked to Aishengna) | Prototype since 2025 |
| **Naura Technology** | Etch, deposition, cleaning tools | Major domestic supplier |
| **AMEC** (Advanced Micro) | Etch & MOCVD | Some leading-edge capability |
| **Empyrean Technology** | EDA tools | CEO co-authored self-assessment |

## 7. Export Control Regime

| Date | Restriction |
|------|-------------|
| Pre-2023 | EUV exports to China completely banned |
| 2023 | Advanced DUV immersion (NXT:2000i and above) banned |
| 2024 | All DUV systems require export licenses |
| Ongoing | US/Netherlands/Japan (Chip 4) coordination |
| Effect | China cut off from newest DUV, all EUV |

Effectiveness: Export controls work well — even if China gets ASML systems, they are worthless without ASML setup and maintenance support.

## 8. Gap Analysis: China vs. World Leaders

| Metric | China (2026) | TSMC (2026) | Gap |
|--------|-------------|-------------|-----|
| Best node | 7nm (N+3) | 3nm (N3P), A16 in 2026 | 4+ generations |
| EUV capability | Prototype, can't produce chips | ~60+ EUV systems in fabs | ~15-20 years |
| DUV capability | 5 domestic systems/yr (2026) | ASML ~130 DUV/yr globally | 2+ orders of magnitude |
| Litho resolution | Unknown (domestic) | <13nm (EUV) | Unknown |
| Overlay accuracy | Unknown (domestic) | <1.0 nm (ASML NXT:2150i) | Unknown |
| Smartphone SoC perf | ~30% of flagship | 100% | Significant |

### Timeline Projections

| Node | TSMC/Samsung | China (domestic tools) |
|------|-------------|----------------------|
| 28nm | 2011 | 2023 (SMEE) |
| 14/16nm | 2014 | 2026-2030 target |
| 7nm | 2018 | 2026-2030 trial target |
| 5nm | 2020 | No date |
| 3nm | 2022-2023 | No date |
| 2nm/A14 | 2025-2028 | No date |

China's best path is multi-patterning on ASML DUV systems they already own + gradual domestic replacement. Even so, they remain 4+ generations behind and economically disadvantaged.
