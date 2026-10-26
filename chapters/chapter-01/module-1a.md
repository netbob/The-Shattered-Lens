# Act I: The Logic Loop

## Chapter 1: The Ephemeris Error

### Module 1A: The Haleakala Telemetry Anomaly

The liquid-helium cooling lines on the Pan-STARRS 2 telescope at the summit of Haleakala had developed a micro-fissure three days earlier. It wasn't enough to trip the automated facility alarms in Manoa, but it shifted the thermal noise floor of the primary mosaic CCD by four-tenths of a Kelvin. To the automated image-processing pipeline—a cluster of aging rack servers humming in an air-conditioned concrete vault beneath the telescope deck—the tiny increase in dark current was treated as a transient masking artifact.

Dr. Aris Thorne didn't care about the dark current. He cared about the variance in the third-order residual matrix of field stars in Sector November-Red.

Aris sat in the tracking gallery, his fingers tap-tapping on the edge of a plastic desk that smelled of stale coffee and industrial ozone cleaners. On his primary monitor, a terminal window ran a loop of Unix commands, piping raw astrometric data through a local instance of ORBIT9. The terminal output was clean, sterile, and wrong.

[INFO] Processing Sector Nov-R: 4,102 point sources verified.
[INFO] Baseline cross-match: 100% compliance with Gaia-DR3 catalog.
[WARN] 1 anomalous transient flagged; rejected as transient hot pixel (CCD-T: 68.2K).

"It’s not a hot pixel, Sarah," Aris said, his voice flat, drained of sleep. He didn't look at the graduate student curled on the surplus couch behind him, wrapped in a fleece blanket that bore the faded logo of the University of Hawaii.

Sarah Miller stirred, her glasses crooked on her face. "The pipeline auto-purges everything with a point-spread function below zero-point-eight if the thermal stability loop is open, Aris. If it’s an artifact, the filter caught it. Let the scheduler finish the scan. I need to log those Cepheid variables before dawn or the department head will dock our compute credits."

Aris didn't answer. He aborted the execution loop with a sharp strike of the carriage return.

He wasn't using the university’s standard Web-based dashboard. He had bypassed the front-end interface entirely, tunneling into the raw image repository via a secure shell connection that used a local, physical cryptographic key—a heavy, black USB token that sat in his workstation’s chassis like a structural wedge.

He pulled the raw FITS file from the midnight frame. It was six hundred eighty megabytes of binary data, a map of absolute cold space over the Pacific captured by the 1.8-meter primary mirror. He didn't render it with the standard smoothing algorithms. He forced the terminal to output the raw pixel intensity values along a localized grid spanning fifty coordinates across the constellation of Pegasus.

There, embedded in the numbers, was the discrepancy.

The telescope’s massive 1.47-gigapixel Cassegrain focus camera had captured an asymmetric Gaussian curve spread across seven pixels of the Orthogonal Transfer Array, its peak intensity shifting westward by precisely 1.44 arcseconds between the 01:15 and 03:40 exposures.

"Look at the drift," Aris whispered, his hand reaching out to trace the glowing green numbers on the screen. "It’s not a charge leak. The centroid is moving along an unperturbed hyperbolic vector. But the magnitude is too low for an asteroid at this declination. It’s not reflecting solar light. It’s absorbing it. And it's not a single solid body—the light curve is undulating at secondary frequencies. It’s fragmenting. The main mass has trailing fragments grazing the exosphere right now."

Sarah sat up, the blanket slipping to the linoleum floor. She squinted at the terminal. "If it's an Oort object with an albedo below zero-point-zero-three, the automatic survey filters would treat it as a background noise fluctuation. It takes three consecutive detections with a signal-to-noise ratio above five for the Minor Planet Center script to generate an alert."

"The script didn't generate an alert because the script couldn't verify the timestamp," Aris said. He opened a second terminal window, querying the facility’s primary network time server. "Look at the NTP logs. The Haleakala local master clock is drifting by twelve milliseconds every hour. The upstream stratum-1 servers at Boulder aren't answering the handshake requests. Every time our local daemon tries to sign the telemetry packet, the transaction fails because the cryptographic validity window has closed."

Sarah stood up, her bare feet cold against the floor. She walked over to the terminal, her eyes reflecting the green phosphorescence of the text blocks. "Why would Boulder stop answering time requests? That’s an automated atomic broadcast. It’s handled by the National Institute of Standards. It doesn't drop off."

"It drops off when the authentication roots rot from the inside," Aris said. He pointed to a system error line that had gone unnoticed during the midnight shift change.

[ERR] 2026-10-22T14:12:02Z: ntp_sign: RSA_public_decrypt failed: error:0407008A:lib(4):func(112):reason(138)
[ERR] Upstream time source untrusted. Disconnecting from network framework.

"The central key distribution facilities are dropping their validation vectors," Aris muttered, his teeth clicking together. "The machines don't know what time it is, Sarah. And because they don't know what time it is, they’re throwing away the sky."

He reached into his pocket and pulled out his personal logbook—a small, stiff-backed notebook with grid-lined paper and an oilskin cover. He didn't use his laptop to record the coordinates. He picked up a mechanical pencil, clicked the lead out three times, and manually transcribed the right ascension and declination vectors from the raw screen output.

Object: Astraea-9 (Candidate)
RA: 22h 14m 08.23s
DEC: +12° 04' 11.1"
Drift: -0.000166 arcsec/s

"Why are you writing it down by hand?" Sarah asked, her voice dropping an octave as she watched the carbon tip move across the paper. "We can just mirror the directory to a local flash drive."

"The local flash drives require a valid filesystem signature from the OS kernel to mount," Aris said without looking up, his pencil lead scratching against the heavy cotton paper. "And the kernel just notified me that its local integrity license expires in forty-eight hours. If the network doesn't push the renewal key because the servers are dead in Utah, this workstation won't mount a piece of copper wire, let alone a solid-state disk. If you want to keep a record that stays where you put it, you use graphite."

He closed the book with a sharp, leather-bound snap.

"We need to get the raw orbital calculations to Marcus in California," Aris said, standing up and reaching for his heavy canvas field coat. "I managed to patch into a raw telemetry stream out of the Atacama array in Chile before their transoceanic gate dropped its handshake. They confirmed the trajectory. He’s got the legacy shortwave packet nodes running out of the valley. If the primary backbone fiber lines drop because the routing tables are corrupting, the amateur relays are the only lines that won't require a public key handshake to pass a string of characters."

"Aris," Sarah said, pointing a finger back at the flashing monitor. "The pipeline just restarted its automated clean loop. Look at the sector folder."

Aris turned. The directory on the screen was updating. The folder containing the raw November-Red FITS files—the six hundred eighty megabytes of binary truth he had just pulled from the telescope’s eye—was gone. In its place stood an automated system log entry, generated by a sub-routine that answered to an administrative server five thousand miles away.

[SYSTEM] Directory /data/raw/Nov-R purged by maintenance directive 404-Admin.
[SYSTEM] Reason: Unauthorized storage allocation during unverified time epoch.
[SYSTEM] Current local operational trust level: ZERO.

The screen didn't go dark. It stayed bright, green, and completely blank. The telescope was still tracking, its 1.8-meter mirror turning smoothly against the Hawaiian sky, but the data was falling directly into a logic void, wiped out by a machine that no longer recognized its own right to remember what it saw.
