# Reproducible builds: evidence required

Status: **pending** for both devices. No source checkout, build configuration, patch set, feeds lock, commands, or complete successful build log was available for this import. The reported version labels alone are insufficient to reconstruct an image.

This page defines the record needed to publish a reproducible procedure; it is not a tested build recipe.

## Capture a build

1. Identify the exact device and hardware revision, intended image type, and authoritative source repository URL plus full commit SHA.
2. Record host OS/architecture, toolchain/dependency versions, and any container image digest.
3. Preserve target/subtarget/profile, sanitized effective configuration, exact feeds revisions, patch contents/order and licensing.
4. Record every command in order, working directory, environment variables relevant to the build, exit status, and complete sanitized output. Include failed attempts and how they were resolved.
5. Record output filenames, sizes and SHA-256 hashes. Keep proprietary outputs and device-specific contents out of Git.
6. Repeat in a clean environment using the recorded inputs. Compare hashes and explain any differences before claiming byte-for-byte reproducibility.
7. Link a separate device test record matching the output hash. Successful compilation does not prove safe flashing or runtime correctness.

Copy the [build template](../../logs/templates/build.md) into a device-specific log directory when an actual run is performed. Do not fill unknown fields with guessed commands. Recovery and installation require separate validation.
