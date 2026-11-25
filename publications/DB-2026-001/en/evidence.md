# DB-2026-001 — public evidence matrix

This matrix is a redacted index of findings from the research documentation, not a collection of raw evidence. Sources remain in the private archive. Samples and raw logs were not reanalysed during editing.

| ID | Finding | Status and limitation | Sources |
| --- | --- | --- | --- |
| E01 | Cloudflare changes on 8 November; two runs on 9 November. | CONFIRMED; causal relationship undetermined. | H1a, H2 |
| E02 | Distinct historical chain and ZIP of 58,109,740 B. | CONFIRMED | H1a, H2, S12 |
| E03 | Two probable transfer attempts. | PROBABLE; receipt UNKNOWN. | H1a, H2 |
| E04 | Identification of Stage 1 and recovery of Stage 2. | CONFIRMED statically. | S12 |
| E05 | Stage 2 includes communication and file preparation. | CONFIRMED statically; telemetry role PROBABLE. | S12 |
| E06 | Mach-O of 5,218,432 B obtained directly. | CONFIRMED; equivalence to complete chain UNKNOWN. | S3, M2, M3 |
| E07 | API resolver, 48/53 hashes, environmental checks. | CONFIRMED statically; complete runtime behaviour UNKNOWN. | S3 |
| E08 | Nine x86_64 configuration entries verified. | CONFIRMED reconstruction; full mapping UNKNOWN. | S3 |
| E09 | Two compiled OSA buffers recovered. | CONFIRMED statically; full dispatch UNKNOWN. | S3 |
| E10 | Code encompasses collection and communication. | CONFIRMED statically; Stage 4 execution UNKNOWN. | S3, AUTH |
| E11 | Run 1: collection, archiving, POST attempts. | CONFIRMED; ZIP contents and termination UNKNOWN. | R1 |
| E12 | Collection before successful password validation. | CONFIRMED in Runs 1–2. | R1, R2 |
| E13 | Run 2: separate state artefact. | CONFIRMED write; consumer UNKNOWN. | R2, POST, AUTH |
| E14 | Static credential validation path. | CONFIRMED structure; detailed interpretation PROBABLE. | AUTH |
| E15 | Run 2: two failed checks and one successful check, artefact written. | CONFIRMED; ordering within the second UNKNOWN. | R2, POST, AUTH |
| E16 | Dialogue and AppleEvents/TCC events. | Dialogue PROBABLE; events CONFIRMED. | R2, N |
| E17 | Residual profile artefacts after Run 2; no active sample in the inspected window. | CONFIRMED within inspection scope; full persistence status UNKNOWN. | POST |
| E18 | Run 3: artefact read and successful check; matching copy hashes. | CONFIRMED traces; reuse PROBABLE. | R3, AUD, M2, M3, N |
| E19 | Matching metadata of two credential artefacts; path present in ZIP. | CONFIRMED; direct flow UNKNOWN. | M3, AUD |
| E20 | Copies of selected stores and configurations in Run 2. | CONFIRMED documented writes; complete ZIP UNKNOWN. | R2 |
| E21 | Notes with WAL/SHM and other files preserved in Run 3. | CONFIRMED files; record state UNKNOWN. | M3, AUD |
| E22 | 6/16 markers found. | CONFIRMED search result; access to objects UNKNOWN. | R3, AUD, N |
| E23 | Three Run 3 archiving operations and clean-up. | CONFIRMED; earlier ZIPs UNKNOWN. | R3, AUD |
| E24 | ZIP 289,526 B, CRC PASS, 61 paths; 38 matching files, 2 metadata differences, 21 AppleDouble entries. | CONFIRMED comparison; cause of differences PROBABLE. | R3, AUD, M3 |
| E25 | Run 1–2 network attempts; 59/124 SYN packets without TCP establishment for observed destination. | CONFIRMED within PCAP scope. | R1, R2, S3 |
| E26 | WAN disconnection according to operator; traffic consistent with isolation. | CONFIRMED documented configuration; open-network behaviour UNKNOWN. | N, R1, R2, M3 |
| E27 | Integrity checks 41/42, 43/43, 44/44 and 90/90. | CONFIRMED according to reports; does not establish completeness. | R1, R2, M2, R3, M3, AUD |
| E28 | Infostealer-class behaviour; heuristic suggesting AMOS. | CONFIRMED class; feature similarity PROBABLE; attribution UNKNOWN. | S3, R1, R2, AUD, H1a, H2 |

## Internal source index (public descriptions)

| ID | Scope |
| --- | --- |
| S12 | Static analysis of Stages 1 and 2, identifiers and historical comparison. |
| S3 / S3A | Current and earlier revisions of Stage 3 static analysis. |
| R1 | Run 1 forensic report. |
| R2 | Run 2 forensic report. |
| M2 | Manifest of the wider Run 2 set. |
| POST | Post-Run 2 host inspection. |
| AUTH | Static analysis of the authentication path. |
| R3 | Run 3 offline analysis. |
| M3 | Run 3 manifest. |
| AUD | Final Run 3 comparative audit. |
| H1a / H1b | Two revisions of the 9 November incident report. |
| H2 | Historical post-compromise audit. |
| N | Project journal, §§1–37. |

We do not publish credential values, their hashes, private archive addresses or detailed user paths.

[Polish evidence matrix](../evidence/README.md) · [Report](report.md)
