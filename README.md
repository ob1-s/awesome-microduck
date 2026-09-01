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

- [DuckKit](https://github.com/craigm26/duckkit) — Pure Swift Microduck runtime and deterministic MuJoCo simulation with ONNX policy loading, kinematics, protocol, voice, and choreography support; Linux-tested.
- [Embodied Agent](https://github.com/mjschock/embodied-agent) — Simulation-first multi-robot agent platform with a Microduck MuJoCo/ONNX adapter and semantic skill API.
- [Meckie Duck Gateway](https://github.com/rangerchaz/meckie-duck-gateway) — HTTP gateway for Pollen Microduck's WebRTC/JSON-RPC control with an included hardware-free fake, for scripts, agents, and home automation.
- [Microduck App](https://github.com/apirrone/microduck_app) — Microduck companion PWA with live 3D state, map view, brain/battery HUD, and commands; deployable on a Raspberry Pi and browsable from a phone.
- [Microduck MapLoc](https://github.com/apirrone/microduck_maploc_rs) — Rust 2D ToF submap-SLAM, Monte Carlo relocalization, A* planning, and telemetry streaming for Microduck, with a Python/MuJoCo reference.
- [Microduck MCP](https://github.com/aj-dev-smith/microduck-mcp) — MCP server, CLI, and browser debug UI for a CPU MuJoCo Microduck simulator using Pollen's ONNX policies; exposes intent tools, sensing, camera frames, behavior machines, and policy tooling.
- [Microduck Miniverse](https://github.com/DollhouseRobotics/microduck-miniverse) — Repackages Pollen's nine official ONNX policies into validated, checksummed deterministic Miniverse simulation bundles.
- [Microduck Policy Golden Vectors](https://huggingface.co/datasets/craigm26/microduck-policy-golden-vectors) — SHA256-pinned golden observation→action vectors recorded from the official policies for conformance-testing custom Microduck runners.
- [Microduck Runtime (legacy)](https://github.com/TommyZihao/microduck_runtime) — Legacy community Raspberry Pi Zero 2W runtime for 15 XL330 servos and a BNO055 IMU, with gamepad, ground-pick/fall, and body-pose controls; separate from Pollen's current runtime.
- [OpenCastor — Microduck](https://docs.opencastor.com/robots/microduck/) — Third-party OpenCastor integration that discovers Microducks, sends intent commands through `robotd`, and composes routines.
- [OpenMicroduck](https://github.com/SaberOnGo/open-microduck) — Unofficial English/Chinese Microduck research and reference project covering software architecture, simulation, sim-to-real, hardware research, and reverse engineering; makes no open-hardware claim.
- [quackd](https://github.com/rokbenko/quackd) — LLM goal-planning layer with a bundled simulator, `.duck` task files, safety rules, and MCP support.
- [Strands Robots — Microduck](https://strands-labs.github.io/robots/policies/microduck/) — Third-party Python/MuJoCo provider for running Pollen Microduck policies through a common simulation and hardware interface.
- [uDuck Registry](https://uduckmoves.com/) — Community catalog of Microduck policy descriptors and artifact links.

## Simulation & policy research

- [autoduck](https://github.com/jakespringer/autoduck) — AI-assisted hill-climbing loop for training Microduck policies, with checkpoint montages and preserved experiment results.
- [DuckLab — Microduck Skate Racing](https://github.com/jvpflum/microduck-lab) — Reproducible MuJoCo roller-skating RL lab with race metrics, ONNX policies, and a simulation-only Race5 benchmark.
- [Isaac Lab Microduck port](https://github.com/5usu/IsaacLab/blob/5usu/microduck-port/source/isaaclab_microduck/docs/README.md) — Isaac Lab extension with Microduck assets, BAM/backlash actuator models, RSL-RL tasks, and PhysX validation; simulation/training only.
- [Microduck Backflip](https://github.com/Lulzx/microduck-backflip/blob/main/docs/backflip.md) — Reproducible `mjlab` backflip task with standing-start evaluation, experiment logs, and safety gates; the current cube-to-mat result is assisted in simulation, with no hardware claim.
- [Microduck Courier](https://github.com/selinayfilizp/microduck-courier) — MuJoCo apartment-delivery task with a trained policy, rollout artifacts, and telemetry.
- [Microduck Electric Slide](https://huggingface.co/datasets/Histochemichael/microduck-electric-slide-motion) — Reproducible Electric Slide motion/retargeting dataset with QC and 25-duck MuJoCo validation artifacts; the trained command controller is published separately and is simulation-only.
- [Microduck Isaac Lab port](https://github.com/kabilankb/isaaclab-microduck) — Isaac Lab 3.0/Newton MJWarp port with locomotion, ball-kick, and two-duck tasks; BallKick/BallRally are trained and measured, while locomotion remains a simulation milestone and is not deployable.
- [Microduck Lab — Mac CPU](https://github.com/jonathanhawkins/microduck-lab) — CPU-first Mac/Linux training and browser-viewer workspace for Microduck policy prototyping, with staged trick curricula, backflip experiments, and baked-normalizer ONNX export; simulation-only.
- [Microduck RL on Genesis](https://github.com/Macmachi/microduck-rl-genesis) — Genesis port of the Microduck walking task for AMD/ROCm systems with committed flat, rough-terrain, and backlash ONNX policies; Genesis–MuJoCo validation is documented, but no physical-robot validation.
- [Microduck Sidekick Dance](https://github.com/pezzonovante7/microduck-sidekick-dance) — Drop-in mjlab reward task for a lateral side-kick dance; task and training scaffold only, not a trained policy.
- [Microduck Sim](https://github.com/lgtkgtv/microduck_sim) — Self-contained educational workspace with custom PPO training, ONNX export, and a six-phase Microduck curriculum.
- [Microduck Simulation Playground](https://github.com/x10zyn/microduck-sim-playground) — Lightweight educational Microduck MuJoCo workspace with pinned upstream repositories, scripted pose experiments, CPU checks, and optional ONNX inference; not a learned walking policy.
- [Microduck Skill Playground](https://github.com/AlexandreEDMOND/microduck-rl-lab) — MuJoCo playground built on the official environments; retrains five skills, composes an automatic course, and currently explores an assisted front-salto curriculum.
- [Microduck Step-Up + Head-Brake Recovery](https://github.com/bihaokun/microduck-step-up-policy) — Simulation-validated ONNX policy pair for a 25 mm step-up with head-brake recovery; hardware-unvalidated.
- [MJX Microduck](https://github.com/APX103/mjx_microduck) — From-scratch MJX (JAX) and Brax PPO reimplementation of the Microduck training tasks with ONNX export.

## Demos & applications

- [Microduck Anatomy](https://huggingface.co/spaces/mishig/microduck-anatomy) — Interactive Microduck anatomy viewer with walking motion, staged component focus, and exploded assembly views.
- [Microduck AR](https://huggingface.co/spaces/multimodalart/microduck-ar) — Community WebXR/AR adaptation of the Microduck simulator with AR placement and ground-pick interaction; it uses Pollen's policies rather than publishing new weights.
- [Microduck Flock Band](https://github.com/SAMBAS123/microduck-sandbox) — Community fork of the browser sandbox adding a pentatonic music mode controlled by the duck's movement and actions; it adds no new policies.
- [Microduck iPhone Simulator](https://github.com/littlejohntj/microduck-sim) — Native Swift/MuJoCo/RealityKit simulator that runs the released policies on-device and includes AR mode.
- [Microduck Lab · gr.Workflow](https://huggingface.co/spaces/ysharma/gr-workflow-microduck-lab) — Plain-English routines choreographed by an LLM and executed with all nine shipped Microduck policies under MuJoCo physics.
- [Microduck Models](https://github.com/IronSpiderMan/MicroDuckModels) — Browser simulator rebuilt with Three.js/React Three Fiber, MuJoCo WebAssembly, and ONNX Runtime Web; bundles all nine shipped policies.
- [Microduck Mommy Flock](https://huggingface.co/spaces/oliveirabruno01/microduck-mommy-flock) — Experimental browser demo where a Mommy Microduck guides two ducklings using local simulated sensing and a project-owned high-level policy; simulation-only.
- [Microduck Racer](https://huggingface.co/spaces/Nirav-Madhani/microduck-racer) — Browser racing fork of the Microduck simulator with four independent roller ducks, waypoint checkpoints, laps, and optional uploaded race policies.
- [Microduck RL playground — with Jump!](https://github.com/Liyucheng1997/318_lab-microduck-simulator) — Browser fork of Pollen's simulator with a custom-trained vertical-jump policy and live demo; simulation-only.
- [Microduck ROS 2 + Isaac Sim](https://github.com/osrbot/microduck-ros2-isaac) — ROS 2 Jazzy/RViz description and Isaac Sim integration for the public Microduck model, including an Isaac USD stage and walking-policy tutorial.
- [Microduck School · gr.Workflow](https://huggingface.co/spaces/ysharma/gr-workflow-microduck-school) — Cross-entropy-method demo that learns a goal-navigation controller on top of nine frozen shipped policies; it does not retrain joint-level policies.
- [Microduck Tracking](https://github.com/AlexBodner/microduck-tracking) — Multi-object tracking and target-fetch demo for Microduck in the official MuJoCo simulator, using Roboflow trackers.
- [Microquack](https://github.com/lryain/microquack) — Procedural droid-voice engine and WebAssembly experience for Microduck, built around a reusable Rust core.
- [NottyDuck](https://github.com/reachjalil/nottyduck) — Social-media coach with trained desk gestures, a 3D office mapper, and an RL training/evaluation lab built on Pollen's official sim-to-real stack.
- [specs-microduck](https://github.com/kgediya/specs-microduck) — Snap Spectacles AR hand-gesture controller for Pollen's browser simulator, with a local WebSocket relay, in-lens telemetry, and synthetic gesture tests.

## Hardware & fabrication

- [Microduck 3D Models](https://github.com/boris721/microduck-3d) — Extracted Microduck STL/MJCF bundle with legs and rollers variants, kinematics JSON, and an Onshape reference; derived from public simulator assets.
- [Microduck DIY](https://github.com/ScrapMeta/microduck-diy) — Chinese-language DIY Microduck build archive with printable STL parts and assembly/exploded 3MF files; currently a Day 1 fabrication record, not an official kit.
- [Microduck Replica](https://github.com/fanhao375/microduck-replica) — Third-party Microduck mechanical and electronics reconstruction with assembly drawings, CAD-importable STLs, fastener analysis, and runtime-derived electronics notes; not affiliated with Pollen.

## Upstream reference

Pollen's official Microduck software:

- [Microduck Sandbox](https://huggingface.co/spaces/pollen-robotics/microduck-simulator) — Official in-browser Microduck RL playground using MuJoCo WebAssembly and onnxruntime-web at 50 Hz, with leg and roller variants.
- [Microduck GStreamer plugins](https://github.com/pollen-robotics/microduck-gst-plugins) — Official prebuilt aarch64 GStreamer plugins for Rockchip MPP hardware encoding and gst-plugins-rs WebRTC.
- [Microduck RL](https://github.com/pollen-robotics/microduck_rl) — Official mjlab/MuJoCo Warp PPO training environments with BAM actuator physics, domain randomization, backlash simulation, and ONNX export.
- [Microduck runtime](https://github.com/pollen-robotics/microduck) — Official Rust runtime and onboard software stack for the Microduck robot.

Browse individual ONNX policies in the [uDuck Registry](https://uduckmoves.com/). To add one, see the [contribution guide](https://github.com/ob1-s/uduck-registry/blob/main/CONTRIBUTING.md).

## Contributing

See [CONTRIBUTING.md](CONTRIBUTING.md) to add a project.
