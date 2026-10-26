# Walking Errata — The Shattered Lens

Living list of open issues, character-arc questions, and consistency notes for the manuscript. Updated as issues are ruled on or resolved. Resolved items move to Settled Canon and are not re-litigated without a new ruling. Last updated: October 26, 2026.

## Open Issues

### Character arcs

1. **Aris Thorne + June Miller — fates at Haleakala (major).** Last seen at the telescope in 1A. Their fate after the impact is unwritten. As Marcus's brother, Aris's survival or death echoes through Marcus's story. Needed: author decision — do they survive, die at Haleakala, or reappear later (Pine Ridge? elsewhere?)?
2. **David Sterling — fate after Pod 4 (major).** Last seen locked in the dark in the Utah salt vault in 1C, pocket watch ticking. Needed: author decision — does he escape, and does he reappear (Shaver Lake? Pine Ridge? elsewhere?), or does he die in the dark?
3. **Janice Vance — relation + fate (minor).** Senior Infrastructure Engineering lead in 1C; her audio link goes dead at the breaker trip. Relation to the Director/Elena unstated (family or shared surname?). Fate after 1C unwritten. Needed: one line if family; otherwise leave as colleague — and a fate decision.
4. **Elena Vance — inheritance beat (end-of-book).** The final image (Elena binding the book while Marcus watches children write on slate) reads as inheritance: he founds the Registry, she becomes its keeper. If intentional, it is the ending's power. If not, her arc wants one more beat of its own. Needed: author confirmation (inheritance intended?) before the final chapters are drafted.
5. **Estranged-sister thread — dropped or reintroduced?** The 1C Camp Williams start introduced Marcus's estranged sister (Sarah Vance); the rewrite removed her entirely. Needed: author decision — reintroduce the estrangement thread elsewhere, or drop it permanently (current state: dropped).

### Technical / consistency

6. **AS/400 hardening mechanism (major).** The Director's Shaver Lake AS/400 survives while Marcus declares silicon dead in 1B. The Synod's survival is the exception the war depends on. Needed: one explicit mechanism (bunker, Faraday shielding, powered-down at impact, or other) established before Chapter 8, when the Synod terminal appears.
7. **SITE 2 (minor).** 1B's Teletype header reads "RAW TELEMETRY INVERSION BURIED FROM SITE 2." What is Site 2 — Haleakala's designation, a second site, the Atacama node? Needed: one clarifying line.
8. **St. George salt geology (minor).** Pod 4 sits "three hundred feet inside a solid salt formation" with "salt flats" near St. George, which is red-rock country; Utah's salt bodies are the Paradox Basin (southeast) and Bonneville (northwest). Needed: a line grounding the salt (fictional salt body, or site sits on salt) — or relocate the salt detail.
9. **1C date pin (minor).** 1C's logs read 05:44Z; causality forces October 22 (the break precedes 1A's October 22 effects), recorded in the editor's notes. The date is unstated in the text. Needed: a date line in 1C if the author wants it pinned on the page.
10. **ARQ connected vs collapsed network (minor).** 1B connects via "[ARQ PACKET CONNECTED]" after the network logic established that connected mode was dead. The direct ionospheric bounce justifies it, but one line distinguishing the direct bounce from the dead routed network would keep the logic tight.
11. **"Three hundred miles" (trivial).** Elena's "three hundred miles west" (Point Conception to Clovis) is road distance; straight-line is ~170 miles. Fine as a stressed estimate, or tighten to "under two hundred miles."

### Structure / repo

12. **Chapter 1, Module 1E — not yet written.** Four of five modules filed (1A–1D). One outline beat not yet dramatized: Marcus computing the true trajectory from the raw data (1B shows receipt, not calculation). Needed: author decision on 1E's content (calculation scene? government misclassification beat? other?).
13. **Outline sync (repo hygiene).** outline.md still says "Robert Miller" (Chapter 10; ruled: Robert Hayes), still says "independent amateur astronomer in Chile" (ruled: ACT/Rubin data via Santiago amateur transponder), and doesn't state the ruled relationships (Thorne brothers, Vance father/daughter, June Miller). Needed: a sync pass on outline.md when it is next touched.
14. **The lens — literal, metaphor, or both? (theme).** 1D introduces a literal atmospheric lens (the ionization glow forming "a vast, shimmering lens" over the valley). Needed: author confirmation — is that the title's lens, or does a physical optic (Haleakala scope?) also carry it?

## Settled Canon (do not re-litigate without a new ruling)

- Timeline: 1C Oct 22, 05:44Z → 1A Oct 22, 01:15–04:12 HST → 1B Oct 23, 05:30 PDT → 1D Oct 25, 06:10 PDT → impact Oct 25 evening.
- Mirror: Pan-STARRS 2 primary is 1.8 meters. Camera: 1.47-gigapixel focal plane; the FITS appendix's 9216² frame is a tracking subframe, not the full mosaic.
- Astraea-9: tidally fragmented, Shoemaker-Levy 9 style; primary 11 km chunk hits Point Conception; trailing fragments graze the ionosphere pre-impact (the 1B wavefront mechanism).
- Chile source: Atacama Cosmological Telescope / Vera C. Rubin data, relayed via an amateur packet transponder in Santiago.
- File size: 9216² × 8 bytes = 679.5 MB ("six hundred eighty megabytes"); BITPIX -64 stands.
- Drift: 1.44 arcsec over 2h25m = 0.000166 arcsec/s (RA); DEC scaled by the same factor to 0.000045 arcsec/s, preserving vector direction.
- Names: Aris + Marcus Thorne are brothers. Elena Vance + the Director are father/daughter. Chapter 10 soldier is Robert Hayes. Haleakala grad student is June Miller (was Sarah Miller). 1C lead is David Sterling (not Vance). The name Sarah appears nowhere in the filed book.
- Truck: the F-250's dead electronics are bypassed by Elena's manual brass fuel pump (mechanically revivable); 1B's "forty gallons" (estimate) vs 1D's "forty-two gallons" (dipstick) is consistent.
- Superseded drafts (do not revive): 1B "The Packet Horizon" (v1) and 1C Camp Williams start (David Vance / Sarah Vance) were never filed. The 1C rewrite voids the earlier Sarah Vance married-name and David-as-brother rulings.
