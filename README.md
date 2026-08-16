# Exp005 Quest continuity diagnostic

This repository contains only the compiled static artifact for the Exp005
Quest 2 controller-continuity and robot-disabled direct-transport gates.

The page:

- visualizes current WebXR controller poses and analog inputs;
- detects missing and frozen pose updates;
- records a bounded downloadable diagnostic trace;
- prefills the current non-secret EU `wss://` telemetry endpoint while
  allowing an operator override and remembering only the endpoint;
- never stores its ephemeral authentication token;
- contains no CloudXR, Isaac Sim, press, or robot-control endpoint;
- has robot authority permanently disabled.

Build provenance is recorded in `deployment.json`. This repository does not
contain the press-tending project, credentials, experiment evidence, or robot
control source.
