# Security

Created by: EV  
Authorized by: MM (also known as MO)  
Created on: 2026-10-16  
Updated by: EV  
Update authorized by: MM  
Update recorded on: 2026-10-16, 2:09 PM America/Phoenix (UTC−07:00; supplied by MM)

## Project status

This repository is community research documentation. There are no maintained firmware releases or declared supported firmware versions in this repository. Reported runtime labels do not establish security support.

## Reporting a vulnerability or exposed secret

Do not put exploit details, credentials, configuration dumps, or sensitive network information in public issues.

If GitHub shows a private vulnerability reporting option under this repository's Security tab, use it. Availability has not been verified. If it is unavailable, open a minimal public issue requesting a private contact method, without sensitive details. No private email address or response-time commitment is established here.

For an exposed credential, revoke or rotate it immediately through its provider. Deleting a file in a later commit does not remove it from history. Notify maintainers without reposting the secret so they can assess history cleanup.

## Handling evidence

Share the smallest sanitized text excerpt needed. Remove passwords, tokens, keys, device identifiers, public addresses tied to deployments, customer names, and sensitive topology. Keep original backups offline and private. Do not upload proprietary firmware or device-unique factory/calibration partitions.

Security updates, upstream support, image provenance, and recovery behavior require verification before production use.
