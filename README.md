# Awesome MicroDuck 🦆

A curated list of awesome MicroDuck projects, games, tools, and hardware mods — for the 25 cm open-source biped from [Pollen Robotics](https://pollen-robotics.com/microduck).

> MicroDuck is a ~800 g, 25 cm biped with 15 servos, camera + LiDAR + 2 IMUs, running a 50 Hz control loop from ONNX policies trained in [microduck_rl](https://github.com/pollen-robotics/microduck_rl) (MuJoCo Warp + PPO, BAM M6). This list is community-maintained and not affiliated with Pollen.

Inspired by the explosion after pre-orders opened Aug 27, 2026 — share what you’re building!

**Contents**

- [Official](#official) · [Games](#games) · [Sim & Tools](#sim--tools) · [VR & Teleop](#vr--teleop) · [Integrations](#integrations) · [Hardware & Custom Parts](#hardware--custom-parts) · [Community Policies](#community-policies) · [Learning](#learning)

---

## Official

- [MicroDuck](https://github.com/pollen-robotics/microduck) — Duck's brain: `robotd` 50 Hz loop, `updaterd`, `padd`, `mediad` WebRTC, on Rockchip RK3566.
- [microduck_rl](https://github.com/pollen-robotics/microduck_rl) — RL training envs (mjlab), PPO, sim2real, `scripts/export.py` ONNX with baked normalizer. 13 tasks (Velocity, VelStand, Roller, Roulade, BallKick…).
- [MicroDuck Simulator](https://huggingface.co/spaces/pollen-robotics/microduck-simulator) — In-browser MuJoCo WASM + onnxruntime-web, multiplayer ghosts via Trystero, switch legs/rollers with `M`.
- [Pollen Discord](https://discord.com/invite/pollen) — #microduck, builds on show, help when a leg does something strange.

## Games

- [Duck Races](https://pollen-robotics.com/microduck) — Community races on flat/rough tracks (Velocity task). Share your time!
- [Roller Glide Challenge](https://github.com/pollen-robotics/microduck_rl#roller) — Downhill slope gliding on `robot_allcollisions_rollers.xml` (5°–15°).
- [Ball Kick Arcade](https://huggingface.co/spaces/pollen-robotics/microduck-simulator) — 70 mm / 15 g ball kicking (`Mjlab-BallKick-Flat-MicroDuck`), ball-blind actor.
- [Roulade Run](https://github.com/pollen-robotics/microduck_rl) — Forward roll over head, land on feet (`Roulade` task).

## Sim & Tools

- [uDuck Registry](https://github.com/ob1-s/uduck-registry) — Community policy index (61-D →14 @50Hz), `pnpm validate` + MuJoCo `sim_verified` CI (private). **Thin index, not a host.**
- [mjlab](https://github.com/mujocolab/mjlab) — MuJoCo Warp training framework behind microduck_rl.
- [microduck_runtime](https://github.com/TommyZihao/microduck_runtime) — Community runtime for `standing_body_control` and custom policies.
- [BAM](https://github.com/Rhoban/bam) — Better Actuator Model (FrictionDRBam) used for XL330.

## VR & Teleop

- [WebRTC Console](https://github.com/pollen-robotics/microduck/blob/main/docs/design/remote-webrtc.md) — `mediad` streams H.264 + `control` datachannel to browser on LAN (`:8080`).
- [WebSocket SDK](https://github.com/pollen-robotics/microduck/blob/main/docs/design/architecture.md#53) — Server-side LLM control: `get_frame` JPEG on demand, no media stack (for agents).
- [Gamepad Cheatsheet](https://github.com/pollen-robotics/microduck/blob/main/docs/robot/cheatsheet.md#gamepad-configd) — Pair a pad, map intents (`G` ground pick, `Y` sit/stand, `R` roulade).
- [ToF Theremin](https://github.com/pollen-robotics/microduck) — Head ToF 8×8 `tof.stream` → head FK, `control` intent.

## Integrations

- [Discord Bot](https://discord.com/invite/pollen) — Post your `uduck submit` PR, get `sim_verified` badge.
- [Hugging Face Jobs](https://github.com/pollen-robotics/microduck_rl/blob/develop/src/mjlab_microduck/hf_jobs.py) — `train_cli.py --hf-jobs` on HF infrastructure.
- [NFC Tags](https://pollen-robotics.com/microduck/press-kit) — 10 tags in packs, Polaroid NFC for behaviors.
- [Chorale](https://github.com/pollen-robotics/microduck) — Each duck gets its own audio identity at first wake.

## Hardware & Custom Parts

- [Roller Pack](https://pollen-robotics.com/microduck) — 2 rollers + ball + laser pointer + NFC, official.
- [Onshape-to-Robot](https://github.com/Rhoban/onshape-to-robot) — MJCF export used for `config_mjcf_*.json` (see `microduck_rl/src/mjlab_microduck/robot/microduck/`).
- [3D Printable Feet](https://github.com/pollen-robotics/microduck/discussions) — Community soles/legs (SOFT/share alike, check CC BY-SA-NC).
- [Spare Motors](https://pollen-robotics.com/microduck) — 3× XL330, 5× cables, dual charger in Maker pack.

## Community Policies

- [Waddle Locomotion](https://github.com/nickoenig37/mjlab_microduck_waddle) — Nick Koenig custom waddle (`registry/behaviors/waddle-locomotion.json`).
- [Standing Body Control](https://github.com/TommyZihao/microduck_runtime) — Tommy Zihao 6-DoF body pose.

## Learning

- [MicroDuck RL AGENTS.md](https://github.com/pollen-robotics/microduck_rl/blob/develop/AGENTS.md) — Env-building workflow + reward design rules.
- [Architecture](https://github.com/pollen-robotics/microduck/blob/main/docs/design/architecture.md) — Daemons, bus, update system.

---

### Contributing

1. One line per entry: `- [Name](link) — One sentence what it does.`
2. Put it in the right category, alphabetical.
3. No self-promo spam — must be usable by others.
4. Open a PR! See [CONTRIBUTING.md](CONTRIBUTING.md).

*Want a policy indexed? Add it to [uDuck Registry](https://uduck-registry.pages.dev/docs/contribute) instead — this list is for *things around* the duck.*

