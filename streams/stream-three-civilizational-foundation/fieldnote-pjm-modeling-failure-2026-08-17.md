# Fieldnote: PJM Capacity-Market Modeling Failure — Infrastructure Fragility Beneath the AI Buildout

**Stream:** Cross-cutting (Stream One financial-architecture / Stream Three institutional-resilience)
**Date logged:** 2026-08-17
**Source:** SemiAnalysis (Substack), "$12B of US ratepayers' money wasted on a modeling mistake and PJM wants to do it again," 2026-08-16. Collaboration with Nathan Iyer. Confidence B (single expert source; reverse-engineered model explicitly described by its authors as "at best a good approximation" due to non-public inputs).
**Filed as:** Fieldnote (candidate signal, not a scored case).

---

## Summary

PJM — the largest electricity market in the US, serving 66 million people — runs an annual capacity auction to procure enough generation for grid reliability. SemiAnalysis reverse-engineered PJM's core planning model (the Reserve Requirement Study, previously a black box) and argues the model systematically overstates the winter supply shortfall by roughly 3–4 GW, because it fails to credit two real physical facts: cold air makes gas turbines more efficient (denser air, up to 25% more output), and the gas fleet has been substantially winterized since Storm Elliott (2022). The consequence: PJM procured more capacity than needed at auctions whose prices spiked from ~$29/MW-day to $270–333/MW-day, costing ratepayers an estimated $12B across 2025–2027 — a transfer to existing generators that produced almost no new capacity (4.8 GW across four auctions costing $63.6B).

The forward risk is worse than the sunk cost. PJM is about to run an "emergency auction" (Sept 30–Oct 21, 2026) to procure 6.8 GW on 11–15 year contracts running to 2043, with **no committed counterparty** — the plants get paid for existing whether or not the forecast datacenter demand ever materializes, and if it doesn't, residential ratepayers hold the bag. On the corrected model, the true shortfall is ~3.0 GW, an amount PJM's own members had voted (>two-thirds) to cover through a voluntary subscription model — which the PJM Board then overruled.

---

## Why this matters to the collapse framework

This is the physical-infrastructure and institutional-modeling layer sitting directly underneath the AI capital web the project tracks. Three distinct collapse-relevant patterns are present in one case:

**1. Model-reality divergence as a fragility driver.** The system's authoritative internal model diverges from physical reality in a way that is known, documented, and uncorrected. PJM's own hired consultant (E3, Dec 2025), its own Independent Market Monitor (Sept 2024), and its own sensitivity analysis (May 2025) all flagged the cold-air-uplift bias. The correction was drafted, passed a task force 77%, and was then killed by the senior committee at 30.7% weighted vote. This is the *administrative-activity-vs-administrative-sovereignty* variable (v3.2, Late-Ottoman anchor) appearing in a contemporary technical institution: PJM continues to legislate, auction, model, and reform — while having lost the capacity to align its own model with facts its own studies acknowledge.

**2. Vetocracy / governance deadlock as terminal-institution signature.** SemiAnalysis describes PJM's governance as "a vetocracy of vested interests" — rule changes need two-thirds across five equally-weighted sectors, so any two sectors veto anything. Generation owners block winter-rating corrections because a higher winter rating raises the benchmark they are penalized against. This is a textbook *stability-theater / frozen-center* configuration: the institution's decision procedure structurally cannot act against the interests of its incumbents even when its own analysis, its regulator (FERC), and its members' majority all point one way. FERC has now given PJM until end of September to reform governance or it will intervene — an external-authority ultimatum to a center that cannot self-correct.

**3. Cost socialization / counterparty-absence as a capital-web stress transmission.** The emergency auction is the sharpest signal: an institution committing to 15-year liabilities (max ~$21B) on the *expectation* of demand from hypothetical datacenter loads that have not signed, cannot be compelled to pay (PJM lacks jurisdiction; requires 50 separate state cost-allocation policies that do not yet exist), and can opt out by self-supplying. Datacenter developers are already writing off PJM and going behind-the-meter. This is the same circular-exposure / no-committed-counterparty structure the project flags at the Anthropic node (cloud-backlog valuation) and the Oracle node (concentrated RPO) — here expressed in the physical power layer.

---

## Cross-stream links

- **Stream One (capital web):** Directly underlies the capex-and-power theme in the Pichai (Intersect / energy vertical integration), Nadella ($190B capex), and Huang (NVIDIA power-securing / PORTS-Pike / SB Energy) dossiers. The AI buildout's power demand is the load-growth PJM is failing to price coherently; the labs' move to behind-the-meter and self-supply is partly a *flight from* this dysfunctional market. Worth cross-referencing in any future energy-layer analysis.
- **Stream One (Oracle parallel):** The "paid for existing, whether or not demand arrives" structure mirrors the RPO-concentration fragility already logged for Oracle.
- **Stream Three (institutional resilience module, v3.2):** Candidate contemporary anchor for *administrative activity vs. administrative sovereignty* and for *governance-deadlock / vetocracy*. Not a collapse case — PJM is not collapsing — but a clean live example of the mechanism variables the historical cases were built to isolate.

---

## Falsifiable / watch signals

- **Emergency auction outcome (results by Dec 2, 2026):** Does PJM procure the full 6.8 GW at elevated prices with no committed counterparty? If yes, the cost-socialization risk is realized and ratepayer exposure is locked to 2043. Watch.
- **FERC end-of-September governance ultimatum:** Does FERC intervene, or does PJM's center self-correct? A center that cannot reform under direct regulatory ultimatum is a stronger frozen-center signal.
- **Datacenter defection rate:** Continued flight to behind-the-meter / other markets (ERCOT, MISO) would confirm the capital web routing around the dysfunctional institution rather than repairing it — an "exit over voice" pattern worth tracking as its own dynamic.

---

## Epistemic caveats

- Single-source finding. SemiAnalysis is a credible specialist outfit and cites PJM's own documents, FERC filings, and the Independent Market Monitor throughout, but the $12B figure rests on their reverse-engineered model, which they explicitly call an approximation. Treat the magnitude as indicative, not precise.
- SemiAnalysis has a directional prior (pro-datacenter-growth, pro-market-reform) visible in the framing. The factual claims (auction prices, vote tallies, FERC deadlines, the E3 and IMM findings) are independently checkable against the cited primary documents; the interpretive frame is theirs.
- This is a fieldnote, not a scored case. It logs a live contemporary instance of the mechanism variables. It should not be promoted to a case brief without independent verification of the modeling claim.

---

*Logged 2026-08-17 from inbox scan. Candidate cross-stream signal. No repo action beyond filing this fieldnote until GitHub is stable.*
