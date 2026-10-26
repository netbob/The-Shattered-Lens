# Walking Errata — The Shattered Lens

Living list of open issues, character-arc questions, and consistency notes for the manuscript. Updated as issues are ruled on or resolved. Resolved items move to Settled Canon and are not re-litigated without a new ruling. Applied patches are recorded in the Patch Log below. Last updated: October 26, 2026.

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

12. **Chapter boundary — impact in Chapter 1 vs Chapter 3 (structural).** Module 1E depicts the impact, but the outline puts the impact in Chapter 3 ("The Crimson Horizon"). Chapter 1 now has all five modules filed (1A–1E), running discovery through impact. Needed: author ruling — does Chapter 1 now run discovery→impact (Chapters 2–3 redefined), or does 1E belong in Chapter 3 (and Chapter 1's fifth module is still the calculation beat — Marcus computing the trajectory, which 1B shows receipt of, not calculation of)?
13. **Outline sync (repo hygiene).** outline.md still says "Robert Miller" (Chapter 10; ruled: Robert Hayes), still says "independent amateur astronomer in Chile" (ruled: ACT/Rubin data via Santiago amateur transponder), and doesn't state the ruled relationships (Thorne brothers, Vance father/daughter, June Miller). Needed: a sync pass on outline.md when it is next touched.
14. **The lens — literal, metaphor, or both? (theme).** 1D introduces a literal atmospheric lens (the ionization glow forming "a vast, shimmering lens" over the valley). Needed: author confirmation — is that the title's lens, or does a physical optic (Haleakala scope?) also carry it?

15. **Resolved — see PATCH-002.** (Six-mile vs eleven-kilometer: the six-mile core is the largest piece of the fragmented eleven-kilometer body.)
16. **"Three hundred miles west of Point Conception" (1E).** Read literally, this puts the impact 300 miles offshore in deep ocean — contradicting both the canon impact AT Point Conception and 1E's own "shallow continental shelf" (the shelf is ~10–30 miles wide; 300 miles out is abyssal plain). Likely slip for "at Point Conception, three hundred miles west [of the valley]" — echoing Elena's 1B line. Needed: rephrase to pin the impact at Point Conception. (Sibling of item 11: the three-hundred-miles figure needs pinning in both places.)
17. **Seventy-eight-second gap (1E).** 1E has the mantle shockwave arriving "precisely seventy-eight seconds before the sound wave" at the Sierra base (~300 km from Point Conception). Seismic P-wave covers ~300 km in ~50 s; sound takes ~860 s (~14 min) — the gap should be ~13–14 minutes, not 78 seconds (a 78 s gap implies ~27 km). Needed: change the number (or the wave described isn't acoustic sound).
18. **Forty miles into the stratosphere (1E).** Forty miles is ~64 km; the stratosphere tops out at ~50 km (~31 mi) — forty miles up is the mesosphere. Needed: "forty miles into the upper atmosphere" or "twenty miles into the stratosphere."
19. **"Air cooling loops on our lungs" (1E).** Unclear whether Marcus and Elena have breathing gear with cooling loops (never established) or Elena means their lungs failing from the sulfur mix. Needed: one clarifying word.
20. **Foothill gate vs ridge gate (1D vs 1E).** 1D says "past the foothill gate"; 1E says "make the ridge gate by dawn." Same gate under two names, or two gates? Needed: one name (or a line distinguishing them).

21. **Chile relay mechanism — transponder vs bridge node (PATCH-003 held).** The draft patch log proposes ACT data via 'an automated network bridge node'; settled canon records a Santiago amateur packet transponder (filed 1B says only 'CHILE APER NODE'). Needed: author ruling — keep the transponder, or retcon to the bridge node (and update the canon note). PATCH-003 is not logged as patched until ruled.

## Patch Log

The following patches are officially applied in the current manuscript files. PATCH-003 is held pending a ruling (see open item 21) and is not logged here.

### [PATCH-001] Chapter 1, Module 1A: Primary Aperture Discrepancy
*   **Severity:** High (Technical Inconsistency)
*   **Identified:** Initial drafts cited an "eleven-meter primary mirror" for the Pan-STARRS telescope array at the summit of Haleakala. This directly violates real-world architectural design and optical engineering specifications.
*   **Resolution:** Modified `chapters/chapter-01/module-1A.md` to correctly specify a **1.8-meter diameter primary aperture mirror** mapping to the actual PS1 and PS2 alt-azimuth optical designs. Grounded the massive pixel output in the camera's **1.47-gigapixel focal plane** rather than raw mirror scale.

### [PATCH-002] Chapter 1, Module 1A/1B: Astraea-9 Orbital Structure
*   **Severity:** Medium (Narrative/Physics Realism)
*   **Identified:** The initial plot layout implied a completely monolithic eleven-kilometer impact event, which failed to explain early high-altitude atmospheric ionization and localized radio frequency inversion events occurring prior to the primary kinetic impact.
*   **Resolution:** Retconned the astronomical taxonomy of Astraea-9 to a **tidally fragmented long-period comet**. The object behaves as a "string of pearls" array. The eleven-kilometer body fragmented; its largest piece — the primary six-mile-wide solid carbonaceous/methane-ice core — is targeted at the Point Conception shelf. Advanced micro-fragments entered the upper exosphere hours early, generating the localized ionospheric shearing, electrical gridding, and violet light emissions tracked by Marcus Thorne on Dakota Avenue. (Closes open item 15.)

### [PATCH-004] Chapter 1, Module 1B: Transmission Filing Loop Closure
*   **Severity:** High (Hanging Execution)
*   **Identified:** The original staging file for Module 1B dropped off mid-scene, leaving Marcus Thorne's packet intercept sequence incomplete and missing his direct manual transition to physical ledger logging.
*   **Resolution:** Completed full integration of `chapters/chapter-01/module-1B.md`. The text now explicitly details the failure of the truck's diagnostic CAN bus and quartz resonator, the death of the CRT monitoring glass, and Marcus's manual transition to physical ledger logging: the Teletype sheet pasted as Page One of the leather ledger with a handwritten entry.

## Settled Canon (do not re-litigate without a new ruling)

- Timeline: 1C Oct 22, 05:44Z → 1A Oct 22, 01:15–04:12 HST → 1B Oct 23, 05:30 PDT → 1D Oct 25, 06:10 PDT → impact Oct 25 evening.
- Mirror: Pan-STARRS 2 primary is 1.8 meters. Camera: 1.47-gigapixel focal plane; the FITS appendix's 9216² frame is a tracking subframe, not the full mosaic.
- Astraea-9: tidally fragmented, Shoemaker-Levy 9 style; the eleven-kilometer body fragmented and its largest piece — the six-mile-wide core — hits Point Conception; trailing fragments graze the ionosphere pre-impact (the 1B wavefront mechanism). (PATCH-002)
- Chile source: Atacama Cosmological Telescope / Vera C. Rubin data, relayed via an amateur packet transponder in Santiago.
- File size: 9216² × 8 bytes = 679.5 MB ("six hundred eighty megabytes"); BITPIX -64 stands.
- Drift: 1.44 arcsec over 2h25m = 0.000166 arcsec/s (RA); DEC scaled by the same factor to 0.000045 arcsec/s, preserving vector direction.
- Names: Aris + Marcus Thorne are brothers. Elena Vance + the Director are father/daughter. Chapter 10 soldier is Robert Hayes. Haleakala grad student is June Miller (was Sarah Miller). 1C lead is David Sterling (not Vance). The name Sarah appears nowhere in the filed book.
- Truck: the F-250's dead electronics are bypassed by Elena's manual brass fuel pump (mechanically revivable); 1B's "forty gallons" (estimate) vs 1D's "forty-two gallons" (dipstick) is consistent.
- Chapter 1 complete: modules 1A–1E filed; 1E is the impact evening, October 25 (date unstated in text, forced by the outline + 1D).
- Marcus + Elena on foot with a two-wheeled handcart in 1E (rig abandoned, per 1D's warning).
- San Joaquin basin floods: the displacement wave reaches the delta gates by noon, matching 1B's five-hundred-foot surge line.
- Superseded drafts (do not revive): 1B "The Packet Horizon" (v1) and 1C Camp Williams start (David Vance / Sarah Vance) were never filed. The 1C rewrite voids the earlier Sarah Vance married-name and David-as-brother rulings.
