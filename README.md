# Awesome-Webassembly-PS2-Emulation-Static-Recompilation

## Top WebAssembly PS2 Emulation & Static Recompilation Ecosystem



**Curated List of SaaS Products & Open-Source GitHub Projects**  

*Focused on Browser-Based PS2 Emulation, Ahead-of-Time Static Recompilation, WebGPU Renderers & Retro Gaming Runtimes*  

**Last updated: November 2026**



This repository (`Awesome-Webassembly-PS2-Emulation-Static-Recompilation`) tracks notable **SaaS/Cloud Gaming platforms** and **open-source projects** for **WebAssembly PS2 Emulation & Static Recompilation** — Top Webassembly PS2 Emulation Static Recompilation (Opensource) 🌟 Star if you like it! 🌟. These tools translate PlayStation 2 Emotion Engine (MIPS R5900) machine code into C++ and WebAssembly, compile traditional PS2 emulators to Wasm, leverage WebGPU for Graphics Synthesizer rendering, or stream console classics over the cloud.



**Examples** include RetroArch, PCSX2, AetherSX2, Play! PS2, DamonPS2, Antstream Arcade, LaunchBox, GeForce NOW, Boosteroid, Shadow PC, and `snuri00/ps2-web-recomp` (the category leaders).



**Open-source emphasis**: This section is heavily expanded with every major active project for PS2 static recompilation to WebAssembly and native C++, browser-based PS2/PSP/N64 Wasm runtimes, and open-source PS2/mobile emulators — ideal for emulation engineers, WebAssembly developers, retro preservationists, and browser game hackers.



Contributions welcome! Open a PR to add/update entries. Keep descriptions factual and link to official sites.



## Table of Contents

