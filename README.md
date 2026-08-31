# Awesome Microduck 🦆

Community-built software, simulations, tools, and hardware work for Pollen
Robotics' [Microduck](https://pollen-robotics.com/microduck/).

## Contents

- [Community software & integrations](#community-software--integrations)
- [Simulation & policy research](#simulation--policy-research)
- [Demos & applications](#demos--applications)
- [Hardware & fabrication](#hardware--fabrication)
- [Upstream reference](#upstream-reference)
- [Contributing](#contributing)

## Community software & integrations

- [DuckKit](https://github.com/craigm26/duckkit) — Pure Swift Microduck runtime and simulation package with policy loading, kinematics, protocol types, and Linux tests.
- [Embodied Agent](https://github.com/mjschock/embodied-agent) — Simulation-first multi-robot agent platform with a Microduck MuJoCo/ONNX adapter and semantic skill API.
- [Meckie Duck Gateway](https://github.com/rangerchaz/meckie-duck-gateway) — Small HTTP gateway and hardware-free protocol double for experimenting with Microduck control from scripts, agents, or home automation.
- [Microduck MCP](https://github.com/aj-dev-smith/microduck-mcp) — MCP server and CPU MuJoCo simulator exposing Microduck intents, sensing, tricks, camera frames, and agent-facing tools.
- [Microduck Miniverse](https://github.com/DollhouseRobotics/microduck-miniverse) — Repackages Pollen's nine official ONNX policies into validated, checksummed deterministic Miniverse simulation bundles.
- [Microduck Policy Golden Vectors](https://huggingface.co/datasets/craigm26/microduck-policy-golden-vectors) — SHA256-pinned golden observation→action vectors recorded from the official policies for conformance-testing custom Microduck runners.
- [Microduck Prototype Suite](https://github.com/apirrone/microduck_app) — Prototype modules from Open Duck Mini's creator: a PWA companion app, head-petting audio CNN, procedural voice synth, and ToF-SLAM/forward-kinematics Rust crates; the shared runtime is currently unavailable.
- [Microduck Runtime (legacy)](https://github.com/TommyZihao/microduck_runtime) — Community Raspberry Pi runtime with standing body-pose controls for Z height, pitch, and roll; exploratory and separate from Pollen's current runtime.
- [OpenCastor — Microduck](https://docs.opencastor.com/robots/microduck/) — Third-party OpenCastor integration that discovers Microducks, sends intent commands through `robotd`, and composes routines.
- [quackd](https://github.com/rokbenko/quackd) — LLM goal-planning layer with a bundled simulator, `.duck` task files, safety rules, and MCP support.
- [Strands Robots — Microduck](https://strands-labs.github.io/robots/policies/microduck/) — Third-party Python/MuJoCo provider for running Pollen Microduck policies through a common simulation and hardware interface.
- [uDuck Registry](https://uduck-registry.pages.dev/) — Community catalog of Microduck policy descriptors and artifact links.

## Simulation & policy research

- [autoduck](https://github.com/jakespringer/autoduck) — AI-assisted hill-climbing loop for training Microduck policies, with checkpoint montages and preserved experiment results.
- [Isaac Lab Microduck port](https://github.com/5usu/IsaacLab/blob/5usu/microduck-port/source/isaaclab_microduck/docs/README.md) — Isaac Lab extension with Microduck assets, BAM/backlash actuator models, RSL-RL tasks, and PhysX validation; simulation/training only.
- [Microduck Backflip](https://github.com/Lulzx/microduck-backflip/blob/main/docs/backflip.md) — Reproducible `mjlab` backflip task with a standing-only evaluation battery, experiment log, and explicit safety gates; simulation work, not a hardware claim.
- [Microduck Courier](https://github.com/selinayfilizp/microduck-courier) — MuJoCo apartment-delivery task with a trained policy, rollout artifacts, and telemetry.
- [Microduck Electric Slide](https://huggingface.co/datasets/Histochemichael/microduck-electric-slide-motion) — Choreography project pairing a retargeted Electric Slide motion dataset with a now-public trained command policy, QC tables, and 25-duck MuJoCo show validation.
- [Microduck Isaac Lab port](https://github.com/kabilankb/isaaclab-microduck) — Isaac Lab 3.0 port of Microduck RL tasks (locomotion, ball kick, two-duck rally) A/B-tested against the mjlab baseline.
- [Microduck Lab](https://github.com/jvpflum/microduck-lab) — DGX Spark workspace around the official training source with smoke tests, policy evaluation, and a local policy-bench workflow.
- [Microduck RL Lab](https://github.com/AlexandreEDMOND/microduck-rl-lab) — Retrains five official Microduck skills and composes them into a single automatic MuJoCo obstacle course.
- [Microduck RL on Genesis](https://github.com/Macmachi/microduck-rl-genesis) — Genesis port of the Microduck walking task for AMD/ROCm systems with committed flat, rough-terrain, and backlash ONNX policies; Genesis–MuJoCo validation is documented, but no physical-robot validation.
- [microduck_sim](https://github.com/lgtkgtv/microduck_sim) — Self-contained educational workspace with custom PPO training, ONNX export, and a six-phase Microduck curriculum.
- [Microduck Sidekick Dance](https://github.com/pezzonovante7/microduck-sidekick-dance) — Drop-in mjlab reward task for a lateral side-kick dance; task and training scaffold only, not a trained policy.
- [Microduck Step-Up + Head-Brake Recovery](https://github.com/bihaokun/microduck-step-up-policy) — Simulation-validated ONNX policy pair for a 25 mm step-up with head-brake recovery; hardware-unvalidated.
- [MJX Microduck](https://github.com/APX103/mjx_microduck) — From-scratch MJX (JAX) and Brax PPO reimplementation of the Microduck training tasks with ONNX export.

## Demos & applications

- [Microduck AR](https://huggingface.co/spaces/multimodalart/microduck-ar) — Community WebXR/AR adaptation of the Microduck simulator with AR placement and ground-pick interaction; it uses Pollen's policies rather than publishing new weights.
- [Gradio Workflow Microduck Lab](https://huggingface.co/spaces/ysharma/gr-workflow-microduck-lab) — Plain-English Microduck routines compiled by an LLM and executed with the nine official policies under real MuJoCo physics.
- [Gradio Workflow Microduck School](https://huggingface.co/spaces/ysharma/gr-workflow-microduck-school) — In-browser cross-entropy-method demo where the duck acquires a goal-navigation skill on top of frozen official policies.
- [Microduck iPhone Simulator](https://github.com/littlejohntj/microduck-sim) — Native Swift/MuJoCo/RealityKit simulator that runs the released policies on-device and includes AR mode.
- [Microduck Jump Playground](https://github.com/Liyucheng1997/318_lab-microduck-simulator) — Fork of the browser simulator with a custom-trained vertical-jump policy and live demo; simulation-only, with no hardware validation.
- [Microduck Models](https://github.com/IronSpiderMan/MicroDuckModels) — Self-contained browser simulator (Three.js, MuJoCo WASM, ONNX Runtime Web) running all nine shipped policies.
- [Microquack](https://github.com/lryain/microquack) — Procedural droid-voice engine and WebAssembly experience for Microduck, built around a reusable Rust core.
- [nottyduck](https://github.com/reachjalil/nottyduck) — Moody desk-companion persona with trained desk gestures, built on an RL training lab atop the official sim-to-real stack.
- [specs-microduck](https://github.com/kgediya/specs-microduck) — Snap Spectacles AR hand-gesture teleoperation bridge for the official Microduck web simulator.

## Hardware & fabrication

- [Microduck Replica](https://github.com/fanhao375/microduck-replica) — Microduck mechanical reconstruction study with assembly drawings, CAD exports, hole analysis, and fabrication notes derived from the public MJCF/STL model.
- [microduck-replica (poboll)](https://github.com/poboll/microduck-replica) — Independent Chinese-language mechanical reconstruction with assembly and exploded drawings, transform-applied CAD exports, and reverse-engineering notes.

## Upstream reference

Pollen's official Microduck software:

- [Microduck browser simulator](https://huggingface.co/spaces/pollen-robotics/microduck-simulator)
- [Microduck GStreamer plugins](https://github.com/pollen-robotics/microduck-gst-plugins) — Official prebuilt aarch64 GStreamer plugins with Rockchip hardware encoders and WebRTC.
- [Microduck RL training source](https://github.com/pollen-robotics/microduck_rl)
- [Microduck runtime](https://github.com/pollen-robotics/microduck)

Browse individual ONNX policies in the [uDuck Registry](https://uduck-registry.pages.dev/). To add one, see the [contribution guide](https://github.com/ob1-s/uduck-registry/blob/main/CONTRIBUTING.md).

## Contributing

See [CONTRIBUTING.md](CONTRIBUTING.md) to add a project.
