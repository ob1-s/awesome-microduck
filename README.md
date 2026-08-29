# Awesome MicroDuck 🦆

A small, curated list of community-built software, simulations, tools, and
hardware work for Pollen Robotics' [MicroDuck](https://pollen-robotics.com/microduck/).

> This list is independent of Pollen Robotics. It covers projects built around
> MicroDuck, not a rewritten copy of Pollen's launch material. Official
> software, shipped policies, product features, and generic dependencies are
> linked as upstream references below, not presented as community projects.

**Reviewed:** 2026-08-29

## Contents

- [Community software & integrations](#community-software--integrations)
- [Simulation & policy research](#simulation--policy-research)
- [Demos & applications](#demos--applications)
- [Hardware & fabrication](#hardware--fabrication)
- [Upstream reference](#upstream-reference)
- [Contributing](#contributing)

## Community software & integrations

- [DuckKit](https://github.com/craigm26/duckkit) — Pure Swift MicroDuck runtime and simulation package with policy loading, kinematics, protocol types, and Linux tests.
- [Embodied Agent](https://github.com/mjschock/embodied-agent) — Simulation-first multi-robot agent platform with a MicroDuck MuJoCo/ONNX adapter and semantic skill API.
- [Meckie Duck Gateway](https://github.com/rangerchaz/meckie-duck-gateway) — Small HTTP gateway and hardware-free protocol double for experimenting with MicroDuck control from scripts, agents, or home automation.
- [MicroDuck MCP](https://github.com/aj-dev-smith/microduck-mcp) — MCP server and CPU MuJoCo simulator exposing MicroDuck intents, sensing, tricks, camera frames, and agent-facing tools.
- [MicroDuck Runtime (legacy)](https://github.com/TommyZihao/microduck_runtime/blob/main/README.md) — Legacy community Raspberry Pi runtime with 3-axis body-pose control; exploratory and separate from Pollen's current runtime.
- [OpenCastor — MicroDuck](https://docs.opencastor.com/robots/microduck/) — Third-party runtime integration that discovers MicroDucks, sends intent commands through `robotd`, and composes routines.
- [quackd](https://github.com/rokbenko/quackd) — LLM goal-planning layer with a bundled simulator, `.duck` task files, safety rules, and MCP support.
- [Strands Robots — MicroDuck](https://strands-labs.github.io/robots/policies/microduck/) — Third-party Python/MuJoCo provider for running Pollen MicroDuck policies through a common simulation and hardware interface.
- [uDuck Registry](https://uduck-registry.pages.dev/) — Community catalog of MicroDuck policy descriptors and artifact links.

## Simulation & policy research

- [Isaac Lab MicroDuck port](https://github.com/5usu/IsaacLab/tree/5usu/microduck-port) — IsaacLab extension with MicroDuck assets, BAM/backlash actuator models, RSL-RL tasks, and PhysX validation; simulation/training only.
- [MicroDuck Backflip](https://github.com/Lulzx/microduck-backflip) — Reproducible `mjlab` backflip task with a standing-only evaluation battery, experiment log, and explicit safety gates; simulation work, not a hardware claim.
- [MicroDuck Courier](https://github.com/selinayfilizp/microduck-courier) — MuJoCo apartment-delivery task with a trained policy, rollout artifacts, and telemetry.
- [MicroDuck Lab](https://github.com/jvpflum/microduck-lab) — DGX Spark workspace around the official training source with smoke tests, policy evaluation, and a local policy-bench workflow.
- [MicroDuck RL on Genesis](https://github.com/Macmachi/microduck-rl-genesis) — Genesis port of the MicroDuck walking task for AMD/ROCm systems, with actuator and sim-to-real comparisons documented.
- [Waddle Locomotion](https://github.com/nickoenig37/mjlab_microduck_waddle) — Community `mjlab` training project for experimenting with an alternative MicroDuck gait.

## Demos & applications

- [MicroDuck AR](https://huggingface.co/spaces/multimodalart/microduck-ar) — Community WebXR/AR adaptation of the MicroDuck simulator with AR placement and ground-pick interaction; it uses Pollen's policies rather than publishing new weights.
- [MicroDuck iPhone Simulator](https://github.com/littlejohntj/microduck-sim) — Native Swift/MuJoCo/RealityKit simulator that runs the released policies on-device and includes AR mode.
- [MicroDuck Jump Playground](https://github.com/Liyucheng1997/318_lab-microduck-simulator) — Fork of the browser simulator with a custom-trained vertical-jump policy and live demo.
- [Microquack](https://github.com/lryain/microquack) — Procedural droid-voice engine and WebAssembly experience for MicroDuck, built around a reusable Rust core.

## Hardware & fabrication

- [MicroDuck Replica](https://github.com/fanhao375/microduck-replica) — Chinese/English mechanical reconstruction study with assembly drawings, CAD exports, hole analysis, and fabrication notes derived from the public MJCF/STL model.

## Upstream reference

These are the canonical starting points for the robot and its original release;
they are intentionally not counted as community entries:

- [MicroDuck browser simulator](https://huggingface.co/spaces/pollen-robotics/microduck-simulator)
- [MicroDuck RL training source](https://github.com/pollen-robotics/microduck_rl)
- [MicroDuck runtime](https://github.com/pollen-robotics/microduck)

Individual ONNX policies belong in the uDuck Registry, not in this list.

## Contributing

This list stays intentionally small. Add a project only when it gives people
something concrete to inspect, run, build, or learn today.

See [CONTRIBUTING.md](CONTRIBUTING.md) for submission rules.

Use one line per project:

```markdown
- [Project Name](https://canonical-project-url) — One factual sentence about its MicroDuck-specific value.
```

Good submissions:

- are public and usable or meaningfully inspectable now;
- add clear MicroDuck-specific value;
- link directly to the project, app, dataset, CAD work, or guide;
- disclose when the project is a fork, experimental, simulator-only, or yours;
- are alphabetized within their section and appear only once.

Please do not submit Pollen's official repositories or release features,
generic dependencies, product listings, individual policies, named challenges
without a project behind them, profile/invite links, or forks with no meaningful
change. If a project moves or disappears, update or remove its entry.

Open a PR with the one-line addition and click the link before submitting.
