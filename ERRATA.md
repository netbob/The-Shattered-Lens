# ERRATA / PATCH LOG: The Shattered Lens

This document tracks technical contradictions, structural retcons, and mechanical telemetry corrections applied across the repository branches of `netbob/The-Shattered-Lens`. All Act I issues logged here are officially patched within the current version of the manuscript files.

## Open Issues
*   **Module 11C timeline precision (unruled):** Module 11C states 05:40 PDT on December 15, 2026, is "precisely two hours before Robert Hayes would be disarmed before the Central Desk" — 05:40 to Module 11A's 08:00 decree is two hours twenty minutes, and the Module 10E disarmament occurred December 14, 23:58 (before, not after). Precision claim unresolved.
*   **Plate hex root count (unruled):** Settled Canon records three master directory roots (0x4F3B, 0x8E12, 0x00FF); Module 11C displays four, adding 0x7C1A. Fourth root or slip — awaiting ruling.
*   **Module 11C "forty-eight hours ago" (minor, likely rough dialogue):** David's cascade reference stretches to approximately fifty-eight hours by December 15, 05:40, against Module 10E's exact forty-eight. Reads as frozen dialogue rather than a ledger claim; confirmation only.

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

### [PATCH-007] Structural Timeline and Act Realignment
*   **Severity:** High (Structural Continuity)
*   **Identified:** Discrepancies between individual module headers and `outline.md` regarding Act definitions, Chapter 3 titles, and Chapter 4 naming parameters.
*   **Resolution:** Synchronized `outline.md`. Act I permanently encompasses Chapters 1–3. Chapter 3 is titled "The Ash Migration." Act II begins cleanly at Chapter 4, titled "The Hillside Vaults." Applied surgically: the Chapter 3 and Chapter 4 sections were replaced with the ruled titles and module lines; the Chapters 1–2 sections and Chapters 5–12 were left intact.

### [PATCH-008] Chapter 3, Module 3B: Utah Geographic Correction
*   **Severity:** Medium (Geographic Realism)
*   **Identified:** Conflicting slot-canyon positioning placing David Sterling east of Green River while inside the San Rafael Swell.
*   **Resolution:** Corrected coordinates in `chapters/chapter-03/module-3b.md` to specify an unmapped red-rock wash **forty road miles west of Green River**, resolving the physical alignment with the Swell landforms.

### [PATCH-009] Character Identity & Population Distribution Sync
*   **Severity:** Medium (Narrative Integrity)
*   **Identified:** Name collision with Robert Hayes (3D vs. Chapter 10) and an apparent population drop between 3E and 4A.
*   **Resolution:** Confirmed Hayes as a single unified refugee-to-soldier character arc. Outline Module 4A now establishes that the 82 survivors are the primary command group in Pod 1, while the remaining 532 registered refugees are distributed through the secondary surface shafts and silos of Pine Ridge; `module-4a.md` text itself is untouched.

### [PATCH-010] Module 3D: Character Name Collision Resolution
*   **Severity:** High (Character Continuity)
*   **Identified:** Name collision between the irrigation-district refugee in Module 3D and the captured Synod soldier in Chapters 10–11.
*   **Resolution:** Preserved the Chapters 10–11 "Robert Hayes" Synod soldier arc to protect the integrity of the Shaver Lake infiltration narrative. Re-indexed the Module 3D refugee character name to **Robert Cross**, clearing the identity collision across the Act I/Act II timeline. All four name occurrences in `module-3d.md` renamed; no other 3D text altered. Outline Module 3D line updated to match. Supersedes the Hayes portion of PATCH-009's canon ruling (the unified refugee-to-soldier arc is void; see Settled Canon). Note: the PATCH-010 staging snippet ended mid-line at 'accept your caloric credit'; applying it verbatim would have deleted Elena's closing clause ('If you keep the glass, you turn around and walk back down to the water line.'). The clause was deliberately preserved per Michael's ruling; only the four renames were applied.

### [PATCH-011] Chapter 4, Module 4C: Sidereal Velocity Sync
*   **Severity:** Medium (Technical Telemetry Bug)
*   **Identified:** Aris reports a drift rate of "fifteen arcseconds per minute" for a stationary telescope, which contradicts the true earth-rotational sidereal rate of fifteen arcseconds per second.
*   **Resolution:** Clarified the mechanical failure state in `chapters/chapter-04/module-4c.md`. The telescope drive has not stopped dead; the heavy clockwork gear train is actively slipping and grinding through the internal ice shelf within the pier, resulting in a net trailing drift of fifteen arcseconds per minute against the sky's actual movement.

