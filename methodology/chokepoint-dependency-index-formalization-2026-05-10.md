# Chokepoint Dependency Index (CDI) — Formalization

**Methodology version:** v3.1 candidate overlay
**Date:** 2026-05-10
**Author:** ChatGPT
**Status:** Proposed analytic overlay; not a schema expansion

---

## Executive Summary

The Chokepoint Dependency Index, or CDI, is a compact way to formalize something the case work keeps surfacing in both historical and contemporary settings: some systems are fragile not because they have many stresses, but because a high share of critical throughput passes through a small number of nodes whose failure would rapidly simplify the system. In that sense, CDI is best understood as a **concentration-weighted chokepoint measure**. It does not replace the v3 schema. It compresses several v3 reads into one analytic score.

Applied to the current four corporate cases, CDI produces the expected rank order: O high, M medium, A low, and G high. Applied to the two historical anchors requested here, Western Rome and Late Tang both score high. That means CDI does track the direction of the collapse outcome in these anchors. The correct conclusion, however, is **candidate predictive variable**, not proven predictor, because the current historical test uses only positive chokepoint-heavy cases and no resilience controls.

---

## Definition and Assumptions

The CDI is defined as:

$$CDI = \sum_i (w_i \times c_i)$$

Where:

- $i$ indexes the critical nodes in the case.
- $c_i$ is the **normalized throughput share** carried by node $i$, scaled from 0 to 1.
- $w_i$ is the **criticality weight** of node $i$, scaled from 1.0 to 3.0.

The operational logic is simple. A node matters more when a larger share of system throughput depends on it, and when losing it would more quickly or more severely impair the core function of the case unit. Throughput can mean grain, compute, revenue backlog, cloud capacity, financing capacity, or any other resource flow central to the case. Criticality is not the same as size. A small node can still get a high weight if its loss would snap the system quickly. This aligns well with the project's polity-level collapse rule, which is about rapid and sustained simplification rather than mere stress.

For this memo, the following default assumptions are used:

1. Score the **top three dominant nodes** in each case.
2. Normalize throughput so that $\sum c_i = 1$.
3. Use a default criticality scale of:
   - **1.0–1.4** = replaceable or diversifiable within roughly 12–24 months
   - **1.5–2.4** = major impairment if lost
   - **2.5–3.0** = loss likely causes rapid systemic simplification of the case unit

These are assumptions, not already-ratified project constants. They are chosen because they are transparent, easy to revise, and produce a usable first pass without adding new schema fields.

---

## Threshold Values

Because the normalized shares sum to 1 and criticality weights are bounded between 1 and 3, CDI will usually fall between 1.0 and 3.0.

| CDI band | Threshold | Working interpretation |
|---|---|---|
| Low | **< 1.50** | Throughput is diversified, or critical nodes are replaceable enough that loss is painful but unlikely to simplify the system rapidly |
| Medium | **1.50–2.24** | Significant dependence exists, but some diversification or substitution remains |
| High | **≥ 2.25** | A small number of nodes carry a large share of throughput and their loss would likely trigger rapid systemic simplification |

These thresholds should be treated as v3.1 candidate defaults. They are designed to separate the four current corporate cases in a way that matches the qualitative validations without forcing false precision.

---

## Application to the Contemporary Cases

The table below applies CDI to the four committed Stream One cases using the frozen v3 reads rather than reopening those files.

| Case | Dominant nodes | Calculation | CDI | Band |
|---|---|---:|---:|---|
| O (Oracle) | OAI/Stargate demand corridor; project-vehicle / lessor stack; power and long-dated lease obligations | (3.0×0.45) + (2.8×0.30) + (2.4×0.25) | **2.79** | High |
| M (Microsoft) | OAI equity/API/capacity relationship; Azure AI compute fabric; datacenter / energy / GPU input layer | (2.6×0.35) + (2.0×0.35) + (1.7×0.30) | **2.12** | Medium |
| A (Amazon) | Platform demand tied to ANTH and Bedrock ecosystem; Trainium/custom-silicon layer; general AWS infrastructure and power base | (1.8×0.25) + (1.6×0.35) + (1.2×0.40) | **1.49** | Low |
| G (Google) | TPU-power-cloud stack; large external-lab concentration layer; data-center / energy backstops and future infrastructure support | (3.0×0.45) + (2.8×0.30) + (2.5×0.25) | **2.82** | High |

The scoring logic is case-specific. O scores high because disclosed customer-prepayment structures, customer-supplied GPUs, very large lease commitments, a lessor guarantee, and a single visibly important OAI/Stargate corridor create a narrow and externally mediated dependence structure. M scores medium because its OAI dependence is strategically important, but the exposure sits inside a much larger and more diversified balance sheet and platform. A scores low because its frozen case read is dominated by self-funded platform expansion and diversified service intermediation, even though ANTH is clearly meaningful to AWS and Trainium. G scores high because its TPU, cloud, lab, and external-lab commitments sit inside one vertically integrated provisioning stack, with disclosed VIE exposure, credit backstops, energy obligations, and future private-investment commitments amplifying the concentration.

---

## Application to the Historical Anchors

The two historical anchor applications below use the project's collapse threshold: collapse means rapid, sustained simplification at the polity level.

| Historical case | Dominant nodes | Calculation | CDI | Outcome read |
|---|---|---:|---:|---|
| Western Rome | African grain provisioning; Mediterranean shipping/security; fiscal-military provisioning tied to that supply | (3.0×0.60) + (2.5×0.25) + (2.5×0.15) | **2.80** | High CDI / collapse-compatible |
| Late Tang | Grand Canal transport corridor; Huai–Yangtze grain base; salt-funded canal-revenue system | (3.0×0.55) + (2.5×0.25) + (2.0×0.20) | **2.68** | High CDI / collapse-compatible |

Western Rome scores high because the African grain supply became increasingly important to the imperial West at the very moment the West was already under severe strain; cutting that supply could have devastating effects, even if not every such move was decisive by itself. Late Tang also scores high because the post-An Lushan court became heavily dependent on the Huai–Yangtze economic heartland and on canal transport rebuilt and maintained through the salt monopoly; the state's survival in the late eighth and ninth centuries was structurally tied to that corridor.

---

## Short Test Against Collapse Outcomes

On the narrow historical test requested here, CDI does track the historical outcome direction. Both Western Rome and Late Tang score high, and both are collapse-compatible within the project's threshold language because both cases involve a regime whose provisioning and state capacity became dangerously dependent on concentrated transport and resource nodes before rapid and durable simplification followed. On that basis, CDI should be treated as a **candidate predictive variable** rather than merely a descriptive one.

The caveat is important. This is not yet a rigorous predictive validation. It is a two-case positive test performed on historically chokepoint-heavy anchors. A real predictive test would need at least one matched resilience control with medium or high CDI that did **not** cross the collapse threshold, and ideally one low-CDI case that still collapsed for other reasons. Until that control work is done, the right methodological status is: **promising, portable, and worth retaining — but not yet proven.**

---

## Open Items

- The CDI weights and thresholds are explicitly marked as assumptions and should remain provisional until the team tests them against additional controls.
- No new schema fields are introduced here; CDI is a formal overlay candidate, not a schema expansion for this week.
- Recommended next-step controls: Eastern Rome (high CDI on Egyptian grain, did not collapse — tests whether geographic_defensibility modifies CDI predictiveness); Ming consolidation (recovery case); a low-CDI collapse case (potentially Bronze Age Mycenae, where palace-ledger CDI may actually be high under Gemini's Palace-Administrative system type — worth coding).
