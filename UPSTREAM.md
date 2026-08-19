---
lifecycle: frozen
authority: historical
last_verified: 2026-08-18
supersedes: []
superseded_by: []
---

# Upstream provenance

This directory is a source-vendored derivative of only
`deps/cloudxr/webxr_client` from NVIDIA IsaacTeleop.

- Repository: `https://github.com/NVIDIA/IsaacTeleop`
- Commit: `e075c8f14dcf8b0ec709c4abb1f9f6bf792a9e04`
- Upstream subtree object: `331bbb93f0b7ce8aadbcfb68c7359fd71a7d89ba`
- CloudXR Web SDK: `6.3.0-rc4`
- External CloudXR build input: `vendor/nvidia-cloudxr-6.3.0-rc4.tgz`
- CloudXR package SHA-256: `16267bc8dd4d4d8daf6ec7aa03f99899d955ad5d9ff757854326326a7a44b31c`
- Imported: 2026-08-17

The CloudXR archive is intentionally not tracked. Follow `vendor/README.md` to
retrieve and verify the pinned build input before dependency installation.

The upstream Apache-2.0 license is in
`LICENSES/IsaacTeleop-Apache-2.0.md`. The CloudXR SDK has separate terms in
`LICENSES/NVIDIA-CloudXR-SDK.txt`. Heroicons retain their upstream MIT notice
at `src/icons/HEROICONS_LICENSE`.

Local changes add the Exp005 browser-observable controller capture contract,
the fixed 244-byte `exp005_quest_control_v1` serializer, newest-state WebRTC
delivery, fail-closed disarm behavior, and direct-channel diagnostics. They do
not make CloudXR controller tracking authoritative and do not grant robot
authority by themselves.