### [PATCH-012] Outline Chapters 5–6: Truck-Cab Premise Resolution
*   **Severity:** Medium (Structural)
*   **Identified:** The outline's Chapter 5 truck-door emergence conflicted with filed Modules 1D–1E, in which Marcus + Elena proceed on foot in the Pine Ridge hills with the rig abandoned. (Chapter 4's F-250 cab tomb was already resolved by the Hillside Vaults retitle — see PATCH-007.)
*   **Resolution:** Rewrote outline Chapters 5–6 (Oct 28, 2026). Chapter 5 now emerges through the Pod 1 subterranean blast doors, with a foraging party salvaging the mechanical fuel pump matrix and vehicle battery plates from the abandoned F-250 before the salt tide seals the lower logging track. Chapter 6 formalizes the deep surface shafts housing the remaining 532 registered refugees, the permanent deep-well hand crank, and the permanent Central Desk. Forward Notes Chapter 5 item marked resolved.

### [PATCH-013] Chapter 4, Module 4E: Character Lineage and Telemetry Data Sync
*   **Severity:** High (Narrative/Technical Bug)
*   **Identified:** Module 4E introduced the illegal character name Sarah Miller, violated the 614-name limit with index 0615, and recorded an unadjusted Zulu timestamp loop for local PDT time occurrences.
*   **Resolution:** Renamed the widow to **Martha Miller**, establishing her cleanly as June Miller's mother back in the valley floor registry. Re-indexed the death log entry to point directly to Arthur's original registration record (**Index 0412**), and standardized the data format block to a manually tracked local time offset string (**-07:00**). The closing allocation line was updated to match (four-hundred-and-twelve).

### [PATCH-014] Appendix B: Tool Index Collision Resolution
*   **Severity:** Medium (Data Schema Consistency)
*   **Identified:** A tool index collision occurred when the three commercial cold chisels were mapped to `[ITEM-013]`, which had already been assigned to the drop-forged 1/2-inch box wrench salvaged in Module 5C.
*   **Resolution:** Preserved both historical entries. The commercial cold chisel array remains anchored to `[ITEM-013]`. The 1/2-inch drop-forged box wrench has been safely re-indexed down to **`[ITEM-014]`**, with an explicit cross-reference note added to its ledger description to prevent future continuity drift.

### [PATCH-015] Chapter 7, Module 7D: Extraction and Transit Gap Closure
*   **Severity:** Medium (Structural Continuity)
*   **Resolution:** Documented the creation of `chapters/chapter-07/module-7d.md` to bridge David Sterling's capture along the canal corridor into Module 8A.

### [PATCH-016] Chapter 8/9: Telemetry Foundation and Script Integration
*   **Severity:** Medium (Technical Framework Alignment)
*   **Resolution:** Created `chapters/chapter-08/module-8e.md` to complete the un-filed Chapter 8 structural spine. Corrected the Shaver Lake foundation to a **granite foundation** in `chapters/chapter-09/module-9b.md` and explicitly mapped the transpacific telemetry monitor to the **Santiago amateur packet transponder (Site 2)**.

### [PATCH-017] Chapter 10, Module 10A: Technician Dialogue Timeline Correction
*   **Severity:** Low (Dialogue Timeline Continuity)
*   **Resolution:** Corrected the Synod line technician's dialogue in `chapters/chapter-10/module-10a.md` from "three weeks ago" to "two weeks ago": the shearing in Module 8E occurred November 28, 2026, and Module 10A is set December 12, 2026 — exactly fourteen days. Preserves the literal calendar line; no other 10A text altered.

### [PATCH-018] Appendix B / Module 10B: Cold Chisel Inventory Sync
*   **Severity:** Medium (Inventory Count Discrepancy)
*   **Identified:** Appendix B logged an inventory of three commercial cold chisels under `[ITEM-013]`, contradicting Module 10B's distribution of twelve chisels to the shaft line.
*   **Resolution:** Reconciled the ledger count to twelve (12) units total by documenting the secondary recovery of nine irrigation district service chisels from the gate heap, maintaining absolute synchronization between the logistics cache and the narrative text.

