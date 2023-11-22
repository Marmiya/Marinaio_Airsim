# This is a fork from [Colosseum](https://github.com/CodexLabsLLC/Colosseum)

## Here are main changes:

* New eigen3 for c++ 20 compile...
* change some paths in camke module for working as a external lib...
* Notice: Original cmake/cmake-moudules/CommonSetup.cmake has some specific C++ flags that are not suitable for everyone, especially for someone who uses Airsim as an external lib. So I annotated them. If you need them(like when you use Airsim singly), you should undo them.

## How to use it:

1. clone this repository
2. enter and execute the build.cmd/build.sh

TODO:

* deal with [problem](https://zhuanlan.zhihu.com/p/548879226#:~:text=%E5%8F%91%E7%8E%B0%E4%BA%86%E4%B8%80%E4%B8%AAairsim%E8%87%AA%E8%BA%AB%E7%9A%84%E9%97%AE%E9%A2%98%EF%BC%8C%E5%A6%82%E6%9E%9Cdepth.plannar%E7%9A%84%E5%88%86%E8%BE%A8%E7%8E%87%E5%BE%88%E5%A4%A7%EF%BC%8Cairsim%E8%8E%B7%E5%8F%96%E6%B7%B1%E5%BA%A6%E5%9B%BE%E7%9A%84%E6%97%B6%E9%97%B4%E4%BC%9A%E9%9D%9E%E5%B8%B8%E5%B0%B1%EF%BC%8C1000%E5%88%86%E8%BE%A8%E7%8E%87%E8%A6%81%E5%87%A0%E4%B9%8E1%E5%88%86%E5%8D%8A%E7%9A%84%E6%97%B6%E9%97%B4)

---

Readme from Colosseum

# Welcome to Colosseum, a successor of [AirSim](https://github.com/microsoft/AirSim)

## Build Status

[![Ubuntu Build](https://github.com/CodexLabsLLC/Colosseum/actions/workflows/test_ubuntu.yml/badge.svg)](https://github.com/CodexLabsLLC/Colosseum/actions/workflows/test_ubuntu.yml)
[![MacOS Build](https://github.com/CodexLabsLLC/Colosseum/actions/workflows/test_macos.yml/badge.svg)](https://github.com/CodexLabsLLC/Colosseum/actions/workflows/test_macos.yml)
[![Windows Build](https://github.com/CodexLabsLLC/Colosseum/actions/workflows/test_windows.yml/badge.svg)](https://github.com/CodexLabsLLC/Colosseum/actions/workflows/test_windows.yml)

[![](https://dcbadge.vercel.app/api/server/y9ZJKKKn8J)](https://discord.gg/y9ZJKKKn8J)

## Looking for more performance?

The company managing this repo created the SWARM Developer System to help build, simulate and deploy single and
multi-agent autonomous systems. Check it out here: [SWARM Developer System](https://www.swarmsim.io/overview/developer)

## IMPORTANT ANNOUNCEMENT

Moving forward, we are now using Unreal Engine 5 version 5.03 or greater! If you
want to use UE4.27, you can use the branch `ue4.27`.

## Unreal Engine Version for Main Branch

The main branch of this repository **only** supports Unreal Engine 5.2! Please see our other branches
for other versions that we support.

## Currently Supported Operating Systems

Below are the list of officially supported Operating Systems, with full Unreal Engine support:

### Windows

- Windows 10 (Latest)

### Linux

- ~~Ubuntu 18.04~~ (NO LONGER SUPPORTED. 18.04 is EOL so we will not be checking this anymore and GitHub doesn't support CI builds)
- Ubuntu 20.04

**NOTE** Ubuntu 22.04 is not currently supported due to Vulkan support. If this changes, we will notify you here. If you want to use Colosseum on 22.04, we highly recommend that you use Docker.

### MacOS (Non-M1 Macs only)

- MacOS Monterey (12)
- MacOS (11)

**NOTE** MacOS support is highly experimental and may be dropped in future releases. This is because Apple continually changes their build tools and doesn't like 3rd party developers in general. There are ongoing discussions to remove this support.

## Sponsors

1. Codex Laboratories LLC [Website](https://www.codex-labs-llc.com)

## Introduction

Colosseum is a simulator for robotic, autonomous systems, built on [Unreal Engine](https://www.unrealengine.com/) (we now also have an experimental [Unity](https://unity3d.com/) release). It is open-source, cross platform, and supports software-in-the-loop simulation with popular flight controllers such as PX4 & ArduPilot and hardware-in-loop with PX4 for physically and visually realistic simulations. It is developed as an Unreal plugin that can simply be dropped into any Unreal environment. Similarly, we have an experimental release for a Unity plugin.

This is a fork of the AirSim repository, which Microsoft decided to shutdown in July of 2022. This fork serves as a waypoint to building a new and better simulation platform. The creater and maintainer of this fork is Codex Laboratories LLC (our website is [here](https://www.codex-labs-llc.com)). Colosseum is one of the underlying simulation systems that we use in our product, the [SWARM Simulation Platform](https://www.swarmsim.io). This platform exists to provide pre-built tools and low-code/no-code autonomy solutions. Please feel free to check this platform out and reach out if interested.

## Join the Community

We have decided to create a Discord channel to better allow for community engagement. Join here: [Colosseum Robotics Discord](https://discord.gg/y9ZJKKKn8J).

## Goals and Project Development

This section will contain a list of the current features that the community and Codex Labs are working on to support and build.

Click [here](https://docs.google.com/document/d/1doohQTos4v1tg4Wv6SliQFnKNK1MouKX2efg2mapXFU/edit?usp=sharing) to view our current development goals!

If you want to be apart of the official development team, attend meetings, etc., please utilize the Slack channel (link above) and
let Tyler Fedrizzi know!

## License

This project is released under the MIT License. Please review the [License file](LICENSE) for more details.
