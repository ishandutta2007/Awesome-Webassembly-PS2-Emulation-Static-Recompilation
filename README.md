# Awesome WebAssembly PS2 Emulation & Static Recompilation

[![Awesome](https://awesome.re/badge.svg)](https://awesome.re)
[![WebAssembly](https://img.shields.io/badge/WebAssembly-Wasm-654FF0?logo=webassembly&logoColor=white)](https://webassembly.org/)
[![WebGPU](https://img.shields.io/badge/WebGPU-Graphics-blue)](https://www.w3.org/TR/webgpu/)
[![PlayStation 2](https://img.shields.io/badge/PlayStation%202-EE%20%2F%20GS-003791?logo=playstation&logoColor=white)](https://en.wikipedia.org/wiki/PlayStation_2)

> A curated list of leading cloud gaming SaaS platforms, browser-based WebAssembly runtimes, static recompilers, WebGPU graphics renderers, and open-source emulation ecosystems for the Sony PlayStation 2 and 6th-generation consoles.

**Curated Directory of Cloud Streaming SaaS Products & Open-Source GitHub Projects**  
*Focused on Browser-Based PS2 Emulation, Ahead-of-Time Static Recompilation, WebGPU/WebGL Renderers, and Retro Gaming Runtimes*  
**Last updated:** November 2026

This directory (`Awesome-Webassembly-PS2-Emulation-Static-Recompilation`) monitors the evolution of next-generation gaming runtimes: translating PlayStation 2 Emotion Engine (MIPS R5900) machine code into portable C++ and WebAssembly (Wasm), running PCSX2 and Libretro cores locally inside web browsers, leveraging WebGPU for hardware Graphics Synthesizer (GS) rasterization, or streaming 6th-gen console classics via low-latency cloud infrastructure.

---

## Table of Contents

- [Sector Overview & Market Dynamics](#sector-overview--market-dynamics)
- [SaaS & Hosted Cloud Platforms](#saas--hosted-cloud-platforms)
- [Open-Source GitHub Projects](#open-source-github-projects)
- [Key Architectural Approaches](#key-architectural-approaches)
- [How to Contribute](#how-to-contribute)
- [License & Disclaimer](#license--disclaimer)

---

## Sector Overview & Market Dynamics

The global cloud gaming and browser runtime ecosystem is estimated at **$4.9B to $6.5B in 2026** (scaling toward **$21B–$100B+ by 2030** at an estimated CAGR exceeding 40%). The sector exhibits **moderate fragmentation across specialized tiers**: while high-bandwidth cloud streaming infrastructure is **concentrated among hyper-scale platform holders** (Sony PlayStation, NVIDIA GeForce NOW, and cloud telecom alliances), the client-side WebAssembly, static recompilation, and retro software preservation landscape remains **highly fragmented and community-driven**, powered by decentralized open-source emulator developers, reverse engineers, and independent Wasm runtime hackers.

---

## SaaS & Hosted Cloud Platforms

The table below catalogs commercial hosted platforms, cloud gaming streaming providers, and proprietary console frontends capable of running retro console software. Entries are sorted descending by company scale (market capitalization, valuation, or verified annual revenue).

| Platform | Company Scale (Valuation / Revenue) | Starting Tier Pricing | Free Tier / Trial Limits | Description |
| :--- | :--- | :--- | :--- | :--- |
| **[NVIDIA GeForce NOW](https://nvidia.com)** | ~$3.0T+ Market Cap / $120B+ Ann. Revenue (NVIDIA) | $9.99/month (Performance Tier, 1440p) or $19.99/month (Ultimate, 4K 240 FPS) | **Permanent Free Tier**: 1-hour session limit per launch, basic rig tier, ad-supported queue wait (up to 2 min video ads) | Ultra-low-latency cloud gaming service streaming PC and emulator-friendly game libraries directly to browsers, TVs, and mobile. |
| **[PlayStation Plus Cloud Streaming](https://playstation.com)** | ~$110B+ Market Cap / ~$85B+ Ann. Revenue (Sony Group) | $17.99/month or $159.99/year (PlayStation Plus Premium) | **7-Day Free Trial**: Available selectively to eligible new PSN accounts (requires active payment method; cancels before day 7) | Sony official cloud subscription catalog streaming PS2, PS3, PS4, and PS5 classics without local hardware requirements. |
| **[Boosteroid](https://boosteroid.com)** | ~$87M Annual Revenue / >8M Registered Users | €16.89/month (Ultra Plan) or €89.89/year (~€7.49/mo) | **No Free Tier / No Trial**: Full paid subscription required immediately to access servers | Independent European/US cloud gaming platform streaming PC games and custom desktop environments in-browser over WebRTC. |
| **[Shadow PC](https://shadow.tech)** | ~$10M–$50M Ann. Revenue (Jezby Ventures / Klaba) | $29.99/month (Shadow PC Lite) or $37.99/month (Neo) | **No Free Tier / No Trial**: Paid monthly subscription required (Lite tier has a 120-hour monthly limit and 4-hour session timeout) | Full cloud-hosted Windows PC with dedicated GPU acceleration capable of executing desktop PCSX2 instances remotely via any web browser. |
| **[Antstream Arcade](https://antstream.com)** | ~$7.7M Ann. Revenue / $20M+ Funding (Tencent & Atari backed) | $4.99/month (Monthly Pass), $39.99/year, or $99.99 Lifetime | **Permanent Free Tier**: Ad-supported access on Web/PC/Mobile restricted to bite-sized community challenges, score tournaments, and ad breaks | Cloud retro gaming subscription streaming over 1,300 officially licensed retro arcade and console classics directly inside web browsers and apps. |
| **[LaunchBox & Big Box](https://launchbox-app.com)** | Independent Private Developer (Unbroken Software, LLC) | $15.00/year (LaunchBox Premium updates) or $45.00 Lifetime License | **Permanent Free Version**: Unlimited desktop launcher and metadata scraper; Big Box couch/controller UI includes a **30-minute trial per launch** | Commercial desktop and Android emulation frontend organizing ROM/ISO game libraries, scraping art, and launching emulators with controller support. |
| **[DamonPS2](https://damonps2.com)** | Independent Mobile App Studio (>10M+ Play Store Downloads) | $9.99 one-time (DamonPS2 Pro standalone app or in-app purchase) | **Permanent Free Tier**: Ad-supported free version limited to 480p resolution, forced pre-game ads, restricted memory cards, and disabled gamepads | Commercial closed-source PlayStation 2 emulator for Android devices supporting hardware-accelerated graphics rendering and save states. |
| **[AetherSX2](https://aethersx2.com)** | Community Project / Former Solo Developer (Tahlreth) | $0.00 (Completely Free / No Paid Plans) | **100% Free Forever**: Full access to all features (unrestricted HD upscaling, save states, touchscreen, and physical gamepad mapping) | Closed-source ARM/Android port of PCSX2 delivering high-performance, high-compatibility PlayStation 2 emulation on mobile smartphones. |
| **[RetroGames.cc / PlayEmulator](https://retrogames.cc)** | Independent Web Emulation Portal (>5M+ Monthly Visits) | $0.00 (Free Ad-Supported Web Service) | **100% Free Forever**: Uncapped in-browser gameplay supported by on-page web banner and display advertisements | Hosted web retro-gaming portal running WebAssembly-compiled Libretro cores and retro console software directly inside standard browsers. |

---

## Open-Source GitHub Projects

The following table catalogs prominent open-source repositories spanning PlayStation 2 static recompilation, WebAssembly runtimes, browser emulators, and compiler toolchains. Projects are sorted descending by GitHub star count, with each star badge linking directly to the repository stargazers page.

| Repository | GitHub Stars | License | Primary Architecture / Language | Description |
| :--- | :--- | :--- | :--- | :--- |
| **[NationalSecurityAgency/ghidra](https://github.com/NationalSecurityAgency/ghidra)** | [![Stars](https://img.shields.io/github/stars/NationalSecurityAgency/ghidra?style=social&color=white)](https://github.com/NationalSecurityAgency/ghidra/stargazers) | Apache-2.0 | Java / C++ / Reverse Engineering | Premier software reverse-engineering framework used across static recompilation workflows to decompile Emotion Engine MIPS binaries and map function symbols. |
| **[emscripten-core/emscripten](https://github.com/emscripten-core/emscripten)** | [![Stars](https://img.shields.io/github/stars/emscripten-core/emscripten?style=social&color=white)](https://github.com/emscripten-core/emscripten/stargazers) | MIT / LLVM | C++ / Python / WebAssembly | Industry-standard LLVM-to-WebAssembly compiler toolchain compiling C/C++ emulator codebases (PCSX2, RetroArch, Play!) for web browser execution. |
| **[copy/v86](https://github.com/copy/v86)** | [![Stars](https://img.shields.io/github/stars/copy/v86?style=social&color=white)](https://github.com/copy/v86/stargazers) | BSD-2-Clause | Rust / WebAssembly / JavaScript | Fast x86 hardware virtualizer and JIT recompiler running entirely in the browser via WebAssembly, demonstrating browser-based binary translation. |
| **[ruffle-rs/ruffle](https://github.com/ruffle-rs/ruffle)** | [![Stars](https://img.shields.io/github/stars/ruffle-rs/ruffle?style=social&color=white)](https://github.com/ruffle-rs/ruffle/stargazers) | MIT / Apache-2.0 | Rust / WebAssembly / WebGPU | Modern Flash Player runtime emulator written in Rust and WebAssembly, pioneering memory-safe browser emulation and WebGPU hardware rendering. |
| **[gfx-rs/wgpu](https://github.com/gfx-rs/wgpu)** | [![Stars](https://img.shields.io/github/stars/gfx-rs/wgpu?style=social&color=white)](https://github.com/gfx-rs/wgpu/stargazers) | MIT / Apache-2.0 | Rust / WebGPU / Direct3D / Vulkan | Safe, portable graphics API based on the WebGPU specification, powering hardware-accelerated console graphics synthesizers and browser shaders. |
| **[OpenEmu/OpenEmu](https://github.com/OpenEmu/OpenEmu)** | [![Stars](https://img.shields.io/github/stars/OpenEmu/OpenEmu?style=social&color=white)](https://github.com/OpenEmu/OpenEmu/stargazers) | BSD-3-Clause | Objective-C / Swift / Metal | Modular retro console emulation frontend providing automated game library management, gamepad mapping, and core orchestration for macOS. |
| **[PCSX2/pcsx2](https://github.com/PCSX2/pcsx2)** | [![Stars](https://img.shields.io/github/stars/PCSX2/pcsx2?style=social&color=white)](https://github.com/PCSX2/pcsx2/stargazers) | GPL-3.0 | C++ / MIPS R5900 JIT / Vulkan | The authoritative open-source PlayStation 2 emulator featuring JIT recompilers, Vulkan/OpenGL/Metal GS renderers, and near-universal game compatibility. |
| **[dolphin-emu/dolphin](https://github.com/dolphin-emu/dolphin)** | [![Stars](https://img.shields.io/github/stars/dolphin-emu/dolphin?style=social&color=white)](https://github.com/dolphin-emu/dolphin/stargazers) | GPL-2.0+ | C++ / PowerPC JIT / Vulkan | Groundbreaking 6th-generation console emulator (GameCube/Wii) featuring experimental WebAssembly/Emscripten research builds for browser play. |
| **[hrydgard/ppsspp](https://github.com/hrydgard/ppsspp)** | [![Stars](https://img.shields.io/github/stars/hrydgard/ppsspp?style=social&color=white)](https://github.com/hrydgard/ppsspp/stargazers) | GPL-2.0+ | C++ / WebAssembly / Vulkan | High-speed PSP emulator with official Emscripten WebAssembly browser targets and cross-platform mobile/desktop HLE architectures. |
| **[libretro/RetroArch](https://github.com/libretro/RetroArch)** | [![Stars](https://img.shields.io/github/stars/libretro/RetroArch?style=social&color=white)](https://github.com/libretro/RetroArch/stargazers) | GPL-3.0 | C / WebAssembly / Libretro API | Flagship cross-platform frontend for Libretro emulation cores, featuring official WebAssembly browser builds (web player) and dynamic shader pipelines. |
| **[stenzek/duckstation](https://github.com/stenzek/duckstation)** | [![Stars](https://img.shields.io/github/stars/stenzek/duckstation?style=social&color=white)](https://github.com/stenzek/duckstation/stargazers) | GPL-3.0 | C++ / JIT / Vulkan | High-accuracy PlayStation 1 emulator featuring PGXP perspective precision, upscaling, and community-driven WebAssembly browser experiments. |
| **[WebAssembly/binaryen](https://github.com/WebAssembly/binaryen)** | [![Stars](https://img.shields.io/github/stars/WebAssembly/binaryen?style=social&color=white)](https://github.com/WebAssembly/binaryen/stargazers) | Apache-2.0 | C++ / WebAssembly Optimizer | Compiler infrastructure and toolchain library optimizing Wasm binaries generated by static recompilers and emulator transpilers. |
| **[N64Recomp/N64Recomp](https://github.com/N64Recomp/N64Recomp)** | [![Stars](https://img.shields.io/github/stars/N64Recomp/N64Recomp?style=social&color=white)](https://github.com/N64Recomp/N64Recomp/stargazers) | GPL-3.0 / MIT | C++ / MIPS III / Static Recompilation | Pioneering offline static recompiler translating N64 MIPS binaries and RSP microcode into clean, recompilable C code for native PC and WebAssembly builds. |
| **[Zelda64Recomp/Zelda64Recomp](https://github.com/Zelda64Recomp/Zelda64Recomp)** | [![Stars](https://img.shields.io/github/stars/Zelda64Recomp/Zelda64Recomp/stargazers) | GPL-3.0 | C / C++ / RT64 Renderer | High-profile native PC port of Majora's Mask generated via N64Recomp static recompilation, supporting unlocked frame rates and RT64 enhancements. |
| **[hedge-dev/UnleashedRecomp](https://github.com/hedge-dev/UnleashedRecomp)** | [![Stars](https://img.shields.io/github/stars/hedge-dev/UnleashedRecomp?style=social&color=white)](https://github.com/hedge-dev/UnleashedRecomp/stargazers) | GPL-3.0 | C++ / PowerPC Recompilation | Unofficial native PC port of Sonic Unleashed (Xbox 360) created via ahead-of-time static recompilation with high-resolution rendering. |
| **[EmulatorJS/EmulatorJS](https://github.com/EmulatorJS/EmulatorJS)** | [![Stars](https://img.shields.io/github/stars/EmulatorJS/EmulatorJS?style=social&color=white)](https://github.com/EmulatorJS/EmulatorJS/stargazers) | GPL-3.0 | JavaScript / WebAssembly | Self-hostable web emulation frontend compiling RetroArch cores to WebAssembly, featuring cloud saves, netplay, and virtual touch controls. |
| **[ran-j/PS2Recomp](https://github.com/ran-j/PS2Recomp)** | [![Stars](https://img.shields.io/github/stars/ran-j/PS2Recomp?style=social&color=white)](https://github.com/ran-j/PS2Recomp/stargazers) | GPL-3.0 | C++ / MIPS R5900 / Static Recompiler | Advanced PlayStation 2 static recompiler and runtime framework translating PS2 ELF binaries into portable C++ to produce native PC and Wasm ports. |
| **[Trixarian/NetherSX2-patch](https://github.com/Trixarian/NetherSX2-patch)** | [![Stars](https://img.shields.io/github/stars/Trixarian/NetherSX2-patch?style=social&color=white)](https://github.com/Trixarian/NetherSX2-patch/stargazers) | Shell / Smali / Python | Community maintenance and patching suite removing advertisements and restoring frontend launch features in AetherSX2 builds. |
| **[jpd002/Play-](https://github.com/jpd002/Play-)** | [![Stars](https://img.shields.io/github/stars/jpd002/Play-?style=social&color=white)](https://github.com/jpd002/Play-/stargazers) | MIT | C++ / WebAssembly (PlayJS) | Lightweight cross-platform PS2 emulator with a built-in High-Level Emulation (HLE) BIOS and official WebAssembly browser target (`PlayJS`). |
| **[peiikai/LASRecomp](https://github.com/peiikai/LASRecomp)** | [![Stars](https://img.shields.io/github/stars/peiikai/LASRecomp?style=social&color=white)](https://github.com/peiikai/LASRecomp/stargazers) | GPL-3.0 | C++ / ARM64 / Static Recompilation | Static recompilation project converting Link's Awakening into native executables for macOS, Windows, Linux, iOS, and Android. |
| **[rt64/rt64](https://github.com/rt64/rt64)** | [![Stars](https://img.shields.io/github/stars/rt64/rt64?style=social&color=white)](https://github.com/rt64/rt64/stargazers) | MIT / GPL-3.0 | C++ / DirectX 12 / Vulkan | Hardware-accelerated graphics renderer designed for static recompilation ports, delivering ray tracing, ultrawide rendering, and high frame rates. |
| **[mupen64plus/mupen64plus-core](https://github.com/mupen64plus/mupen64plus-core)** | [![Stars](https://img.shields.io/github/stars/mupen64plus/mupen64plus-core?style=social&color=white)](https://github.com/mupen64plus/mupen64plus-core/stargazers) | GPL-2.0+ | C / Plugin Architecture | Modular N64 emulator core serving as the foundation for WebAssembly browser ports and Libretro emulation cores. |
| **[adriadam10/mkw-recomp](https://github.com/adriadam10/mkw-recomp)** | [![Stars](https://img.shields.io/github/stars/adriadam10/mkw-recomp?style=social&color=white)](https://github.com/adriadam10/mkw-recomp/stargazers) | GPL-3.0 | C++ / Static Recompilation | Experimental static recompilation converting console binary code into a standalone native desktop application. |
| **[snuri00/ps2-web-recomp](https://github.com/snuri00/ps2-web-recomp)** | [![Stars](https://img.shields.io/github/stars/snuri00/ps2-web-recomp?style=social&color=white)](https://github.com/snuri00/ps2-web-recomp/stargazers) | MIT | C++ / WebAssembly / WebGPU | Milestone project running PlayStation 2 games in web browsers via static MIPS R5900 recompilation to Wasm paired with a WebGPU Graphics Synthesizer. |
| **[google/dawn](https://github.com/google/dawn)** | [![Stars](https://img.shields.io/github/stars/google/dawn?style=social&color=white)](https://github.com/google/dawn/stargazers) | BSD-3-Clause | C++ / WebGPU Specification | Google's native WebGPU implementation facilitating hardware-accelerated GPU pipelines across Chromium browsers and standalone Wasm runtimes. |
| **[arcanite24/pinyon-shift](https://github.com/arcanite24/pinyon-shift)** | [![Stars](https://img.shields.io/github/stars/arcanite24/pinyon-shift?style=social&color=white)](https://github.com/arcanite24/pinyon-shift/stargazers) | GPL-3.0 | C++ / Static Recompilation | Static recompilation runtime exploring ahead-of-time binary translation and native rendering pipelines for 7th-gen titles. |
| **[TGP482/BLACK-XBERecomp](https://github.com/TGP482/BLACK-XBERecomp)** | [![Stars](https://img.shields.io/github/stars/TGP482/BLACK-XBERecomp?style=social&color=white)](https://github.com/TGP482/BLACK-XBERecomp/stargazers) | GPL-3.0 | C++ / Xbox Recompilation | Ahead-of-time static recompiler translating original Xbox XBE binaries of Criterion's BLACK into native PC executables. |
| **[sp00nznet/ps3recomp](https://github.com/sp00nznet/ps3recomp)** | [![Stars](https://img.shields.io/github/stars/sp00nznet/ps3recomp?style=social&color=white)](https://github.com/sp00nznet/ps3recomp/stargazers) | GPL-3.0 | C++ / Cell Broadband Engine | Static recompilation runtime and library suite decoding PlayStation 3 PowerPC/SPU binaries into native PC code. |
| **[snuri00/psp-web-recomp](https://github.com/snuri00/psp-web-recomp)** | [![Stars](https://img.shields.io/github/stars/snuri00/psp-web-recomp?style=social&color=white)](https://github.com/snuri00/psp-web-recomp/stargazers) | MIT | C++ / WebAssembly / WebGL2 | PlayStation Portable static recompiler translating MIPS Allegrex code to WebAssembly with an HLE kernel and WebGL2 renderer. |
| **[jessicanataliagta/PSPRecomp](https://github.com/jessicanataliagta/PSPRecomp)** | [![Stars](https://img.shields.io/github/stars/jessicanataliagta/PSPRecomp?style=social&color=white)](https://github.com/jessicanataliagta/PSPRecomp/stargazers) | GPL-3.0 | C++ / PSP Recompilation | Static recompilation framework for PSP software generating native PC binaries with high-framerate support. |
| **[KIexster/god-of-war-recomp](https://github.com/KIexster/god-of-war-recomp)** | [![Stars](https://img.shields.io/github/stars/KIexster/god-of-war-recomp?style=social&color=white)](https://github.com/KIexster/god-of-war-recomp/stargazers) | GPL-3.0 | C++ / PS2Recomp | Native PC port of God of War (PS2) generated via ahead-of-time static recompilation using PS2Recomp with ultrawide and modern controller input. |
| **[exoteric33/ps2-native-recomp](https://github.com/exoteric33/ps2-native-recomp)** | [![Stars](https://img.shields.io/github/stars/exoteric33/ps2-native-recomp?style=social&color=white)](https://github.com/exoteric33/ps2-native-recomp/stargazers) | MIT | C++ / PS2 Binary Translation | Standalone static recompilation pipeline converting PS2 disc images into native Windows and Linux executables based on ps2-web-recomp. |
| **[TabStationToo/TabStationToo](https://github.com/TabStationToo/TabStationToo)** | [![Stars](https://img.shields.io/github/stars/TabStationToo/TabStationToo?style=social&color=white)](https://github.com/TabStationToo/TabStationToo/stargazers) | GPL-3.0 | WebAssembly / C++ / PCSX2 | In-browser PlayStation 2 emulator porting PCSX2 to WebAssembly, enabling users to boot PS2 ISOs directly in Chrome or Edge tabs. |
| **[sal063/Ace-Combat-5-Static-recompilation](https://github.com/sal063/Ace-Combat-5-Static-recompilation)** | [![Stars](https://img.shields.io/github/stars/sal063/Ace-Combat-5-Static-recompilation?style=social&color=white)](https://github.com/sal063/Ace-Combat-5-Static-recompilation/stargazers) | GPL-3.0 | C++ / PS2 Recompilation | Static recompilation project bringing Ace Combat 5: The Unsung War to native platforms with custom rendering. |
| **[n64hub/super-mario-64-recomp](https://github.com/n64hub/super-mario-64-recomp)** | [![Stars](https://img.shields.io/github/stars/n64hub/super-mario-64-recomp?style=social&color=white)](https://github.com/n64hub/super-mario-64-recomp/stargazers) | MIT | C / WebAssembly | Static recompilation build of Super Mario 64 targeting both desktop PCs and web browsers via N64Recomp and Wasm runtimes. |
| **[koaque/Metropolismania-PC](https://github.com/koaque/Metropolismania-PC)** | [![Stars](https://img.shields.io/github/stars/koaque/Metropolismania-PC?style=social&color=white)](https://github.com/koaque/Metropolismania-PC/stargazers) | GPL-3.0 | C++ / PS2Recomp Runtime | Native PC port of Metropolismania (PS2) via PS2Recomp static binary translation and incremental runtime patching. |

---

## Key Architectural Approaches

1. **Ahead-of-Time (AOT) Static Recompilation:**  
   Instead of interpreting machine code or translating instructions just-in-time (JIT) at runtime, static recompilers (e.g., `PS2Recomp`, `ps2-web-recomp`, `N64Recomp`) lift binary machine instructions (such as MIPS R5900 Emotion Engine or Allegrex) into portable intermediate C++ or LLVM IR. The translated code is subsequently compiled with modern optimizing compilers (Clang, GCC, or Emscripten) into native x86/ARM executables or WebAssembly modules. This technique delivers deterministic performance, zero JIT compilation stutter, and frictionless deployment to web browsers.

2. **WebGPU Graphics Synthesizer Pipelines:**  
   The PlayStation 2 Graphics Synthesizer (GS) possesses a massive internal memory bandwidth (48 GB/s on-chip eDRAM) that historically posed severe bottlenecks for PC emulation. Modern browser recompilers and emulators leverage **WebGPU compute and render pipelines** (`wgpu`, `google/dawn`) to emulate custom GS blend modes, scissor registers, and texture sampling directly on modern client GPUs inside Chromium and WebKit browsers.

3. **Cloud Game Streaming vs. Client-Side Wasm Runtimes:**  
   * **Cloud SaaS Platforms** (`GeForce NOW`, `PlayStation Plus`, `Boosteroid`, `Shadow PC`) execute game binaries on dedicated remote server rigs equipped with hardware GPUs, transmitting audio/video frames via low-latency WebRTC streams.  
   * **WebAssembly Runtimes** (`ps2-web-recomp`, `TabStationToo`, `Play!`, `EmulatorJS`) run 100% locally on the user device inside the browser sandbox, preserving user privacy, enabling offline play, and eliminating streaming infrastructure costs.

---

## How to Contribute

Contributions are welcome! Please follow these guidelines:
1. Ensure the project is directly related to WebAssembly, PlayStation 2 emulation, static recompilation, or browser retro gaming.
2. Maintain alphabetical ordering for new categories and star-count sorting for repository entries.
3. Keep descriptions factual, concise, and neutral.
4. Verify all hyperlinks and repository references before submitting a pull request.

---

## License & Disclaimer

- Distributed under the [MIT License](LICENSE).
- All product names, trademarks, and registered trademarks belong to their respective owners (Sony Interactive Entertainment Inc., NVIDIA Corporation, etc.). Their mention in this repository is strictly for descriptive, identification, and educational purposes.
