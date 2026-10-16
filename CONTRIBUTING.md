# Contributing

Created by: EV  
Authorized by: MM (also known as MO)  
Created on: 2026-10-16  
Updated by: EV  
Update authorized by: MM  
Update recorded on: 2026-10-16, 2:09 PM America/Phoenix (UTC−07:00; supplied by MM)

Help make Luxul/OpenWrt research useful to other owners. Small corrections, negative results, sanitized logs, and clearly scoped questions are welcome through issues and pull requests.

## Evidence first

Use one of these labels for every technical finding:

- **Verified artifact:** supported by an inspectable artifact, with its revision or hash.
- **Reported observation:** stated by a contributor, but original evidence or independent reproduction is missing.
- **Hypothesis:** an explanation to test, not a measured result.
- **Pending:** work not yet performed or information not yet collected.
- **Independently reproduced:** a separate run supports the claim and includes the procedure, environment, and evidence.

Include device model and hardware revision, firmware runtime identification, source commit, configuration, topology, commands, expected behavior, actual result, and limitations where relevant. Use the [build](logs/templates/build.md) and [test](logs/templates/test.md) templates. Record failures as carefully as successes. Do not invent missing commands or timestamps.

## Review checklist

1. Explain the problem and scope; link related records.
2. Check relative documentation links and units.
3. Separate raw measurements from conclusions; identify missing controls.
4. Inspect every attachment and diff for secrets and identifying data.
5. Include only material you have permission to redistribute.

Use placeholders in examples. Never upload complete router backups, passwords, private keys, tokens, VPN secrets, customer topology, MAC addresses, serial numbers, or proprietary images. Review logs manually; ignore rules are only a first layer.

Build scripts, patches, device trees, and flash/recovery procedures need an identified source, licensing, exact device applicability, and validation evidence before being presented as working instructions. No validated procedure exists in this initial documentation.

Licensing is [pending maintainer selection](docs/licensing.md). Agree on applicable licensing before contributing substantive code or redistributable assets. Do not assume public visibility grants a license.

## Attribution and naming

Follow [attribution and naming conventions](docs/attribution-and-naming.md) for every new file, folder and update. Preserve creator identity, record the authorizer, and include the change date/time and timezone. EV is the assistant; MM (MO) is the maintainer. Template attribution must be replaced when recording an actual run.
