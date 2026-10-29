# ERRATA / PATCH LOG: The Shattered Lens

This document tracks technical contradictions, structural retcons, and mechanical telemetry corrections applied across the repository branches of `netbob/The-Shattered-Lens`. All Act I issues logged here are officially patched within the current version of the manuscript files.

## Open Issues
*   None. All structural, geographic, and timeline discrepancies are verified and resolved.

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

## Forward Notes (writing tasks, not contradictions)
*   ARQ clarifying line for 1B (ruling #10) — written Oct 28, 2026: ARQ connected-mode paragraph inserted into module-1B.md between the 'It's Aris' paragraph and the 'Teletype shattered' line.
*   AS/400 mechanism to be established in text before Chapter 8 (canon defined: cold-chassis + Faraday cage).
*   Chapter 3 redefinition — complete: 'The Ash Migration' (Modules 3A–3E), outline synced — see PATCH-007.
*   Chapter 5 premise vs Modules 1D–1E — the truck-door emergence (Ch5) conflicts with Marcus + Elena on foot in the Pine Ridge hills, rig abandoned; needs a story decision (hillside shelter? return to the truck? rework?). (Chapter 4's F-250 cab tomb resolved by the Hillside Vaults retitle — see PATCH-007.)
*   Pod 4 facility name at Moab — "NSA-South" retained for now; rename if desired.
*   David's route — east out of Utah first, then west to Shaver Lake (long arc, not a direct route); confirm if intended.
