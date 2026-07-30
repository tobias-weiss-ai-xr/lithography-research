# Lithography Research — Detailed Facts

## Sources

All articles by Mark Mantel, heise.de:
- [New rumor round about Chinese lithography systems (2026-07-28)](https://www.heise.de/en/news/New-rumor-round-about-Chinese-lithography-systems-11380980.html)
- [Report: China is said to have a functioning EUV lithography system (2025-12-20)](https://www.heise.de/en/news/Report-China-is-said-to-have-a-functioning-EUV-lithography-system-11121936.html)
- [Lithography systems: Chinese physicists demand their own ASML (2026-03-06)](https://www.heise.de/en/news/Lithography-systems-Chinese-physicists-demand-their-own-ASML-11202833.html)
- [China further improves its 7-nanometer technology (2025-12-12)](https://www.heise.de/en/news/China-further-improves-its-7-nanometer-technology-11114194.html)
- [ASML to build significantly more lithography systems (2026-07-15)](https://www.heise.de/en/news/ASML-to-build-significantly-more-lithography-systems-11366229.html)
- [EUV Lithography: ASML will shoot tin droplets 300,000 times per second (2026-02-24)](https://www.heise.de/en/news/EUV-Lithography-ASML-will-shoot-tin-droplets-300-000-times-per-second-11187649.html)
- [Chip Research: Europe's Imec Gets High-NA EUV System (2026-02-09)](https://www.heise.de/en/news/Chip-Research-Europe-s-Imec-Gets-High-NA-EUV-System-11170367.html)
- [ASML Record Revenue and Profit in 2025 (2026-01-28)](https://www.heise.de/en/news/ASML-Record-Revenue-and-Profit-in-2025-AI-Fuels-Demand-11157655.html)
- [Export ban — ASML may only sell old lithography systems to China (2023-06-30)](https://www.heise.de/en/news/Export-ban-ASML-may-only-sell-old-lithography-systems-to-China-9204299.html)

## 1. Breaking News: Aishengna DUV Immersion (2026-07-28)

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

## 9. ASML 1000W EUV Milestone (Feb 2026)

**Source:** ASML/Reuters — heise.de "ASML will shoot tin droplets 300,000 times per second"

### The Technology
- Pre-series system boosts EUV source power: **600W → 1000W**
- Tin droplets: **50,000/sec → 100,000/sec**
- Laser pulses: **100,000/sec → 300,000/sec** (3 shots per droplet: 2 pre-form + 1 heat)
- Laser/amplifiers reach up to **40kW** (but can't emit 13.5nm directly)
- Tested in 2025 at ASML research facility in San Diego, California

### Target
- **330 wafers/hour** by 2030 (+50% vs NXE:3800E today)
- Clear path to **1500W**, no fundamental barrier to **2000W**
- Upgradable in existing Low-NA systems (module swap)
- Principle transferable to High-NA EUV (identical light source, different orientation)

### Challenges
- Tin splatter contamination (historically delayed EUV by years)
- Modular chamber design for cleaning
- Scanner must withstand higher power, move masks faster
- Not yet commercial: "research milestone" per ASML spokesperson

### Supply Chain
- **Trumpf** (Germany): lasers and amplifiers
- **Zeiss SMT** (Germany): multi-layer Mo/Si mirrors (11-13 per EUV system)
- Only a fraction of 1000W reaches wafer — optics absorb most

## 10. High-NA EUV — The Next Generation

### Specifications
| Parameter | Low-NA EUV (NXE:3800E) | High-NA EUV (EXE:5200B) |
|-----------|----------------------|----------------------|
| Numerical aperture | 0.33 | 0.55 |
| Critical dimension | ~13nm | ~8nm |
| Transistor shrink | baseline | ~1.7x |
| Density gain | baseline | ~2.9x |
| Cost | €170-200M | ~€350M |
| Fab requirement | standard | taller ceilings needed |

### Timeline
- Imec (Belgium) gets first European system: **March 2026** (NanoIC pilot line)
- Intel: **14A process in 2027** (already testing systems)
- TSMC: later, preferring multi-patterning on Low-NA for now
- ASML: both types share identical light sources

### European Research (Imec)
- NanoIC pilot line: €350M, funded by Belgium + EU (Digital Europe, Horizon Europe)
- Partners: Fraunhofer (DE), CEA-Leti (FR), VTT (FI), CSSNT (RO), Tyndall (IE)
- **A14 PDK** already available for virtual chip design (Cadence/Synopsys compatible)
- eDRAM PDK: embedded DRAM in logic chips — bridges SRAM speed with DRAM density
- Europe has no leading-edge chip manufacturing but maintains research leadership

## 11. ASML Financials 2025 — Record Year Driven by AI

### Annual Results (2025)
| Metric | 2025 | vs 2024 |
|--------|------|---------|
| Revenue | **€32.7B** | +16% |
| Net profit | **€9.6B** | +27% |
| R&D spending | **€4.7B** | +9% |
| Systems sold | 300 new + 27 refurbished | fewer units but more complex (EUV/High-NA) |
| Installed base revenue | **€8.2B** (25% of total) | upgrades + maintenance |

### Record Bookings (Q4 2025)
- **€13.2B** quarterly bookings — 2.4x previous quarter, surpassing COVID-era records
- Memory manufacturers booked **€7.4B** (unusually surpassed logic)
- Total backlog: **€38.8B** (40% from memory)

### Q1 2026 Guidance
- Revenue: €8.2-8.9B (slight dip seasonal)
- Full year 2026: **€34-39B** (raised later to €43-45B by July)
- Dividend: €7.50/share (+17%), share buyback up to €12B through 2028
- Job cuts: ~1,700 of 44,000+ (mainly management, to streamline)

### AI-Driven Demand
- CEO Fouquet: "sustainability of long-term AI demand" confirmed
- HBM (High-Bandwidth Memory) for AI accelerators driving DRAM orders
- Tight supply expected through 2026 and beyond
- Memory crisis recovery complete: SK Hynix, Samsung, Micron investing heavily

## 12. Memory Manufacturers and EUV

### DRAM Evolution
- 6th generation of 10nm-class DRAM now using EUV
- More chip layers exposed with EUV each generation
- EUV adoption in memory started later than logic but accelerating fast

### HBM (High-Bandwidth Memory)
- Key enabler for AI accelerators (NVIDIA, AMD, etc.)
- Combines multiple DRAM dies with through-silicon vias (TSV)
- Requires advanced lithography for both DRAM and interconnects
- ASML: "very strong demand for HBM ... most probably lead to very tight supply"

### Market Dynamics
- Memory overtook logic in ASML bookings in Q4 2025 (€7.4B vs ~€5.8B)
- Historically cyclical but AI demand considered structural
- Chinese memory makers (YMTC, CXMT) excluded from EUV tools
- Gap widening: Samsung/SK Hynix/Micron with EUV vs Chinese fabs on DUV
