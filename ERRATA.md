# ERRATA / PATCH LOG: The Shattered Lens

This document tracks technical contradictions, structural retcons, and mechanical telemetry corrections applied across the repository branches of `netbob/The-Shattered-Lens`. All Act I issues logged here are officially patched within the current version of the manuscript files.

## Open Issues
*   **Outline sync pending (Michael's call):** Chapter 3 is titled 'The Ash Migration' in the Module 3A header (first Chapter 3 module filed), but the outline still lists Chapter 3 as 'The Crimson Horizon' (content TBD). All six Chapter 2-3 modules filed so far (2A-2E, 3A) carry 'Act II: The Great Disconnection' headers, but the outline places Chapters 2 and 3 in Act I (Act II starts at Chapter 4). The outline is untouched pending Michael's decision on the Chapter 3 title and the Chapter 2-3 act placement.

## Patch Log

### [PATCH-001] Chapter 1, Module 1A: Primary Aperture Discrepancy
*   **Severity:** High (Technical Inconsistency)
*   **Identified:** Initial drafts cited an "eleven-meter primary mirror" for the Pan-STARRS telescope array at the summit of Haleakala. This directly violates real-world architectural design and optical engineering specifications.
*   **Resolution:** Modified `chapters/chapter-01/module-1A.md` to correctly specify a **1.8-meter diameter primary aperture mirror** mapping to the actual PS1 and PS2 alt-azimuth optical designs. Grounded the massive pixel output in the camera's **1.47-gigapixel focal plane** rather than raw mirror scale.

### [PATCH-002] Chapter 1, Module 1A/1B: Astraea-9 Orbital Structure
*   **Severity:** Medium (Narrative/Physics Realism)
*   **Identified:** The initial plot layout implied a completely monolithic eleven-kilometer impact event, which failed to explain early high-altitude atmospheric ionization and localized radio frequency inversion events occurring prior to the primary kinetic impact.
*   **Resolution:** Retconned the astronomical taxonomy of Astraea-9 to a **tidally fragmented long-period comet**. The object behaves as a "string of pearls" array. The eleven-kilometer body fragmented; its largest piece — the primary six-mile-wide solid carbonaceous/methane-ice core — is targeted at the Point Conception shelf. Advanced micro-fragments entered the upper exosphere hours early, generating the localized ionospheric shearing, electrical gridding, and violet light emissions tracked by Marcus Thorne on Dakota Avenue.

### [PATCH-003] Chapter 1, Module 1A/1B: Chile Telemetry Source Integration
*   **Severity:** Low (Contextual Realism)
*   **Identified:** Aris Thorne's data verification source in the Southern Hemisphere was ambiguously attributed to a generic "independent amateur astronomer," and SITE 2 was unexplained.
*   **Resolution:** Standardized to the **Santiago amateur packet transponder (Site 2)**, which processed Atacama Cosmological Telescope (ACT) / Vera C. Rubin data before the transoceanic gates fell. The "automated network bridge node" draft is superseded.

### [PATCH-004] Chapter 1, Module 1B: Transmission Filing Loop Closure
*   **Severity:** High (Hanging Execution)
*   **Identified:** The original staging file for Module 1B dropped off mid-scene, leaving Marcus Thorne's packet intercept sequence incomplete and missing his direct manual transition to physical ledger logging.
*   **Resolution:** Completed full integration of `chapters/chapter-01/module-1B.md`. The text now explicitly details the failure of the truck's diagnostic CAN bus and quartz resonator, the death of the CRT monitoring glass, and Marcus's manual transition to physical ledger logging: the Teletype sheet pasted as Page One of the leather ledger with a handwritten entry.

### [PATCH-005] Chapter 1, Modules 1C/1E: Physics, Geology, and Location Sync
*   **Severity:** High (Technical/Geographic Consistency)
*   **Identified:** Module 1E placed the impact "three hundred miles west of Point Conception" (deep ocean, contradicting the shallow shelf); the seismic-acoustic gap was seventy-eight seconds (should be ~thirteen minutes at 300 km); the plume rose "forty miles into the stratosphere" (mesosphere); "air cooling loops" implied nonexistent breathing gear; Pod 4's St. George salt flats contradicted Utah geology; Module 1C's log dates were unstated.
*   **Resolution:** Module 1E rewritten — impact "at Point Conception, three hundred road miles west of the valley floor"; gap "precisely thirteen minutes"; plume "forty miles into the upper atmosphere"; "before our lungs fail from the superheated sulfur mix." Pod 4 relocated to the Paradox Basin formation near Moab, Utah (salt dome). Module 1C log timestamps pinned to 2026-10-22T05:44:12Z et seq.

### [PATCH-006] Chapter 1, Modules 1D/1E + outline.md: Text Corrections and Chapter-Boundary Shift
*   **Severity:** Medium (Structural)
*   **Identified:** Gate named inconsistently (foothill gate vs ridge gate); Module 1D dialogue needed tightening; the outline placed the impact in Chapter 3 while Chapter 1's modules ran through the impact; the outline carried superseded names and sources.
*   **Resolution:** Gate standardized to "The Foothill Ridge Gate" (1D snippet + 1E rewrite). Module 1D dialogue passage replaced with the corrected snippet (dead vehicles, navigation screens clearing, municipal water lockup, "Keep the paper dry" refrain). outline.md updated — Chapter 1 runs discovery through impact (1A–1E); Chapter 2 focuses on pitch-black aftermath and infrastructural disintegration; Chapter 10 soldier is Robert Hayes; Chile source is ACT/Rubin via Santiago Site 2; Thorne brothers and Vance father/daughter recorded.

## Settled Canon
*   **Timeline:** Oct 22–25, 2026, discovery through impact. 1C Oct 22, 05:44Z → 1A Oct 22, 01:15–04:12 HST → 1B Oct 23, 05:30 PDT → 1D Oct 25, 06:10 PDT → impact Oct 25 evening.
*   **Chapter boundary:** Chapter 1 runs discovery through impact (Modules 1A–1E). Chapter 2 focuses on pitch-black aftermath and infrastructural disintegration.
*   **Fates:** Aris and June survive on Haleakala (10,000 feet, above the displacement waves) and become an independent Mountain Node, tracking atmospheric collapse with analog optics and wind-up equipment, contacting Pine Ridge via shortwave mirror-bounce in later acts. David escapes Pod 4 via pneumatic emergency bypass doors, migrates eastward out of Utah carrying the physical cryptographic master key template on an un-magnetized metal plate, and eventually surfaces as a technical resource for the Synod at Shaver Lake before realizing their database is rotting. Janice perishes during the breaker explosion in 1C.
*   **Relationships:** Aris + Marcus Thorne are brothers. Elena Vance + the Director are father/daughter. Janice Vance is the Director's sister and Elena's estranged aunt (the Director stayed with centralized digital systems; Elena broke away to physical grid mechanics with Marcus). The estranged-sister thread (Sarah Vance) is permanently dropped.
*   **Names:** Haleakala grad student is June Miller (was Sarah Miller). Chapter 10 soldier is Robert Hayes. 1C lead is David Sterling (not Vance). The name Sarah appears nowhere in the filed book.
*   **Astraea-9:** Tidally fragmented, Shoemaker-Levy 9 style; the eleven-kilometer body fragmented and its largest piece — the six-mile-wide core — hits Point Conception; trailing fragments graze the ionosphere pre-impact (the 1B wavefront mechanism).
*   **Chile source:** Atacama Cosmological Telescope / Vera C. Rubin data, relayed via the Santiago amateur packet transponder (Site 2).
*   **Mainframe shielding:** Shaver Lake AS/400 survived via cold-chassis upgrade disconnection inside a military-grade Faraday cage, input lines disconnected, protecting its magnetic disk architecture from the early ionization wave.
*   **Pod 4 geology:** Paradox Basin formation near Moab, Utah (deep salt dome), not St. George.
*   **1C date:** Console logs read 2026-10-22T05:44:12Z et seq.
*   **ARQ:** Direct ionospheric knife-edge bounce mimics a point-to-point physical connection; the handshake is a raw, non-routed, un-encrypted RF link, distinct from the dead routed network (clarifying line for 1B to be written — see Forward Notes).
*   **"Three hundred miles":** Kept as a stressed human estimate (circuitous mountain-pass path, not straight-line flight distance); 1E standardizes to "three hundred road miles west of the valley floor."
*   **The lens:** Both — the literal atmospheric lens from the ionization inversion, and the shattered optical lenses of the dying automated observatories.
*   **The gate:** The Foothill Ridge Gate.
*   **The impact:** At Point Conception; thirteen-minute seismic-acoustic gap; plume forty miles into the upper atmosphere; lungs fail from the superheated sulfur mix.
*   **The truck:** The F-250's dead electronics are bypassed by Elena's manual brass fuel pump (mechanically revivable); 1B's "forty gallons" (estimate) vs 1D's "forty-two gallons" (dipstick) is consistent; Marcus + Elena proceed on foot with a two-wheeled handcart by 1E.
*   **The mirror/camera:** Pan-STARRS 2 primary is 1.8 meters; camera is 1.47-gigapixel focal plane; the FITS appendix's 9216² frame is a tracking subframe, not the full mosaic.
*   **File size / drift:** 9216² × 8 bytes = 679.5 MB ("six hundred eighty megabytes"); BITPIX -64 stands. Drift 1.44 arcsec over 2h25m = 0.000166 arcsec/s (RA); DEC scaled to 0.000045 arcsec/s, preserving vector direction.
*   **Superseded drafts (do not revive):** 1B "The Packet Horizon" (v1) and 1C Camp Williams start (David Vance / Sarah Vance) were never filed. The 1C rewrite voids the earlier Sarah Vance married-name and David-as-brother rulings.

## Forward Notes (writing tasks, not contradictions)
*   ARQ clarifying line for 1B (ruling #10) — to be written.
*   AS/400 mechanism to be established in text before Chapter 8 (canon defined: cold-chassis + Faraday cage).
*   Chapter 3 redefinition — its impact content moved to Chapter 1; new content now defined by Module 3A ('The Ash Migration,' delta back-surge, Oct 26 noon). Outline sync (title + Chapter 2-3 act placement) pending — see Open Issues.
*   Chapters 4–5 premise vs Modules 1D–1E — the F-250 cab tomb (Ch4) and truck-door emergence (Ch5) conflict with Marcus + Elena on foot in the Pine Ridge hills, rig abandoned; needs a story decision (hillside shelter? return to the truck? rework?).
*   Pod 4 facility name at Moab — "NSA-South" retained for now; rename if desired.
*   David's route — east out of Utah first, then west to Shaver Lake (long arc, not a direct route); confirm if intended.
