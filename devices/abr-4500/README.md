# Luxul ABR-4500

## Reported state

- OpenWrt label: **25.12.5** (maintainer-reported; runtime output and source mapping pending).
- NAT forwarding: **645–649 Mbps**, with high softirq CPU.
- An earlier faulty cable and FCS errors were reported.

See the [networking record](../../docs/testing/networking.md) for limitations. These observations do not establish maximum throughput, offload support, or production readiness.

## Device notes to collect

Hardware revision, SoC, RAM, flash capacity and layout, switch/PHY identity, port mapping, bootloader, console voltage/pinout, image format, driver versions, and recovery mechanism are all pending evidence. Do not copy assumptions from similarly named hardware.

Capture sanitized board/runtime identification, boot logs, interface/driver information, and image checksum. Keep full flash backups, factory partitions, identifiers, and credentials private.

Build instructions and flashing steps are intentionally pending. See [build requirements](../../docs/builds/README.md).