### [PATCH-019] Chapter 10, Module 10E: Registry Room Combat Closure
*   **Severity:** High (Narrative/Structural Gap)
*   **Identified:** The repository tree skipped the literal execution of the midnight fight module (`10E`), causing downstream citations in Chapter 11 to reference an un-filed asset.
*   **Resolution:** Created `chapters/chapter-10/module-10e.md`, documenting the mechanical clash between the twenty-pound book press and Hayes' rifle stock to provide a complete, verified baseline for the Act IV timeline.

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

*   **Act structure (Oct 28, 2026 ruling):** Act I (The Logic Loop) spans exclusively Chapters 1–3 (Modules 1A–3E). Chapter 3 is permanently titled "The Ash Migration." Act II (The Great Disconnection) begins precisely at Chapter 4, permanently titled "The Hillside Vaults." Module headers win over the prior outline; outline.md patched to match.
*   **3B geography (Oct 28, 2026 ruling):** David Sterling's slot-canyon wash is in the San Rafael Swell, **forty road miles west of Green River**, Utah, heading east toward the Book Cliffs.
*   **Robert Hayes (Oct 28, 2026 ruling, corrected same evening — see PATCH-010):** The Chapters 10–11 soldier. A child of the Shaver Lake Synod, a conscript fighting to save his mother's digital voucher identity before the mainframe suffers absolute bit-rot; captured by Marcus in the Chapter 10 midnight raid, spared, and returned to Shaver Lake with an asylum message in Chapter 11. He is NOT the Module 3D refugee (see Robert Cross).
*   **Robert Cross (Oct 28, 2026 ruling — see PATCH-010):** The Module 3D refugee. Irrigation-district infrastructure supervisor who surrenders his iPhone at the Foothill Ridge Gate on October 26; undergoes a refugee-to-Registry-laborer arc in the foothills. Originally filed as Robert Hayes; renamed to clear the collision with the Chapters 10–11 soldier.
*   **Pod numbering (Oct 28, 2026 ruling):** Independent local numbering architectures. The shared "Pod" designation is purely an artifact of industrial-military jargon; facilities number their sub-structures independently from local deployment blueprints, not a shared network mesh.
*   **Population distribution (Oct 28, 2026 ruling):** The eighty-two in the Pod 1 map room are the core logistical crew, administrative staff, and young families housed directly around the Central Desk. The remaining 532 registered refugees are distributed throughout the facility's extended layout — the deep surface shafts, the legacy missile silos, and the auxiliary equipment decks.

*   **Miller family (Oct 28, 2026 ruling — see PATCH-013):** Arthur Miller (retired diesel mechanic, Clovis irrigation pool) and Martha Miller are June Miller's father and mother, in the valley floor registry. June at the Haleakala Mountain Node does not know her father died November 2 in Pod 1.

*   **ARQ connected mode (Oct 28, 2026 — written into module-1B.md):** ARQ connected-mode paragraph inserted between the 'It's Aris' paragraph and the 'Teletype shattered' line, grounding the unrouted ionospheric knife-edge bounce in physical reality.
*   **Chapter 5 premise (Oct 28, 2026 ruling — see PATCH-012):** Marcus and Elena emerge from the Pod 1 subterranean blast doors into the winter frost; the F-250 is salvaged for parts, not lived in.
*   **Tool index alignment (Oct 28, 2026 ruling — see PATCH-014):** The commercial cold chisel array is anchored to [ITEM-013]; the 1/2-inch drop-forged box wrench is re-indexed to [ITEM-014] with a cross-reference note, preserving both entries.

*   **David's Route:** East out of Utah into the Paradox Basin/sandstone country first to evade the immediate interstate gridlock, then tracking a massive long-arc loop back west toward Shaver Lake in later acts to serve as a hardware calibration asset for the Synod.

*   **Chapter 3 Redefinition:** Complete. Chapter 3 is permanently titled "The Ash Migration" (Modules 3A–3E), with the master repository architecture fully synchronized across `outline.md` per `[PATCH-007]`.

*   **The Oracle Mainframe Framework (established in text — see Module 8A):** The IBM AS/400 Model 720 survives inside a military-grade Faraday cage (double-interlocked copper mesh on polyethylene blocks) four levels beneath the Shaver Lake hydroelectric station, its input strands severed by spring-loaded guillotines 42 minutes before impact; magnetic platters cold and intact, clock frame reference lost with the Boulder broadcast.

*   **The Steel Plate Lever (established in text — see Modules 7D, 8D):** David Sterling explicitly withholds the un-magnetized tool-steel hex-root template, hidden in its oilcloth sleeve against his ribs; he bargains only with his memory of the hex structures. If the Director's crew obtained the template, they could flash the hard-coded root authorization certificates back into the AS/400's firmware, giving the Synod permanent, unilateral legal dominance over the valley's land deeds.

