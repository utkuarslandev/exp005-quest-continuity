# Exp005 Quest CloudXR direct-control client

This repository contains the compiled static Quest client for the Exp005
robot-disabled live transport gates. The runtime bytes were built from the
accepted offline implementation commit recorded in `deployment.json`.

The page combines:

- NVIDIA CloudXR WebXR video and headset tracking;
- independent six-digit bootstrap pairing over secure WebSocket;
- an unordered, zero-retransmit WebRTC `poses` data channel carrying QDC1
  controller frames; and
- bounded HUD diagnostics for buffered-frame drops, forwarding drops, and
  reconnect attempts.

The published endpoint is the reviewed public Brev gateway mapping compiled
into the client. Pairing codes, session tickets, nonces, SDP, ICE candidates,
TURN credentials, and private network mappings are not stored in this
repository.

Robot authority is false. Publication does not establish a physical
Quest-to-Brev RTC pass, CloudXR coexistence pass, server-ghost pass, or Franka
authority. Those gates remain pending under the governing Exp005 plan.

Build provenance and safety boundaries are in `deployment.json`; exact runtime
hashes are in `runtime-files.sha256`. NVIDIA and third-party terms are retained
in `NOTICE.md`, `THIRD_PARTY_NOTICES.md`, the emitted bundle notice files, and
`LICENSES/`.
