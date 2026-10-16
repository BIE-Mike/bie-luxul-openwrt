# Luxul OpenWrt community research

Created by: Original README author retained in Git history; documentation expansion by EV  
Authorized by: MM (also known as MO)  
Created on: 2026-10-16 (original README and EV expansion; see Git history)  
Updated by: EV  
Update authorized by: MM  
Update recorded on: 2026-10-16, 2:09 PM America/Phoenix (UTC−07:00; supplied by MM)

Community documentation and development records for Luxul networking hardware running OpenWrt. The goal is to make findings reviewable, preserve failed experiments, and help other owners reproduce results.

This is an independent community project; vendor endorsement and upstream device support have not been established here. No firmware download or validated installation procedure is provided.

## Devices and evidence

| Device | Reported OpenWrt label | Current documentation status |
| --- | --- | --- |
| [ABR-4500](devices/abr-4500/README.md) | 25.12.5 | User-reported version and NAT observations; raw evidence pending |
| [XWC-1000](devices/xwc-1000/README.md) | 25.12.2 | User-reported version; build and functional validation pending |

These labels come from the project conversation and current maintainer request. They are not independently verified release, source-tag, image-compatibility, or upstream-support claims.

Reported ABR-4500 NAT forwarding was **645–649 Mbps**, with **high softirq CPU**. A previous faulty cable and FCS errors were also reported. The original commands, counters, topology, and per-run outputs are unavailable in the accessible record. Do not interpret this range as a guaranteed capability or a controlled comparison.

## Start here

- [Current state and evidence levels](docs/current-state.md)
- [Source provenance](docs/provenance.md)
- [Networking findings and repeat-test plan](docs/testing/networking.md)
- [Build evidence requirements](docs/builds/README.md)
- [Build and test records](logs/README.md)
- [Open questions and cautions](docs/open-questions.md)
- [Contributing](CONTRIBUTING.md) and [security reporting](SECURITY.md)
- [Licensing status](docs/licensing.md)

Contributions should separate measured observations, interpretations, and unanswered questions. Add sanitized text evidence, exact source revisions, and repeatable procedures before promoting a report to independently reproduced status.

## Safety and scope

Flashing and recovery remain undocumented and unverified for these units. Do not infer flash layouts, image compatibility, serial voltage, or recovery steps from model names. Establish a device-specific recovery path before any firmware changes. Keep backups private.

Do not commit credentials, complete configuration backups, device-unique calibration data, or proprietary binaries. This repository currently contains documentation only.

## Attribution and update records

See [attribution and naming conventions](docs/attribution-and-naming.md). EV identifies the assistant; MM (also MO) identifies the authorizing maintainer. Metadata is documentary attribution, not a cryptographic signature.
