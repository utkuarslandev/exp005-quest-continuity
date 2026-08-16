# Exp005 Quest continuity diagnostic

This repository contains only the compiled static artifact for the Exp005
Quest 2 controller-continuity and robot-disabled direct-transport gates.

The page:

- visualizes current WebXR controller poses and analog inputs;
- detects missing and frozen pose updates;
- records a bounded downloadable diagnostic trace;
- optionally connects to an operator-supplied authenticated `wss://` telemetry
  endpoint without storing its token;
- contains no embedded Brev, CloudXR, Isaac Sim, press, or robot endpoint;
- has robot authority permanently disabled.

Build provenance is recorded in `deployment.json`. This repository does not
contain the press-tending project, credentials, experiment evidence, or robot
control source.
