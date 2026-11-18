# Awesome 3D Animation & Motion Retargeting [![Awesome](https://awesome.re/badge.svg)](https://awesome.re)

> A curated list of top tools, AI models, libraries, and SaaS platforms for **3D character animation**, **markerless motion capture (mocap)**, **skeletal auto-rigging**, and **motion retargeting** across Blender, Unreal Engine, Unity, and Godot.

[![GitHub stars](https://img.shields.io/github/stars/ishandutta2007/Awesome-3D-Animation-Motion-Retargeting?style=flat-square)](https://github.com/ishandutta2007/Awesome-3D-Animation-Motion-Retargeting/stargazers)
[![GitHub forks](https://img.shields.io/github/forks/ishandutta2007/Awesome-3D-Animation-Motion-Retargeting?style=flat-square)](https://github.com/ishandutta2007/Awesome-3D-Animation-Motion-Retargeting/network/members)
[![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg?style=flat-square)](https://github.com/ishandutta2007/Awesome-3D-Animation-Motion-Retargeting/blob/main/README.md#contributing)
[![License: CC0-1.0](https://img.shields.io/badge/License-CC0_1.0-lightgrey.svg?style=flat-square)](https://creativecommons.org/publicdomain/zero/1.0/)

---

## Overview

This repository tracks the leading **open-source tools** and **SaaS platforms** for **3D animation and motion retargeting**. Whether you are building an indie game, producing VTuber animations, or developing next-generation VFX pipelines, these tools extract humanoid and quadruped motion from video, sensors, or text prompts, retarget animations between disparate skeletal rigs (Mixamo, Rigify, UE5 Mannequin, VRM, SMPL-X), and export clean, production-ready assets.

### Key Use Cases & Keywords
- **Video-to-Motion Capture (Mocap):** Markerless single and multi-camera tracking using computer vision and deep learning.
- **Skeletal Auto-Rigging:** Automatic bone placement, weighting, and skinning for humanoid and non-humanoid meshes.
- **Motion Retargeting:** Cross-skeleton animation mapping (e.g., Mixamo to Unreal Engine 5 or Blender Rigify).
- **Text-to-Motion Synthesis:** Generative AI diffusion models for generating 3D skeletal animations from natural language prompts.
- **Physics-Assisted Animation:** Trajectory optimization, secondary motion simulation, and foot contact stabilization.

---

## Table of Contents

- [SaaS & Hosted Platforms](#saas--hosted-platforms)
- [Open-Source GitHub Projects](#open-source-github-projects)
  - [Blender Add-ons & Local Mocap Tools](#blender-add-ons--local-mocap-tools)
  - [Markerless Mocap Systems & Biomechanics](#markerless-mocap-systems--biomechanics)
  - [Text-to-Motion & Generative AI Models](#text-to-motion--generative-ai-models)
  - [Robotics & Cross-Embodiment Retargeting](#robotics--cross-embodiment-retargeting)
  - [Live Streaming, VTubing & Face Tracking](#live-streaming-vtubing--face-tracking)
  - [Game Engine Native Retargeting Suites](#game-engine-native-retargeting-suites)
- [Recommended Production Pipelines](#recommended-production-pipelines)
- [Contributing](#contributing)
- [Disclaimer & Licensing Notice](#disclaimer--licensing-notice)

---

## SaaS & Hosted Platforms

The following hosted solutions provide cloud-based AI motion capture, automated rigging, character emote generation, and cloud retargeting libraries:

| Platform | Primary Focus / Capabilities | Pricing Model | Free Tier Limits |
| :--- | :--- | :--- | :--- |
| **[Adobe Mixamo](https://mixamo.com)** | Automatic humanoid auto-rigging and royalty-free mocap animation library. | Free | 100% free with Adobe ID; unlimited character auto-rigging & animation downloads for personal and commercial projects. |
| **[DeepMotion](https://deepmotion.com)** | Cloud AI markerless mocap from standard 2D video (full-body, hands, face, and physics). | Freemium (Credit-based, paid tiers from ~$15/mo) | Free tier includes ~60 animation credits/month for personal non-commercial testing. |
| **[Plask](https://plask.ai)** | Browser-based AI motion capture, 3D keyframe cleanup, and bone retargeting editor. | Freemium (Paid plans from ~$18/mo) | Free plan includes ~15 seconds of daily AI mocap and 1 GB cloud storage. |
| **[Cascadeur](https://cascadeur.com)** | Physics-assisted 3D keyframe animation software with AutoPosing and trajectory control. | Freemium (Indie from ~$8-$19/mo, Pro ~$49/mo) | Free plan available with full animation toolset; export limitations apply for non-commercial evaluation. |
| **[Rokoko Studio](https://rokoko.com)** | Hardware mocap recording, smart suit integration, and Rokoko Vision AI video tracking. | Freemium (Paid tiers like Plus/Pro from ~$20+/mo) | Free Starter plan ($0 forever) includes unlimited FBX/BVH exports and ~30 seconds/month of Rokoko Vision AI. |
| **[Move.ai](https://move.ai)** | Single-camera (Move One iOS) and multi-camera studio markerless AI mocap. | Freemium (Move One from ~$15-$18/mo; API & Genesis custom) | Free trial / preview access on Move One iOS app with limited processing credits. |
| **[Autodesk Flow Studio](https://wonderdynamics.com)** | Cloud AI VFX tool replacing actors in live-action footage with rigged 3D CG characters. | Freemium (Lite starting around $10/mo, scaling to Pro) | Free plan includes ~300 monthly credits (watermarked 720p output, limited storage). |
| **[Reallusion ActorCore](https://reallusion.com)** | AAA mocap animations, AccuRIG auto-rigging tool, and multi-format retargeting. | Freemium / Pay-per-asset (Flex plans from ~$29/mo) | Permanent free section with 3 rigged 3D characters, ~32 mocap animations, and free AccuRIG desktop software. |
| **[Anything World](https://anything.world)** | AI-driven 3D model generation, automated rigging, and runtime character animation. | Freemium (Nano at $30/mo, Micro at $60/mo) | Free Individual plan ($0/mo) includes ~15-20 monthly credits for personal/student use. |
| **[Kinetix](https://kinetix.tech)** | Generative AI 3D emote SDK and developer integrations for virtual worlds and games. | Developer / Enterprise Custom Pricing | Contact sales; occasional free developer preview quotas through gaming platform partners. |

---

## Open-Source GitHub Projects

### Blender Add-ons & Local Mocap Tools

- **[MaxLiu22/Motion2MixamoRig](https://github.com/MaxLiu22/Motion2MixamoRig)** - Open-source Python and Blender 4.2+ extension that extracts human motion from video or photos and automatically retargets it onto Adobe Mixamo-rigged characters (`Apache-2.0`).
- **[BlendCap](https://github.com/Arcomade/BlendCap)** - Offline single-video performance capture add-on for Blender with body, hand, and facial tracking, foot grounding cleanup, and retargeting presets for Rigify, Auto-Rig Pro, CloudRig, and Mixamo (`GPL-3.0`).
- **[toyxyz-blender-retargeter](https://github.com/toyxyz/toyxyz-blender-retargeter)** - Open-source Blender add-on for skeletal motion retargeting featuring automatic bone matching, reusable JSON presets, reference pose editing, and foot contact stabilization (`MIT`).
- **[Open Mocap for Blender](https://github.com/Larenju-Rai/open-mocap-blender)** - Offline open-source Blender add-on utilizing MediaPipe and OpenCV for real-time and recorded full-body and hand pose tracking (`MIT`).
- **[ioxandrii/blender_mocap](https://github.com/ioxandrii/blender_mocap)** - Lightweight Blender CLI utility script for batch retargeting BVH motion capture data onto Mixamo-style FBX armatures while preserving skin weights (`MIT`).
- **[VRM Add-on for Blender](https://github.com/saturday06/VRM-Addon-for-Blender)** - Open-source Blender extension for importing, rigging, bone-mapping humanoid armatures, and exporting VRM 3D avatars (`MIT`).
- **[Rokoko Studio Live Blender Plugin](https://github.com/Rokoko/rokoko-studio-live-blender)** - Official open-source Blender plugin for live motion capture streaming and custom skeletal bone-mapping directly inside Blender viewport (`GPL-3.0`).

### Markerless Mocap Systems & Biomechanics

- **[FreeMoCap](https://github.com/freemocap/freemocap)** - Free, hardware-agnostic open-source multi-camera markerless motion capture system bringing research-grade 3D tracking to indie creators and research labs (`AGPL-3.0`).
- **[Pose2Sim](https://github.com/perfanalytics/pose2sim)** - Open-source Python package for markerless kinematics that triangulates 2D human poses from calibrated multi-camera video into 3D OpenSim biomechanical skeletal models (`Apache-2.0`).
- **[OpenCap](https://github.com/stanfordnmbl/opencap-core)** - Stanford open-source software pipeline computing 3D kinematics and joint dynamics from two or more smartphone video feeds (`Apache-2.0`).
- **[MoCap Anything](https://github.com)** - Universal video-to-3D motion capture framework extracting and retargeting joint rotations onto humans, animals, creatures, and arbitrary custom rigs (`MIT`).

### Text-to-Motion & Generative AI Models

- **[HyMotion (Tencent Hunyuan)](https://github.com)** - Open-source 3D character animation model using Diffusion Transformers (DiT) and flow matching to generate natural 3D skeletal motion from text prompts, with ComfyUI and Blender integrations.
- **[HumanML3D](https://github.com/EricGuo5517/HumanML3D)** - Foundational 3D human motion-language dataset and baseline models for text-driven 3D animation generation using SMPL bodies.
- **[MotionDiffuse](https://github.com/mingyuan-zhang/MotionDiffuse)** - First diffusion-based text-driven 3D human motion generation model with cross-skeleton and fine-grained body part control (`MIT`).
- **[Mesh2Motion](https://github.com)** - Open-source web-based 3D auto-rigging and animation generator offering instant humanoid, quadruped, and avian motion sets with GLB export (`MIT`).

### Robotics & Cross-Embodiment Retargeting

- **[NVIDIA SOMA Retargeter](https://github.com/NVIDIA/soma-retargeter)** - Open-source motion retargeting library built on Newton and NVIDIA Warp for converting BVH human motion into humanoid robot joint trajectories using inverse kinematics (IK) and contact stabilization (`Apache-2.0`).
- **[Kimodo (NVIDIA)](https://github.com/nv-tlabs/kimodo)** - Kinematic motion generation model supporting SMPL-X skeletons and General Motion Retargeting (GMR) across diverse digital humans and physical humanoid robots.

### Live Streaming, VTubing & Face Tracking

- **[SysMocap](https://github.com)** - Open-source real-time webcam motion capture and live character retargeting tool supporting VRM, Live2D, and custom 3D avatars (`GPL-3.0`).
- **[OpenSeeFace](https://github.com/emilianavt/OpenSeeFace)** - Robust open-source facial tracker and expression solver streaming blendshape weights to Blender, Unity, and VSeeFace over OSC/UDP (`BSD-2-Clause`).
- **[VSeeFace](https://www.vseeface.net)** - High-performance free VTuber software supporting VRM avatar tracking with expression blending, leap motion hand tracking, and virtual camera export.

### Game Engine Native Retargeting Suites

- **[Blender 4.x](https://www.blender.org)** - Industry-standard 3D creation suite featuring Rigify auto-rigging, Non-Linear Animation (NLA) blending, dynamic constraints, and native bone retargeting tools (`GPL-2.0+`).
- **[Godot Engine 4.x](https://godotengine.org)** - Lightweight open-source game engine featuring built-in runtime `SkeletonProfileHumanoid` mapping, enabling shared humanoid animations across distinct character meshes (`MIT`).
- **[Unreal Engine 5 IK Rig & Retargeter](https://www.unrealengine.com)** - Advanced real-time skeletal retargeting framework with full-body IK (FBIK), chain mapping, and runtime batch retargeting between UE4 Mannequin, UE5 Manny/Quinn, and custom skeletons.

---

## Recommended Production Pipelines

| Goal | Recommended Workflow Stack |
| :--- | :--- |
| **Solo Indie Game Dev** | Video clip ➔ **BlendCap** or **DeepMotion** ➔ Blender (Clean up with **toyxyz-blender-retargeter**) ➔ Export FBX/GLTF to **Godot 4** or **Unity** |
| **Mixamo Rig Compatibility** | Video / Image ➔ **MaxLiu22/Motion2MixamoRig** ➔ Batch apply to Mixamo characters with **ioxandrii/blender_mocap** |
| **High-Precision Multi-Camera Studio** | Synchronized cameras / smartphones ➔ **FreeMoCap** or **Move.ai** ➔ Blender Rigify / UE5 IK Retargeter |
| **Generative Animation from Text** | Natural language prompt ➔ **HyMotion** or **MotionDiffuse** ➔ SMPL / BVH ➔ Unreal Engine 5 or Blender NLA |
| **Live VTuber / Streaming** | Standard Webcam ➔ **OpenSeeFace** + **SysMocap** / **VSeeFace** ➔ OBS Studio virtual camera |

---

## Contributing

Contributions are warmly welcomed! To suggest a tool, add a new library, or fix an outdated entry:

1. **Fork** this repository.
2. Create a new branch (`git checkout -b feature/add-new-tool`).
3. Add the project under the appropriate section following the existing format:
   ```markdown
   - **[Project Name](https://github.com/username/project)** - Descriptive 1-2 sentence overview highlighting key features and target engines (`License`).
   ```
4. If adding a SaaS product, please update the [SaaS & Hosted Platforms table](#saas--hosted-platforms) with accurate pricing and free tier limits.
5. Commit your changes and open a **Pull Request**.

---

## Disclaimer & Licensing Notice

- This curated list is maintained for educational, research, and technical animation purposes.
- Some open-source AI mocap tools utilize academic models (such as SMPL, SMPL-X, or MANO) which carry non-commercial research licensing terms. Always verify model licenses prior to commercial game or film release.
- Self-hosted deep learning mocap models typically require hardware acceleration (NVIDIA CUDA, AMD ROCm, or Apple Metal) for real-time inference.
