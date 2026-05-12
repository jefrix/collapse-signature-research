# Methodology Updates for v3

## Executive Summary

Based on the past week's case work, this update incorporates **four major themes** into Methodology v3. First, we formalize a **literary-sparse asymmetry rule** for cases with little or no contemporary written evidence, as flagged by the Mongol-fragmentation brief. When a case falls below a strict source threshold, the literary-strategic module's weight is reduced and proxy signals from successors or neighbors are used. Second, we treat **system type** (conquest empire vs agrarian-bureaucratic vs city-state vs modern state) as a coded variable. Conquest empires (like the Mongols, Romans, or British East India Company) are flagged by rapid military expansion, multi-ethnic elites, and frontier-driven governance, whereas agrarian-bureaucratic states (e.g. Zhou China or Mughal India) center on farming, dynastic legitimacy, and internal bureaucracy. Third, we add a **common-mode shock susceptibility** variable. This captures when multiple polities face the same large shock: for example, the 14th-century Black Death struck all Mongol khanates near-simultaneously, and by analogy a single AI-sector shock could hit the entire "AI capital web." Finally, we include all nine of the Oracle-generated schema refinements (actor-role split, obligation state, customer funding mode, vehicle visibility, guarantee support, counterparty concentration, power dependencies, common-mode correlation, and evidence scope) because the Microsoft case and others will need them. These changes mesh seamlessly with the existing Tainter/Cline/Turchin/Seshat framework and respond directly to the new cases and controls now in hand.

## Literary-Sparse Asymmetry Rule

**Rule:** If a case's literary corpus is extremely limited (threshold TBD), down-weight literary-strategic codes.
**Operational thresholds:**
- *Literary-Rich:* ≥10 unique contemporary texts or inscriptions per century relevant to elite discourse.
- *Literary-Moderate:* 2–10 texts per century.
- *Literary-Sparse:* <2 texts per century, or entirely lacking elite-authored narrative records.

In literary-sparse cases, code the case as **sparse**, use successor or nearby society texts only with caveats, and mark all narrative-driven variables as low confidence. For example, the Mongol fragmentation brief noted virtually no native chronicles of Mongol-ruled Central Asia; in such cases we rely on travelogues, court documents of successor states, or archaeological proxies for ideological analysis, and we do not let a weak corpus dominate the collapse signature.

## Conquest Empires as a System Type

We now explicitly code **system type** as a stratifying variable with four categories: *conquest empire*, *agrarian-bureaucratic state*, *city-state confederation*, and *modern liberal-bureaucratic state*. Criteria:

- **Conquest Empire:** Extensive territory acquired by continuous military conquest; multi-ethnic ruling class; frontier garrisons; tribute economy; personal or dynastic loyalty chains. (Examples: Mongol Empire, Alexander's Empire, Napoleonic France, British East India Company as a quasi-empire.)
- **Agrarian-Bureaucratic State:** Territory cohesive around a single heartland; legitimacy based on dynastic or theocratic sanction; heavy emphasis on agriculture and irrigation; strong centralized bureaucracy with tax/famine relief roles. (Examples: Roman Empire (at its core, after expansion), Ming/Qing China, Mughal India.)
- **City-State Confederation:** Multiple self-governing city-states in loose alliance or hegemony; collective military effort but shared sovereignty; limited imperial control. (Examples: Delian League/Athenian Empire, early Italian Renaissance leagues, Hanseatic League.)
- **Modern Liberal-Bureaucratic State:** Institutionalized rule-of-law state in industrial/post-industrial society; elected or constitutional regime; economic base not purely agrarian; standing military. (Examples: post-World-War-II democracies, socialist republics with some free-market features, etc.)

The code answers allow us to compare, for example, whether **conquest empires** tend to collapse in bursts tied to overextended frontiers and shared disasters (as hypothesized for the Mongol and late-British cases) versus how agrarian bureaucracies produce different patterns (e.g. dynastic breaks vs fragmentary successor states).

## Common-Mode Shock Susceptibility

**Rule:** Add a `common_mode_shock` variable (Low/Medium/High) to capture whether geographically distinct polities experienced the same shock.
**Operational criteria:**
- Identify candidate shock (e.g. plague, climate event, AI chip crash).
- **High** if multiple polity-level collapses or near-collapses coincide in time and have shock-consistent triggers. (Example: Black Death arguably struck multiple khanates in the late 1340s.)
- **Medium** if the shock was widespread but outcomes differed (some collapse, some adapt).
- **Low** if crises were temporally isolated or regionally confined.

This flag is coded at the case group level (e.g. "Late Mongol Empire episode") and annotated per polity case. It helps test whether events are independent or part of a single system-wide disturbance. In the Oracle example, we treat `common_mode_shock=High` because a single sectoral downturn in AI (e.g. a chip shortage or regulatory ban) would affect both the AI infrastructure build (OpenAI) and the financial stack (private equity, CRE), as the methodology now explains explicitly.

## Other New Protocols

- **Rising Narrative, Hidden Decline:** The Gemini LBA brief suggests that a successful *return-to-foundations* campaign can temporarily create a confident "rising" narrative even as systemic strain deepens. Methodology v3 introduces a sub-code under narrative-classification: if `narrative=rising` but the polity has also launched an explicit restorative project ("return to foundations") without increasing complexity, flag as *rising-but-vulnerable*. This helps prevent misclassifying a successful propaganda campaign as economic stabilization.

- **Schema Module Additions:** The nine fields from the Oracle memo are now official:
  1. `actor_legal_role_split` (distinguish operator vs sponsor vs offtaker vs guarantor etc.)
  2. `obligation_recognition_state` (on-balance vs signed/unrealized liabilities)
  3. `customer_funding_mode` (prepayment, in-kind, etc.)
  4. `vehicle_visibility` (known vehicles vs sector-inferred)
  5. `guarantee_support` (guarantee details)
  6. `counterparty_concentration_visibility` (known vs unknown share)
  7. `power_dependency_obligation` (for energy/power commitments)
  8. `common_mode_shock` (as above)
  9. `evidence_scope` (issuer-specific vs general insight)

The methodology document will codify these fields as part of the ontology, with data-entry rules illustrated by the Oracle and forthcoming Microsoft cases.
