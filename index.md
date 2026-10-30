---
layout: home
title: Fluorite - Home
---

# Fluorite

Fluorite is a Linux distribution that replaces almost every layer above the kernel. It is built by one developer with a focus on architecture and user experience.

## What do we have?

**Custom desktop environment** called *fldesktop*. It is built using Python and PySide6. It also holds all the subsystems, all the beautiful and all the messy code together.

**ExtSvInit subsystem.** *fldesktop* runs as PID 2 and manages everything, including system services (such as CUPS and NetworkManager). No systemd included ;)

**Server-side UI.** Powered by FS3. Applications can create widgets as nodes, reparent them with relations, call methods, edit attributes and receive events. Widgets are drawn by Qt in *fldesktop*, which means that every application will have similar theming. We also have *FVGI* icon system to create beautiful icons without any SVG.

**FS3 subsystem.** FS3, which stands for *"Fluorite Semantic Storage System"*, is a node-based storage system. Data is stored as nodes with attributes, not as files in a hierarchy. They are connected by Relations (which are a node species). A photo may have a place, a time, and a context.

**Atomic architecture.** The entire system is a single UKI (Unified Kernel Image) with the root filesystem embedded. Updates replace the image. Rollback is instant.

**SuperFX subsystem.** An OpenGL compositor for glassy windows/panels/menus. A software fallback exists for hardware without GPU acceleration.

**Compatibility layers.** There is an X11 bridge called *x2agv* to show legacy X11 apps UI in Fluorite (WIP).

**And much more**

## Status
### Current codename: Dawn

Dawn is the first release, planned for december 2026. It is an experimental preview: the core architecture schould work, but a lot of things, such as system installer, are delayed to codename *"Endeavour"*. **Not recommended for daily use. You have been warned.**

## Philosophy

Fluorite is not trying to be the next Windows or macOS. It is trying to be an OS that feels considered - one where the architecture and the interface are designed together, not assembled from parts. UI/UX was inspired from Windows Vista/7 and pre-reset Longhorn builds.