# ABR-4500 networking findings

Created by: EV  
Authorized by: MM (also known as MO)  
Created on: 2026-10-16  
Updated by: EV  
Update authorized by: MM  
Update recorded on: 2026-10-16, 2:09 PM America/Phoenix (UTC−07:00; supplied by MM)

## Historical report

Evidence level: **reported observation**, not independently reproduced.

| Observation | Available detail | Missing evidence |
| --- | --- | --- |
| NAT forwarding | 645–649 Mbps | Test tool/version, protocol, direction, streams, duration, repeats, raw output |
| CPU | High softirq CPU during forwarding | Per-core utilization, exact percentages, sampling method |
| Earlier link fault | Faulty cable and FCS errors reported | Interface identity, counter values/deltas, cable substitution and retest transcript |

Source: [provenance](../provenance.md). Hardware-test date and exact topology are unknown. The report is associated with ABR-4500; the requested runtime label is 25.12.5, but per-run firmware identity has not been captured.

Do not describe 645–649 Mbps as an average, a guaranteed ceiling, or an offload-disabled baseline. It is the reported range; the number of runs and offload state are unknown. Do not assert the faulty cable was definitively cleared during these specific measurements.

High softirq CPU is consistent with packet-processing pressure, but does not prove the bottleneck. FCS errors identify a link-integrity symptom; the reported cable fault needs controlled before/after evidence to establish causality.

## Repeat-test protocol (proposed; not executed)

1. Use an isolated test network with an external wired traffic endpoint on each side of the router. Record port roles, link speed/duplex, MTU, and a sanitized topology. Avoid running the traffic endpoint on the router when measuring forwarding.
2. Identify device revision, runtime/build, image hash, relevant driver versions, firewall/NAT settings, and enabled services. Record software and hardware flow-offload settings separately; do not assume either is supported or active.
3. Verify endpoint and direct-link capacity. Use known-good cables; capture FCS/error counters before and after each run, with the exact interface and counter source.
4. Specify tool/version and exact client/server commands, protocol, direction, duration, parallel streams and payload settings. Keep endpoints and parameters consistent across comparisons.
5. Record repeated runs in each direction with throughput, loss/retransmissions where available, per-core CPU including softirq, and counter deltas. Preserve units and individual outputs.
6. Compare baseline and supported offload configurations one change at a time. Verify the setting took effect and that forwarding/NAT and firewall behavior remain correct. Record unsupported or failed attempts.
7. Save sanitized outputs with the [test template](../../logs/templates/test.md), explicitly marking uncontrolled factors and conclusions.

Pending: establish a clean-cable baseline; quantify CPU behavior; compare offload modes; check sustained stability, latency under load, and correctness. No new hardware testing was performed for this import.
