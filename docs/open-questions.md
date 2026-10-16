# Open questions and cautions

## Priority evidence gaps

- Can runtime identification and source/image hashes substantiate 25.12.5 on ABR-4500 and 25.12.2 on XWC-1000? Are these upstream labels, custom labels, or another provenance?
- What exact source target, feeds, patches, configuration and host reproduce each image?
- What are the hardware revisions, flash layouts, console specifications and validated recovery paths?
- What topology and traffic settings produced 645–649 Mbps? Were the error counters clean during those runs?
- Does high softirq CPU correlate with per-core saturation or another limit?
- Is software or hardware flow offloading supported, active and correct? What changes in controlled comparisons?
- Which XWC-1000 functions actually work, and under which image?
- What long-duration stability, latency, security-update and firewall-correctness tests remain?
- What license should apply to original documentation and future code?

## Cautions

Do not infer upstream support, security maintenance, image compatibility or recovery steps from a version or model name. Flashing may render a device unusable; validate device-specific recovery first.

Cable faults and FCS errors can confound throughput conclusions. Keep physical-layer validation separate from CPU/offload hypotheses and preserve both successful and failed tests.

Raw backups and factory data can expose secrets or unique device information. Publish minimal sanitized evidence and keep proprietary binaries out of this repository.