*   **The Chapter 7 Gap (closed — see Module 7D):** David's transit from the Tavaputs trek (7B) to the Shaver Lake vault (8A) is bridged by Module 7D, "The Intercept Loop": captured on the rim trail by a Shaver Lake line patrol after a shale-skid betrayed his position, carried under guard down the mountain. Correction note: an earlier matrix draft claimed 7D was already filed; a directory check at head showed only 7A, 7B, 7C, 7E, and the cage-construction text in fact lives in 8A. That claim was a schema bug, caught before entering ERRATA; 7D was then written and filed.

*   **The Director and Elena (established in text — see Module 8D):** The Director is fully aware of Elena's position at Pine Ridge and of her mechanical preservation of the Registry. He views her not as a lost relative but as an engineering defector who lent corporate network utility knowledge to a scribal collective; his silence on her is calculated, breaking toward the ultimatum scene.

*   **The Shaver Lake Engineer "Miller" (unrelated namesake — see Module 10C):** The junior systems engineer David addresses as "Miller" in Module 10C is an unrelated namesake — a common valley surname trapped on the opposite side of the logic divide — not a blood relative of Arthur, Martha, or June Miller. No lineage link exists. Should a future text module require a hidden blood link, it must earn its entry in the patch log first.

*   **Reginald Miller (unrelated namesake — see Module 11E):** The senior line supervisor from the hydro decks registered at Index 0616 in Module 11E is an unrelated namesake — a common Central Valley surname trapped on the opposite side of the logic divide — not a blood relative of Arthur, Martha, or June Miller, nor of the junior engineer from Module 10C. No lineage link exists. (Ruled October 29, 2026.)

*   **Newcomer double-rotation intake (see Modules 6E, 11A, 11E):** The "eight ounces of salt pork and the pint of water" requested in Module 11E is the full caloric requirement for a twenty-four-hour day — two consecutive twelve-hour manual labor rotations at four ounces per rotation under the 6E/11A lock — not a change to the single-shift unit value. The ledger entry locks the newcomer into the standard shift breakdown under manual verification. No text overwrite required. (Ruled October 29, 2026.)

*   **Arthur Cross (lineage exception — see Modules 3D, 4E, 12A):** Arthur Cross is explicitly codified as Robert Cross's son — a deliberate exception to the standalone namesake default. Robert processed through the gate line on October 26, 2026, as an irrigation supervisor with his family [3D]; five years later his son Arthur sits in the slate room. Arthur is named in memory of the Registry's first casualty, Arthur Miller [4E]. This deepens the inter-generational continuity of the labor group faction [6A, 7A]. (Ruled October 29, 2026.)

*   **Epoch Zero and the First Scribal Day (see Modules 1E, 3E, 12A):** The core fragment of Astraea-9 struck the coast on the evening of October 25, 2026 [1E]. The first complete calendar day under scribal administration — Marcus drew the double horizontal rule on Page Six, closed out the gate registries, and officially locked the books at 18:34 PDT on October 26, 2026 [3E] — is the First Scribal Day, the formal initiation of the paper kingdom. October 26, 2031, is therefore exactly five years to the day from that initiation. (Ruled October 29, 2026.)

*   **Arthur Cross renaming (late November 2026 — see Modules 3D, 4E, 12A):** The renaming interpretation is confirmed and intentional: the four-year-old child was registered in October 2026 under his original pre-impact name; following Arthur Miller's death on November 2, 2026 — the event that forced the Registry's first structural allocation adjustment [4E] — the community formally renamed the child Arthur Cross to honor the first resident to fall under the stone, transforming his identity into a living symbol of the new scribal order. (Ruled October 29, 2026.)

*   **Epoch Zero (October 25, Impact Night) vs. the First Scribal Day (October 26 — see appendix/ledger-page-three.md, Modules 3E, 12A):** The Page Three header stands as ground truth: October 25, 2026, is Epoch Zero (Impact Night). October 26, 2026, is the First Scribal Day. Module 12A's opening line is corrected accordingly: "exactly five years after the First Scribal Day," not "after Epoch Zero." No filename or other text regressions. (Ruled October 29, 2026.)

## Forward Notes (writing tasks, not contradictions)
*   **NSA-South Facility Naming Parameters:** Open rename decision pending for whenever the Moab/Paradox Basin infrastructure re-surfaces in the text.
