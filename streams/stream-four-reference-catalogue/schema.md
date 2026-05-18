# Reference Entry Schema

**Version:** 1.0  
**Date:** 2026‑05‑18  

Every entry in the Stream Four Reference Catalogue must follow this schema.

## Required fields

| Field | Description | Example |
|---|---|---|
| `title` | Full title of the work (in original language and English translation if not originally English) | “The Second Coming” / “The Second Coming” |
| `author` | Author or creator. Use standard scholarly transliteration for non‑Latin scripts. | W.B. Yeats |
| `date` | Date of composition/publication. Use `c.` for approximate dates. If the work was published posthumously, note the date of writing. | 1919 (written), 1920 (published) |
| `type` | Genre: `poetry`, `fiction`, `philosophy`, `visual-art`, `film`, `music`, `science-metaphor`, `essay`, `aphorism`, `other` | poetry |
| `source_location` | Where the full text can be found (URL, standard edition, library call number). For online sources, include access date. | *The Collected Poems of W.B. Yeats* (1989), ed. Richard J. Finneran |
| `load_bearing_passage` | The specific excerpt(s) that do the analytical work. Include original language if the work is not in English and the translation is relevant. | “Things fall apart; the centre cannot hold” |
| `analytical_use` | **The most important field.** What specific analytical work does this reference perform that prose alone cannot? Be precise. | Compresses the concept of systemic incoherence under stress into a single, instantly‑graspable image; useful for arguments about institutional fracture where the process is diffuse and hard to visualise. |
| `project_context` | Which section of the project this reference has been or could be used in: `book-chapter`, `dispatch`, `field-note`, `multiple`. If used already, cite the document. | Multiple; referenced in Fieldnotes Dispatch #3 (financial fragility) and in the Stream Three Late Tang case brief (as a cross‑cultural collapse motif) |
| `catalogue_notes` | Any curatorial notes: warnings about overuse, alternative translations, connections to other entries, etc. | Overexposed in collapse literature; if used, prefer the less‑quoted lines (“the falcon cannot hear the falconer”) to avoid cliché. |
| `confidence` | Confidence in the reference’s load‑bearing status: `Confirmed` (used in project prose and proven load‑bearing), `Proposed` (suggested but not yet used), `Under Review` (under editorial scrutiny). | Confirmed |
| `date_added` | Date the entry was created (YYYY‑MM‑DD). | 2026‑05‑18 |
| `last_modified` | Date the entry was last updated. | 2026‑05‑18 |

## Optional fields

| Field | Description |
|---|---|
| `cross_references` | List of other catalogue entries this reference connects to. |
| `translator` | If the work is translated, the translator’s name. |
| `related_project_documents` | Links to project documents that discuss or use this reference. |
| `editorial_history` | Notes on revisions, promotions, demotions. |