- [SaaS/Hosted Platforms](#saashosted-platforms)

- [Open-Source GitHub Projects](#open-source-github-projects)

- [How to Contribute](#how-to-contribute)

- [Disclaimer](#disclaimer)



## SaaS/Hosted Platforms



- **[Antstream Arcade](https://antstream.com)**  

  Cloud retro gaming subscription platform streaming thousands of licensed classic console and arcade titles directly to browsers, PCs, and mobile devices.



- **[PlayStation Plus Cloud Streaming](https://playstation.com)**  

  Official Sony cloud streaming tier offering on-demand access to select PlayStation 2, PS3, and PS4 classics without local hardware emulation.



- **[NVIDIA GeForce NOW](https://nvidia.com)**  

  High-performance cloud gaming service streaming PC titles and user-owned libraries at high framerates to web browsers and low-power devices.



- **[Boosteroid](https://boosteroid.com)**  

  Browser-accessible cloud gaming platform providing instant streaming of desktop games and custom applications over WebRTC.



- **[Shadow PC](https://shadow.tech)**  

  Full Windows cloud workstation with dedicated GPU acceleration capable of running heavy desktop emulators like PCSX2 remotely from any browser or phone.



- **[LaunchBox & Big Box](https://launchbox-app.com)**  

  Commercial desktop and Android emulation frontend organizing ROM/ISO libraries, metadata scraping, and one-click emulator launching.



- **[AetherSX2](https://aethersx2.com)**  

  Closed-source ARM/Android port of PCSX2 delivering high-compatibility PlayStation 2 emulation on smartphones and tablets.



- **[DamonPS2](https://damonps2.com)**  

  Commercial proprietary PlayStation 2 emulator for Android devices supporting hardware-accelerated rendering and save states.



- **[RetroGames.cc / PlayEmulator (Web Hosting)](https://retrogames.cc)**  

  Hosted browser retro-gaming portals running WebAssembly-compiled Libretro cores directly inside standard web pages.



## Open-Source GitHub Projects



- **[ps2-web-recomp (snuri00/ps2-web-recomp)](https://github.com/snuri00/ps2-web-recomp)**  

  Groundbreaking open-source project running PlayStation 2 games in the browser via ahead-of-time static recompilation of Emotion Engine (R5900) machine code to C++ and WebAssembly, paired with a WebGPU Graphics Synthesizer renderer.



- **[PS2Recomp (ran-j/PS2Recomp)](https://github.com/ran-j/PS2Recomp)**  

  Open-source PlayStation 2 static recompiler and runtime framework that parses PS2 ELF binaries, decodes MIPS R5900 instructions into C++, and links them with an IOP/GS runtime for native PC ports.



- **[ps2-native-recomp (exoteric33/ps2-native-recomp)](https://github.com/exoteric33/ps2-native-recomp)**  

  MIT-licensed open-source static recompiler built on `ps2-web-recomp` that converts PS2 disc images into standalone native Windows and Linux executables without game-specific patches.



- **[God of War: Recompiled (KIexster/god-of-war-recomp)](https://github.com/KIexster/god-of-war-recomp)**  

  Open-source native PC port of God of War (PS2) generated via static MIPS R5900 recompilation using `PS2Recomp` with ultrawide and modern controller support.



- **[Metropolismania-PC (koaque/Metropolismania-PC)](https://github.com/koaque/Metropolismania-PC)**  

  Open-source static recompilation PC port of Metropolismania (PS2) demonstrating incremental function replacement over `PS2Recomp` output.



- **[psp-web-recomp (snuri00/psp-web-recomp)](https://github.com)**  

  Sibling open-source static recompiler translating PlayStation Portable (MIPS Allegrex) binaries to WebAssembly with a High-Level Emulation (HLE) kernel and WebGL2 renderer.



- **[TabStationToo (TabStationToo/TabStationToo)](https://github.com/TabStationToo/TabStationToo)**  

  Open-source browser-based PlayStation 2 emulator compiling PCSX2 to WebAssembly so users can run BIOS and disc images locally inside a Chrome or Edge tab.



- **[Play! PS2 Emulator (jpd002/Play-)](https://github.com/jpd002/Play-)**  

  Cross-platform open-source PlayStation 2 emulator featuring a built-in HLE BIOS (no external BIOS dump required) and an official Emscripten WebAssembly browser target (`PlayJS`).



- **[PCSX2 (PCSX2/pcsx2)](https://github.com)**  

  The premier open-source PlayStation 2 emulator for Windows, Linux, and macOS featuring JIT recompilers, Vulkan/OpenGL/D3D12 GS renderers, and near-complete library compatibility.



- **[NetherSX2 Patcher (Trixarian/NetherSX2-patch)](https://github.com)**  

  Open-source community patching suite that removes ads, restores frontend launcher support, and updates controller profiles for AetherSX2 on Android.



- **[RetroArch (libretro/RetroArch)](https://github.com)**  

  Flagship open-source cross-platform frontend for Libretro emulation cores, featuring an official Emscripten WebAssembly web player (`://libretro.com`) and shaders.



- **[LRPS2 (libretro/LRPS2)](https://github.com)**  

  Official open-source Libretro core bringing PCSX2's PlayStation 2 emulation engine into RetroArch and compatible frontend ecosystems.



- **[EmulatorJS (EmulatorJS/EmulatorJS)](https://github.com)**  

  Self-hostable open-source web emulation frontend wrapping RetroArch WebAssembly cores with save states, netplay, and mobile touch controls.



- **[N64Recomp (N64Recomp/N64Recomp)](https://github.com/N64Recomp/N64Recomp)**  

  Pioneering open-source static recompiler translating Nintendo 64 MIPS binaries and RSP microcode into portable C code for native and WebAssembly builds.



- **[Zelda 64: Recompiled (Zelda64Recomp/Zelda64Recomp)](https://github.com/Zelda64Recomp/Zelda64Recomp)**  

  High-profile open-source static recompilation port of Majora's Mask powered by `N64Recomp` and the `RT64` renderer for unlocked framerates and widescreen play.



- **[Super Mario 64 Web/PC Recomp (n64hub/super-mario-64-recomp)](https://github.com/n64hub/super-mario-64-recomp)**  

  Open-source static recompilation port of Super Mario 64 targeting both desktop PCs and WebAssembly browsers via `N64Recomp-browser`.



- **[PPSSPP (hrydgard/ppsspp)](https://github.com)**  

  Ultra-fast open-source PSP emulator written in C++ with official WebAssembly/Emscripten builds and Vulkan/WebGL rendering backends.



- **[DuckStation (stenzek/duckstation)](https://github.com)**  

  High-accuracy open-source PlayStation 1 emulator featuring upscaling, PGXP perspective correction, and community WebAssembly ports.



- **[Dolphin Emulator (dolphin-emu/dolphin)](https://github.com)**  

  Industry-leading open-source GameCube and Wii emulator with experimental WebAssembly/Emscripten research forks for browser-based 6th-gen console emulation.



- **[v86 (copy/v86)](https://github.com)**  

  Open-source x86 PC emulator and virtualizer compiled to WebAssembly, capable of booting full operating systems and retro software directly in JavaScript.



- **[Ruffle (ruffle-rs/ruffle)](https://github.com)**  

  Memory-safe open-source Flash Player emulator written in Rust and compiled to WebAssembly with WebGPU rendering, setting the standard for browser media preservation.



### Additional Strong Open-Source Options



- **[Emscripten](https://github.com)** and **[Binaryen](https://github.com)** core open-source LLVM-to-WebAssembly compiler toolchains enabling C/C++ emulators and static recompilers to run in browsers.

- **[wgpu (gfx-rs/wgpu)](https://github.com)** and **[Google Dawn](https://googlesource.com)** open-source WebGPU implementations powering native-speed console graphics shaders on the web.

- **[Ghidra](https://github.com)** and **[ghidra-emotionengine-reloaded](https://github.com)** open-source reverse-engineering tools and PS2 Emotion Engine processor modules for generating function maps.

- **[RT64](https://github.com)** open-source hardware-accelerated graphics engine widely paired with static recompilation projects for high-framerate rendering.

- **[Pegasus Frontend](https://github.com)** and **[ES-DE (EmulationStation Desktop Edition)](https://gitlab.com)** open-source cross-platform alternatives to LaunchBox for organizing PS2 and retro libraries.
