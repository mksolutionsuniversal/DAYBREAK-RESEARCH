# Defensive indicators — DB-2026-001

[English CSV](IOC.csv) · [English JSON](IOC.json) · [Original Polish data](../indicators/README.md) · [Report](report.md)

The 17 indicators comprise 4 SHA-256 hashes, 12 domains and 1 IPv4 address. Domains and the IP address are defanged. The campaign/historical distinction separates research conducted on 18–21 November from the incident on 8–9 November 2026.

`research_window` indicates the documented research period, not established first_seen/last_seen dates for infrastructure activity. `confidence` applies to the described role and basis of observation, not attribution to a person or malware family. Static indicators do not establish a successful connection; observed attempts do not establish receipt of data. Malicious infrastructure availability was not checked and no connections to it were made during editing. Do not automatically treat every value as a current blocklist entry.

English CSV and JSON contain the same records; only the descriptive text has been translated from the Polish dataset. Values are derived from the report and evidence matrix, not renewed sample acquisition.
