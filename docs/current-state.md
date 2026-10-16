# Current state

As documented on 2026-10-16; actual hardware-test dates are unknown.

| Item | Evidence level | What is known / missing |
| --- | --- | --- |
| Initial repository | Verified artifact | Initial main commit contains only README; see provenance |
| ABR-4500 / 25.12.5 | Reported observation | Runtime label supplied; runtime output, source revision and image hash missing |
| XWC-1000 / 25.12.2 | Reported observation | Runtime label supplied; runtime output, source revision and image hash missing |
| ABR-4500 NAT forwarding | Reported observation | 645–649 Mbps; raw run outputs, method and settings missing |
| High softirq CPU | Reported observation | Qualitative observation; per-core samples and percentages missing |
| Earlier faulty cable / FCS errors | Reported observation | Historical fault; exact counter deltas and retest sequence missing |
| CPU/softirq limits forwarding | Hypothesis | Needs controlled profiling and repeats |
| Flow offloading | Pending | Configuration and comparative results not established |
| Reproducible firmware build | Pending | Source, feeds, config, patches, host and complete commands needed |
| Flash / recovery procedure | Pending | Device-specific validation needed |
| Upstream support / release-label authenticity | Pending | No independent verification included |

“Verified artifact” describes only the particular artifact inspected. No device performance claim is independently reproduced by this documentation import.

See [provenance](provenance.md), [network results](testing/networking.md), and [open questions](open-questions.md).
